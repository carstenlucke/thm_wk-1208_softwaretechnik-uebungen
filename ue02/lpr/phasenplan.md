# Phasenplan — Terminplaner für die THM

Kürzel: lpr

## Studie

**Ergebnis der Phase:** Bedarfs- und Machbarkeitsstudie mit Ist-Analyse, Bewertung möglicher Lösungen und einem begründeten Projektvorschlag.

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Systemspezifikation

**Ergebnis der Phase:** Abgestimmte, prüfbare Anforderungen: Anwendungsfälle, Regeln, Daten, Schnittstellen und Abnahmekriterien.

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Systemkonstruktion

**Ergebnis der Phase:** Systementwurf mit Komponenten, Schnittstellen, Datenmodell und ausgewählten technischen Grundlagen.

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** Implementierte Komponenten mit Quellcode und bestandenen Komponententests.

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Integriertes Gesamtsystem mit bestandenen System- und Abnahmetests, eingeführt im Fachbereich.

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Im Betrieb gepflegtes System mit Fehlerkorrekturen und vereinbarten Erweiterungen.

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen** (Systemspezifikation): Ich ordne die Skizzen der Systemspezifikation zu, weil sie Anforderungen mit Nutzenden abstimmen; die ausgearbeitete Gestaltung könnte auch zur Systemkonstruktion zählen.
- **Aufwand schätzen und einen Meilensteinplan vorschlagen** (Studie): Das passt zur Studie als Vorschlag für die weitere Arbeit; die Übung grenzt Projektplanung und Schätzung allerdings ausdrücklich aus, daher bleibt die Zuordnung unscharf.
- **Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen** (Systemspezifikation): Ich habe die Kartenangaben zu Terminen als Anforderungen modelliert; die konkrete Datenstruktur kann aber auch Teil der Systemkonstruktion sein.
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Studie): Ich werte den Prototyp als Machbarkeitsprüfung in der Studie; wenn er schon eine Architekturentscheidung absichert, gehört er ebenso zur Systemkonstruktion.
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Systemkonstruktion): Die Reihenfolge kann aus technischen Abhängigkeiten der Systemkonstruktion folgen; Zwischenziele klingen zugleich nach Projektplanung, die hier nicht behandelt wird.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=integration k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k10 k13 k14 k15 k18 -->
