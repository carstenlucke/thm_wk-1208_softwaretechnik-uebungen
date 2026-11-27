# Von Hand und mit dem Agenten — Terminplaner für die THM

<!-- Aufgaben 1 bis 4 des Übungsblatts und „Vor der nächsten Vorlesung“.
     Ersetzen Sie jedes „…“ durch Ihre Angabe und fügen Sie so viele
     Zeilen hinzu, wie Sie benötigen. Löschen Sie die Kommentare, sobald
     Sie fertig sind. -->

## Aufgabe 1 — Use-Case-Diagramm

- Der Agent hat im Gegensatz zu meiner Handskizze eine Systemgrenze eingezeichnet.
- Die Akteure werden als Strichmännchen und die Anwendungsfälle als Ovale dargestellt.
- Der Agent hat die Anmeldung als Vorbedingung statt als eigenen Use-Case modelliert.
- Die Warteliste wurde mit «extend» und der Bedingung [ausgebucht] dargestellt.
- Die Benachrichtigungen wurden mit «include» eingebunden.
- Der Anmeldedienst war nur mit einer Notiz verbunden.

**Meine Korrektur in `usecase.puml`:** Ich habe den Anmeldedienst mit den Anwendungsfällen Buchen, Stornieren, Anlegen und Absagen verbunden, damit seine Beteiligung deutlicher dargestellt wird.

## Aufgabe 2 — Aktivitätsdiagramm

- Der Agent hat das Aktivitätsdiagramm zunächst in Mermaid statt in PlantUML erstellt.
- Ich habe den Agenten aufgefordert, das Diagramm in PlantUML mit den beiden Aktivitätsbereichen Studentin und Terminplaner zu erstellen.
- Die drei parallelen Aktionen wurden mit fork und end fork dargestellt.
- Die erneute Auswahl eines Zeitfensters wurde als Schleife dargestellt.

**Die Änderung um die Warteliste:** Der Agent hat die Warteliste an der richtigen Stelle ergänzt. Wenn kein Zeitfenster mehr frei ist, wird der Studentin die Warteliste angeboten. Bei Annahme wird sie auf die Warteliste gesetzt. Bei Ablehnung endet der Ablauf. Der bisherige Buchungsablauf bleibt unverändert.


## Aufgabe 3 — Klassendiagramm

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| Künstliche Schlüssel | 0 | 0 |
| Technische Datentypen | 12 | 0 |
| Erfundenes Attribut, Klasse oder Operation | 0 | 0 |
| Falsche oder fehlende Multiplizitäten | 1 | 1 |
| Fehlende Komposition | 0 | 0 |

**Was die Regeln behoben haben und was nicht:** Durch die Regeln wurden alle technischen Datentypen durch fachliche Datentypen ersetzt. Die falsche Multiplizität zwischen Sekretariat und Lehrperson wurde jedoch nicht korrigiert. Der Agent hat die Regel zu den korrekten Multiplizitäten nicht vollständig umgesetzt. Die übrigen Regeln wurden eingehalten.

### Meine Regeln für Datenmodelle

- Verwende nur fachliche Schlüssel, die in der Beschreibung genannt werden.
- Verwende fachliche Datentypen wie Kennung, Name, Datum, Uhrzeit und Raum.
- Modelliere ausschließlich die genannten Klassen und Attribute ohne Operationen.
- Gib an beiden Enden jeder Assoziation die korrekten Multiplizitäten an.
- Verwende eine Komposition, wenn Teile mit dem Ganzen gelöscht werden.
- Verwende Generalisierung für gemeinsame Eigenschaften von Ober- und Unterklassen.

## Aufgabe 4 — Zustandsdiagramm

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| Fehlende Endknoten bei abgesagt, wahrgenommen und verfallen | nicht berechtigt | Die Zustände besitzen keine ausgehenden Übergänge und können sich somit nicht mehr ändern, wie in der Beschreibung gefordert. |

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
