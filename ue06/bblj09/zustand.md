# Zustandsdiagramm – Lebenszyklus eines Zeitfensters

```mermaid
stateDiagram-v2
    state "Wahrgenommen" as Wahrgenommen
    state "Verfallen" as Verfallen
    state "Abgesagt" as Abgesagt

    [*] --> Frei
    Frei --> Gebucht: buchen
    Gebucht --> Frei: stornieren [jetzt ≤ Beginn − 2 Stunden]
    Frei --> Gesperrt: Lehrperson sperrt
    Gesperrt --> Frei: Lehrperson gibt frei

    Frei --> Abgesagt: Sprechstunde absagen
    Gebucht --> Abgesagt: Sprechstunde absagen
    Gesperrt --> Abgesagt: Sprechstunde absagen

    Frei --> Verfallen: Beginn erreicht
    Gesperrt --> Verfallen: Beginn erreicht
    Gebucht --> Wahrgenommen: Beginn erreicht

    Abgesagt --> [*]
    Verfallen --> [*]
    Wahrgenommen --> [*]
```

Die Stornierungsgrenze wird einschließlich des Zeitpunkts genau zwei Stunden vor Beginn verstanden. Die Übergänge zum UML-Endknoten schließen den Lebenszyklus ab.
