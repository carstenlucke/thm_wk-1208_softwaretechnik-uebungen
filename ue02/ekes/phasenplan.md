# Phasenplan — Terminplaner für die THM

Kürzel: ekes

## Studie

**Ergebnis der Phase:** Bewertung der Möglichkeiten mit Kosten und grobem Plan

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Was das System können muss

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Aufbau des Systems mit Komponenten und Technik

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** Fertige und einzeln getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Abgenommenes System im Einsatz

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Verbesserte Versionen des Systems

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Systemspezifikation): Wer was darf, entscheidet der Kunde, deshalb Spezifikation.
- **Datenbank, Programmiersprache und Web-Framework auswählen** (Systemkonstruktion): Könnte auch in die Studie, wenn es um Kosten geht.
- **Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen** (Wartung): Fängt bei der Einführung an, läuft aber im Betrieb weiter.
- **Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen** (Systemkonstruktion): Endpunkte und Datenformat sind schon das Wie, also Konstruktion.
- **Aufwand schätzen und einen Meilensteinplan vorschlagen** (Studie): Geplant wird eigentlich in jeder Phase, der erste Plan aber in der Studie.
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Systemkonstruktion): Könnte man auch schon in der Studie machen, um zu sehen, ob es geht.
- **Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen** (Wartung): Ist Wartung, aber dafür muss man wieder spezifizieren und programmieren.
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Systemkonstruktion): Ähnlich wie der Meilensteinplan, geht aber erst, wenn die Komponenten feststehen.
- **Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt** (Integration & Einführung): Könnte auch ein früher Test sein, am fertigen System ist es aber Integration.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k22 k09 k11 k23 k13 k15 k17 k18 k24 -->
