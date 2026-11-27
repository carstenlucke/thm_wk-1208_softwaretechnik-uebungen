# Von Hand und mit dem Agenten — Terminplaner für die THM

<!-- Aufgaben 1 bis 4 des Übungsblatts und „Vor der nächsten Vorlesung“.
     Ersetzen Sie jedes „…“ durch Ihre Angabe und fügen Sie so viele
     Zeilen hinzu, wie Sie benötigen. Löschen Sie die Kommentare, sobald
     Sie fertig sind. -->

## Aufgabe 1 — Use-Case-Diagramm

- Der Agent hat die Anmeldung mit include-Beziehungen dargestellt.
- Die Warteliste wurde mit einer extend-Beziehung modelliert.
- Der Anmeldedienst wurde als externer Akteur dargestellt.
- Der Agent hat auch die Benachrichtigungen berücksichtigt.


**Meine Korrektur in usecase.puml :** Ich habe die Anmerkung zur Warteliste in eine eigene Zeile verschoben, um den Syntaxfehler zu korrigieren.

<!-- Schritt 6: was Sie selbst im Text geändert haben und warum. -->

## Aufgabe 2 — Aktivitätsdiagramm

- Der Agent hat die beiden Bahnen Studentin und Terminplaner berücksichtigt.
- Bei einem vergebenen Zeitfenster führt der Ablauf zurück zur Anzeige der freien Zeitfenster.
- Die drei gleichzeitigen Aktionen wurden mit einer Gabelung und Vereinigung dargestellt.



**Die Änderung um die Warteliste:** Der Agent hat nur die neue Verzweigung ergänzt. Wenn kein Zeitfenster mehr frei ist, wird die Warteliste angeboten. Der Ablauf endet mit einem Endknoten. Der restliche Buchungsablauf blieb unverändert.

## Aufgabe 3 — Klassendiagramm

<!-- Schritte 4 und 7: Zahl der Verstöße je Art, ohne und mit Ihren
     Regeln. -->

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | … | … |
| technische statt fachlicher Datentypen | … | … |
| Erfundenes (Attribute, Klassen, Operationen) | … | … |
| fehlende oder abweichende Multiplizitäten | … | … |
| Assoziation statt Komposition | … | … |

**Was die Regeln behoben haben und was nicht:** …

### Meine Regeln für Datenmodelle

<!-- Schritt 5: knapp und eindeutig, als Liste. Der Agent liest diesen
     Abschnitt in Schritt 6. -->

- …

## Aufgabe 4 — Zustandsdiagramm

<!-- Schritt 5: jede Abweichung, welche der Agent gemeldet hat, mit Ihrem
     Urteil (berechtigt / nicht berechtigt) und einem Satz Begründung. -->

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| … | … | … |

## Ein System, vier Sichten

<!-- Vor der nächsten Vorlesung. -->

### Was kommt mehrfach vor?

| Element | Use-Case | Aktivität | Klassen | Zustand |
|---|---|---|---|---|
| … | … | … | … | … |

<!-- Je Zelle: unter welchem Namen und in welcher Form das Element dort
     vorkommt (Akteur, Use-Case, Aktion, Klasse, Zustand …), oder „—“. -->

### Wo passt es nicht zusammen?

- …

### Aus „Zeitfenster“ wird „Termin“

**Stellen:** … in … Dateien



