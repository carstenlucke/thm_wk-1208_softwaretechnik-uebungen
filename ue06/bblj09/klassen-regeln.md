# Regeln für das Datenmodell

- Nur die fachlichen Klassen, Attribute und Beziehungen aus Beschreibung 3 modellieren. Keine Operationen, technischen Klassen oder zusätzlichen Attribute ergänzen.
- Die vorgegebene Hochschulkennung übernehmen. Keine künstlichen Schlüssel oder Fremdschlüssel einführen. Beziehungen als UML-Assoziationen darstellen.
- Fachliche Typen wie Datum, Uhrzeit, Zeitpunkt und Anliegen verwenden. Auf Implementierungstypen wie String oder int verzichten.
- Jede Assoziation an beiden Enden mit einer Multiplizität versehen. „Beliebig viele“ als 0..*, „mindestens eins“ als 1..*, „mehrere“ als 2..* und „höchstens eins“ als 0..1 modellieren.
- Die gemeinsame Kennung und den Namen an der Basisklasse des Hochschulkontos modellieren. Die Rollen ergänzen nur ihre jeweils beschriebenen Attribute.
- Die Zugehörigkeit eines Zeitfensters zur Sprechstunde als Komposition modellieren. Die Sprechstunde ist das Ganze. Das Zeitfenster gehört genau einer Sprechstunde und wird mit ihr gelöscht.
