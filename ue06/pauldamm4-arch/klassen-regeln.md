# Klassendiagramm nach meinen Regeln — Terminplaner der THM

Modell zu Beschreibung 3 in [`fall.md`](../fall.md), entstanden mit den
Regeln aus „Meine Regeln für Datenmodelle“ in
[`vergleich.md`](vergleich.md). Zum Vergleich: die frühere Fassung ohne
Regeln steht in [`klassen.md`](klassen.md).

Angewandte Regeln:

1. Keine künstlichen Schlüssel — keine `id`-Attribute; Personen werden über
   ihre fachliche Kennung identifiziert.
2. Fachliche statt technischer Datentypen — `Kennung`, `Text`, `Datum`,
   `Uhrzeit`, `Zeitpunkt` statt `String`, `Date`, `Time`, `DateTime`.
3. Nichts erfinden — nur Klassen und Attribute, die in Beschreibung 3
   genannt sind; keine Operationen. `Zeitfenster` hat dort keine Attribute,
   die 15-Minuten-Einteilung stammt aus Beschreibung 1.
4. Jedes Assoziationsende trägt eine Multiplizität, gelesen in Richtung des
   Verbs am anderen Ende.
5. Komposition (`*--`), wo die Beschreibung das Mitlöschen nennt — nur bei
   `Sprechstunde` und `Zeitfenster`.

```mermaid
---
title: Klassendiagramm nach meinen Regeln — Terminplaner der THM
---
classDiagram
    class Person {
        -kennung: Kennung
        -name: Text
    }

    class Lehrende {
        -titel: Text
    }

    class Studierende {
        -studiengang: Text
    }

    class Sekretariat {
        -bezeichnung: Text
        -raum: Text
    }

    class Sprechstunde {
        -datum: Datum
        -beginn: Uhrzeit
        -ende: Uhrzeit
        -ort: Text
    }

    class Zeitfenster

    class Buchung {
        -zeitpunkt: Zeitpunkt
        -anliegen: Text
    }

    Person <|-- Lehrende
    Person <|-- Studierende

    Sekretariat "0..1" -- "1..*" Lehrende : betreut
    Lehrende "1" -- "0..*" Sprechstunde : bietet an
    Sprechstunde "1" *-- "1..*" Zeitfenster : besteht aus
    Zeitfenster "1" -- "0..1" Buchung : hat
    Studierende "1" -- "0..*" Buchung : bucht
```
