# Phasenplan — Terminplaner für die THM

Kürzel: cms

## Studie

**Ergebnis der Phase:** Lastenheft

- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt

## Systemspezifikation

**Ergebnis der Phase:** Fachkonzept:Enthält Geschäftprzess, Anwendungsfälle(Use case), Benutzerschnittstelle,Objektmodell, Nachbarsysteme

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Systemkonstruktion

**Ergebnis der Phase:** Die Fachliche Konstrucktion (Anwendungskonstrucktion) und die technische Konstrucktion , dabei soll ein technische Prototyps (wenn es möglich)erstellt werden.

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Die Komponenten des Systems werden programmiert und getestet.

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Integerationstests und Systemstests: Teilesystem auslierfern und weiterhin eine Abnahmetests. Probebetrieb/Einführung

- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Wartung

**Ergebnis der Phase:** Fehlerbeseutigung, Technishce Anpassung an Sorftware, neue erweitere Funktione, Beratung des Fachbereich, Anwender der Betreuungs

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten** (Systemspezifikation): …

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=spezifikation k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=konstruktion k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=spezifikation k14=spezifikation k15=konstruktion k16=integration k17=spezifikation k18=spezifikation k19=studie k24=integration k20=integration k21=spezifikation | unsicher: k02 -->
