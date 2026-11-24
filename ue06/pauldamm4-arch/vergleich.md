# Von Hand und mit dem Agenten — Terminplaner für die THM

<!-- Aufgaben 1 bis 4 des Übungsblatts und „Vor der nächsten Vorlesung“.
     Ersetzen Sie jedes „…“ durch Ihre Angabe und fügen Sie so viele
     Zeilen hinzu, wie Sie benötigen. Löschen Sie die Kommentare, sobald
     Sie fertig sind. -->

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
