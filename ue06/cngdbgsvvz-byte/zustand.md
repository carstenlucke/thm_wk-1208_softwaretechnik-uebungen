# Zustandsdiagramm – Zeitfenster

```mermaid
stateDiagram-v2
    [*] --> Frei
    Frei --> Gebucht: Buchen
    Gebucht --> Frei: Stornieren [mindestens 2 Stunden vorher]
    Frei --> Gesperrt: Sperren
    Gesperrt --> Frei: Freigeben

    Frei --> Abgesagt: Absagen
    Gebucht --> Abgesagt: Absagen
    Gesperrt --> Abgesagt: Absagen

    Gebucht --> Wahrgenommen: Beginn erreicht
    Frei --> Verfallen: Beginn erreicht
    Gesperrt --> Verfallen: Beginn erreicht

    Abgesagt --> [*]
    Wahrgenommen --> [*]
    Verfallen --> [*]