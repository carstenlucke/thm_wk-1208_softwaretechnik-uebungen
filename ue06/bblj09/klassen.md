# Klassendiagramm – Daten des Terminplaners

```mermaid
classDiagram
    class Hochschulkonto {
        Kennung kennung
        Name name
    }
    class Lehrperson {
        Titel titel
    }
    class Studierende {
        Studiengang studiengang
    }
    class Sprechstunde {
        Datum datum
        Uhrzeit beginn
        Uhrzeit ende
        Ort ort
    }
    class Zeitfenster
    class Buchung {
        Zeitpunkt buchungszeitpunkt
        Anliegen anliegen
    }
    class Sekretariat {
        Bezeichnung bezeichnung
        Raum raum
    }

    Hochschulkonto <|-- Lehrperson
    Hochschulkonto <|-- Studierende
    Lehrperson "1" -- "0..*" Sprechstunde : bietet an
    Sprechstunde "1" *-- "1..*" Zeitfenster : besteht aus
    Zeitfenster "1" -- "0..1" Buchung : hat
    Studierende "1" -- "0..*" Buchung : tätigt
    Sekretariat "0..1" -- "2..*" Lehrperson : betreut
```

Das Hochschulkonto ist die gemeinsame fachliche Basisklasse der beiden Kontorollen. Die Formulierung „mehrere Lehrende“ wird als mindestens zwei betreute Lehrpersonen gelesen.
