# Von Hand und mit dem Agenten — Terminplaner für die THM

## Aufgabe 1 — Use-Case-Diagramm

- Der Agent hat die Anmeldung mit include-Beziehungen dargestellt.
- Die Warteliste wurde mit einer extend-Beziehung modelliert.
- Der Anmeldedienst wurde als externer Akteur dargestellt.
- Der Agent hat auch die Benachrichtigungen berücksichtigt.

**Meine Korrektur in usecase.puml :** Ich habe die Anmerkung zur Warteliste in eine eigene Zeile verschoben, um den Syntaxfehler zu korrigieren.

## Aufgabe 2 — Aktivitätsdiagramm

- Der Agent hat die beiden Bahnen Studentin und Terminplaner berücksichtigt.
- Bei einem vergebenen Zeitfenster führt der Ablauf zurück zur Anzeige der freien Zeitfenster.
- Die drei gleichzeitigen Aktionen wurden mit einer Gabelung und Vereinigung dargestellt.

**Die Änderung um die Warteliste:** Der Agent hat nur die neue Verzweigung ergänzt. Wenn kein Zeitfenster mehr frei ist, wird die Warteliste angeboten. Der Ablauf endet mit einem Endknoten. Der restliche Buchungsablauf blieb unverändert.

## Aufgabe 3 — Klassendiagramm

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | 0 | 0 |
| technische statt fachlicher Datentypen | 0 | 0 |
| Erfundenes (Attribute, Klassen, Operationen) | 0 | 0 |
| fehlende oder abweichende Multiplizitäten | 0 | 0 |
| Assoziation statt Komposition | 0 | 0 |

**Was die Regeln behoben haben und was nicht:** Beide Diagramme enthalten keine erkennbaren fachlichen Verstöße. Durch die Regeln wurden die Multiplizitäten mit 0..* genauer ausgeschrieben.

### Meine Regeln für Datenmodelle

- Keine künstlichen Schlüssel oder IDs erfinden.
- Nur fachliche Datentypen verwenden.
- Keine zusätzlichen Attribute, Klassen oder Operationen erfinden.
- Alle Multiplizitäten entsprechend der Fallbeschreibung angeben.
- Komposition verwenden, wenn ein Teil mit dem Ganzen gelöscht wird.

## Aufgabe 4 — Zustandsdiagramm

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| Keine fachlichen Abweichungen | Berechtigt | Alle Zustände, Übergänge und Bedingungen entsprechen der Beschreibung 4. |

## Ein System, vier Sichten

### Was kommt mehrfach vor?

| Element | Use-Case | Aktivität | Klassen | Zustand |
|---|---|---|---|---|
| Studierende | Akteur | Studentin als Bahn | Klasse Studierende | — |
| Lehrperson | Akteur | Lehrperson benachrichtigen | Klasse Lehrperson | — |
| Sprechstunde | Sprechstunde anlegen | Sprechstunde auswählen | Klasse Sprechstunde | — |
| Zeitfenster | Zeitfenster buchen | Zeitfenster auswählen | Klasse Zeitfenster | Modelliertes Objekt |
| Buchung | Buchen und stornieren | Buchung eintragen | Klasse Buchung | Gebucht |
| Warteliste | Use-Case | Aktion und Entscheidung | — | — |

### Wo passt es nicht zusammen?
- Die Warteliste kommt im Use-Case-Diagramm und im Aktivitätsdiagramm vor, fehlt aber im Klassendiagramm.
- Die Stornierung wird im Use-Case-Diagramm und im Zustandsdiagramm dargestellt, aber nicht im Aktivitätsdiagramm.
- Die Zwei-Stunden-Regel wird nur im Zustandsdiagramm ausdrücklich dargestellt.

### Aus „Zeitfenster“ wird „Termin“

**Stellen:** 14 in 5 Dateien

