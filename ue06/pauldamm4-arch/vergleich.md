# Von Hand und mit dem Agenten — Terminplaner für die THM

## Aufgabe 1 — Use-Case-Diagramm

- Der Agent hat gemacht, dass Studierende einen ICal-Datei machen können aber in der Beschreibung steht, dass jede Buchung sich als iCal-Datei herunterladen lässt.
- Sonst ist es aber relativ genau gleich außer, dass er noch bei Anlegen zu Hochschulkonto anmelden eine <<Include>> gemacht hat

**Meine Korrektur in `usecase.puml`:** …

- Ich habe in Zeile 46 die Richtung geändert der <<extend>> , da es für mich so mehr Sinn gemacht hat

## Aufgabe 2 — Aktivitätsdiagramm

- Der KI-Agent hat es genauso dargestellt, wie es auch bei mir in dem Diagramm war

**Die Änderung um die Warteliste:** …

- Ja der Agent hat nur das geändert, was ich verlangt habe und er hat es auch an die richtige Stelle gesetzt.

## Aufgabe 3 — Klassendiagramm

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | keine | keine |
| technische statt fachlicher Datentypen | Ja - String, Date, Time, DateTime | keine|
| Erfundenes (Attribute, Klassen, Operationen) | keine | keine |
| fehlende oder abweichende Multiplizitäten | Ja - Sekretariat/Lehrende | keine |
| Assoziation statt Komposition | nein – Komposition bei Sprechstunde/Zeitfenster vorhanden | keine |

**Was die Regeln behoben haben und was nicht:** …

### Meine Regeln für Datenmodelle

1. Verwende nur Klassen, Attribute und Beziehungen, die aus der

   Beschreibung hervorgehen.

2. Erfinde keine künstlichen Schlüssel wie `id`, wenn diese nicht in der

   Beschreibung genannt werden.

3. Verwende fachliche Datentypen und keine technischen

   Implementierungsdatentypen wie `String`, `int`, `Date` oder `DateTime`.

4. Verwende keine Operationen, Methoden oder technischen Funktionen,

   sofern diese nicht ausdrücklich in der Beschreibung gefordert werden.

5. Übernimm die Multiplizitäten genau aus der Beschreibung. Begriffe wie

   „beliebig viele“, „mehrere“, „mindestens ein“ und „höchstens einer“

   müssen korrekt in Multiplizitäten umgesetzt werden.

6. Verwende Generalisierung, wenn mehrere Klassen gemeinsame Eigenschaften

   besitzen.

7. Verwende Komposition, wenn ein Teil zu genau einem Ganzen gehört und

   mit diesem Ganzen gelöscht wird.

8. Ergänze keine Informationen, die nicht aus der Beschreibung

   abgeleitet werden können.

## Aufgabe 4 — Zustandsdiagramm

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| `frei` wird durch `state frei { ... }` gleichzeitig als einfacher und zusammengesetzter Zustand verwendet. | berechtigt | `frei` soll ein einfacher Zustand sein. Der innere Block stammt aus der Tür-Vorlage und ist hier nicht notwendig. |
| Der Startknoten innerhalb von `frei` zeigt auf `frei` selbst. | berechtigt | `frei` ist kein Unterzustand seiner eigenen Region. Der innere Startknoten ist daher falsch und außerdem überflüssig. |
| `[mehr als 2h vor Beginn]` schließt genau zwei Stunden vor Beginn aus. | berechtigt | Laut Beschreibung kann bis zwei Stunden vor Beginn storniert werden. Daher muss der Grenzfall von genau zwei Stunden eingeschlossen sein. |
| `Beginn erreicht` ist als Auslöser kein explizites Zeitereignis der UML. | nicht berechtigt | Die Aufgabenstellung verwendet selbst freie Textauslöser in der Vorlage. Außerdem ist `Beginn erreicht` inhaltlich verständlich und passend zur Beschreibung. |

## Ein System, vier Sichten


### Was kommt mehrfach vor?

| Element | Use-Case | Aktivität | Klassen | Zustand |
|---|---|---|---|---|
| Zeitfenster | Use-Case | Aktion/Objekt „Zeitfenster“ | Klasse | Zustand/Objekt |
| Studierende | Akteur | Bahn „Studentin“ | Klasse „Studierende“ | — |
| Lehrende | Akteur | — | Klasse „Lehrende“ | — |
| Sprechstunde | Use-Case „Sprechstunde anlegen/absagen“ | Aktion „Sprechstunde auswählen“ | Klasse „Sprechstunde“ | — |
| Buchung | Use-Case „Zeitfenster buchen/stornieren“ | Aktionen rund um die Buchung | Klasse „Buchung“ | Zustand „gebucht“ |

### Wo passt es nicht zusammen?

- Im Use-Case-Diagramm heißt es „Zeitfenster buchen“, im Aktivitätsdiagramm geht es ebenfalls um das Buchen eines Zeitfensters – das passt zusammen.
- Im Use-Case-Diagramm gibt es „Sprechstunde“, und im Aktivitätsdiagramm wird eine Sprechstunde ausgewählt – das passt zusammen.
- Das Klassendiagramm enthält die Klasse `Buchung`, während das Zustandsdiagramm den Zustand `gebucht` verwendet. Das beschreibt unterschiedliche Dinge und ist daher kein Widerspruch.
- Das Zustandsdiagramm enthält die Zustände `gesperrt`, `abgesagt`, `wahrgenommen` und `verfallen`. Für diese Zustände gibt es im Klassendiagramm keine eigenen Klassen. Das ist kein Widerspruch, weil Zustände eines Zeitfensters keine eigenen Klassen sein müssen.

### Aus „Zeitfenster“ wird „Termin“

**Stellen:** 14 Stellen in 4 Dateien
- `usecase.puml`: 3 Stellen
- `aktivitaet.puml`: 5 Stellen
- `klassen.md`: 3 Stellen
- `zustand.md`: 3 Stellen
