stateDiagram-v2
    [*] --> frei

    frei --> gebucht : buchen
    gebucht --> frei : stornieren [mindestens 2h vor Beginn]

    frei --> gesperrt : sperren
    gesperrt --> frei : freigeben

    frei --> abgesagt : Sprechstunde absagen
    gebucht --> abgesagt : Sprechstunde absagen
    gesperrt --> abgesagt : Sprechstunde absagen

    gebucht --> wahrgenommen : Beginn erreicht
    frei --> verfallen : Beginn erreicht
    gesperrt --> verfallen : Beginn erreicht

    abgesagt --> [*]
    wahrgenommen --> [*]
    verfallen --> [*]