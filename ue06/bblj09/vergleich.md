# Von Hand und mit dem Agenten – Terminplaner für die THM

Abgleich der vier handschriftlichen Goodnotes-Skizzen mit den digitalen Fassungen und der Fallbeschreibung. Die digitalen Fassungen und der Abgleich entstanden mit KI-Unterstützung.

## Aufgabe 1 – Use-Case-Diagramm

- Buchen, Stornieren, Anlegen, Absagen und der iCal-Download sind eigenständige Ziele. Das Erzeugen der 15-Minuten-Zeitfenster und die Benachrichtigungen stehen als Systemverhalten an den zugehörigen Use-Cases.
- Die Warteliste erweitert das Buchen nur bei einer ausgebuchten Sprechstunde. Der Pfeil zeigt vom erweiternden Use-Case auf den Basis-Use-Case.
- Die vier geschützten Aktionen beziehen die Anmeldung ein. Eine bestehende Sitzung kann weiterverwendet werden. Der Anmeldedienst steht als externer Akteur außerhalb der Systemgrenze.

**Korrektur in `usecase.puml`:** In der Skizze ist der linke Akteur unbeschriftet, und der Anmeldepfeil von „anlegen“ läuft durch das Oval „absagen“. Die digitale Fassung benennt den Akteur als Studierende und gibt für jede geschützte Aktion eine eigene Beziehung zur Anmeldung an. Die Wartelistenbedingung und die Nebenwirkungen stehen explizit im Modell.

## Aufgabe 2 – Aktivitätsdiagramm

- In der Skizze führen die Anmeldung, die bestehende Sitzung und der Buchungskonflikt direkt zum Anzeigen. In der digitalen Fassung führt der Konflikt über die Schleife zur erneuten Anzeige. Die drei parallelen Aktionen und der Abschluss nach dem Join bleiben erhalten.
- Verfügbarkeitsprüfung und Eintragen der Buchung müssen zusammen vor einer parallelen Buchung geschützt sein. Nach einem Konflikt werden die freien Zeitfenster erneut angezeigt.
- Die Bestätigung mit iCal-Datei, die Nachricht an die Lehrperson und das Vermerken des gebuchten Zeitfensters laufen parallel. Erst am Join ist die Buchung abgeschlossen.

**Die Änderung um die Warteliste:** Die Verzweigung greift nur, wenn die Liste freier Zeitfenster leer ist. Das gilt sowohl beim ersten Anzeigen als auch nach einer konkurrierenden Buchung. Die Studentin kann die Warteliste wählen oder den Vorgang beenden. Der erfolgreiche Buchungszweig bleibt dabei gleich.

## Aufgabe 3 – Klassendiagramm

Die Zahlen vergleichen die vorliegende Handskizze mit der digitalen Fassung. Ein unabhängiger Agentenlauf ohne Regeln wurde für diesen Vergleich nicht dokumentiert. Einträge werden pro fehlerhaftem Assoziationsende gezählt.

| Verstoß | Handskizze | digitale Fassung mit Regeln |
|---|---:|---:|
| künstliche Schlüssel | 0 | 0 |
| technische statt fachlicher Datentypen | 0 | 0 |
| Erfundenes (Attribute, Klassen, Operationen) | 0 | 0 |
| fehlende oder abweichende Multiplizitäten | 1 | 0 |
| Aggregation statt Komposition | 1 | 0 |

**Was die Regeln behoben haben:** In der Skizze steht beim Ende Lehrperson der Sekretariat-Beziehung „2..“ ohne obere Grenze. Die digitale Fassung verwendet `2..*`. Sie verwendet außerdem die Komposition anstelle der offenen Raute und den fachlichen Typ Uhrzeit für Beginn und Ende. „Mehrere“ wird als mindestens zwei gelesen.

### Meine Regeln für Datenmodelle

