# Klassendiagramm — Terminplaner der THM

Modell zu Beschreibung 3 in [`fall.md`](../fall.md). Die Multiplizitäten
stehen an den Enden der Assoziationen, die Leserichtung folgt dem jeweiligen
Verb.

```mermaid
---
title: Klassendiagramm — Terminplaner der THM
---
classDiagram
    class Person {
        -kennung: String
        -name: String
    }

    class Lehrende {
        -titel: String
    }

    class Studierende {
        -studiengang: String
    }

    class Sekretariat {
        -bezeichnung: String
        -raum: String
    }

    class Sprechstunde {
        -datum: Date
        -beginn: Time
        -ende: Time
        -ort: String
    }

    class Zeitfenster

    class Buchung {
        -zeitpunkt: DateTime
        -anliegen: String
    }

    Person <|-- Lehrende
    Person <|-- Studierende

    Sekretariat "1" -- "0..*" Lehrende : betreut
    Lehrende "1" -- "0..*" Sprechstunde : bietet an
    Sprechstunde "1" *-- "1..*" Zeitfenster : besteht aus
    Zeitfenster "1" -- "0..1" Buchung : hat
    Studierende "1" -- "0..*" Buchung : bucht
```