- Vorgaben aus Beschreibung 3 als Grenze für Klassen, Attribute und Beziehungen nehmen.
- Die vorgegebene Hochschulkennung übernehmen. Beziehungen über Assoziationen ausdrücken. Künstliche Schlüssel und technische Typen weglassen.
- Jede Assoziation an beiden Enden mit der passenden fachlichen Multiplizität angeben.
- Gemeinsame Kontoattribute in der Basisklasse modellieren.
- Für Sprechstunde und Zeitfenster eine Komposition verwenden.

## Aufgabe 4 – Zustandsdiagramm

Der Abgleich bezieht sich auf die Handskizze. Die digitale Mermaid-Fassung entstand mit KI-Unterstützung.

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| Der rechte Absagepfeil hat keinen Anschluss an Gebucht. | berechtigt | Auch gebuchte Zeitfenster müssen bei einer Absage der Sprechstunde nach Abgesagt wechseln. Die digitale Fassung enthält den Übergang. |
| Gesperrt verfällt bei Beginn. | als Einwand unberechtigt | Beschreibung 4 verlangt genau diesen Übergang. |
| Gebucht wechselt bei Stornierung wieder nach Frei. | als Einwand unberechtigt | Die Skizze nennt die Zwei-Stunden-Grenze. Die digitale Fassung schreibt sie als Bedingung. |

## Ein System, vier Sichten

### Was kommt mehrfach vor?

| Element | Use-Case | Aktivität | Klassen | Zustand |
|---|---|---|---|---|
| Zeitfenster | Zielobjekt beim Buchen | anzeigen, wählen, prüfen, als gebucht vermerken | Klasse und Teil der Sprechstunde | Objekt des gesamten Zustandsdiagramms |
| Buchung | buchen, stornieren, iCal herunterladen | prüfen, eintragen und bestätigen | Klasse mit Zeitpunkt und Anliegen | Ereignisse buchen und stornieren, Zustand Gebucht |
| Sprechstunde | anlegen und absagen | auswählen | Klasse mit Datum, Uhrzeit und Ort | Absage löst Übergänge aus |
| Studierende | Akteur | Verantwortungsbereich Studentin | spezialisierte Kontorolle | — |
| Lehrperson | Akteur | erhält Benachrichtigung | spezialisierte Kontorolle | sperrt, gibt frei oder sagt ab |
| Warteliste | bedingte Erweiterung beim Buchen | Alternative bei leerer Liste freier Zeitfenster | — | — |
| Hochschulkonto | Anmeldung mit externem Prüfdienst | Anmeldung bei fehlender Sitzung | gemeinsame Basisklasse der Rollen | — |

### Wo passt es nicht zusammen?

- Das fachliche Datenmodell enthält keine Warteliste, obwohl sie in der Funktionssicht und im Buchungsablauf vorkommt. Für eine Implementierung müsste geklärt werden, wie Wartelisteneinträge gespeichert werden.
- Im Ablauf wird die Buchung zuerst eingetragen und der Zustand anschließend parallel zu den Benachrichtigungen vermerkt. Das Zustandsdiagramm fasst beides als Übergang beim Buchen zusammen. Die Verfügbarkeitsprüfung muss daher bereits einen erfolgreich gespeicherten Buchungseintrag berücksichtigen, auch wenn der Zustandseintrag noch aussteht.

### Aus „Zeitfenster“ wird „Termin“

**Stellen:** In den vier Diagrammdateien steht das exakte Wort „Zeitfenster“ an **10 Stellen in 3 Dateien**. Davon sind 2 in `usecase.puml`, 5 in `aktivitaet.puml` und 3 in `klassen.md` (Klassendeklaration und beide Referenzen). In `zustand.md` ist zusätzlich die Überschrift mit der gebeugten Form „Zeitfensters“ anzupassen. Das ergibt einschließlich dieser Wortform **11 Stellen in 4 Dateien**. Begleittexte und Papierzeichnungen sind bei dieser Zählung ausgeklammert.
