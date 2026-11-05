# Phasenplan — Terminplaner für die THM

GitHub-Benutzername: hjle99

## Studie

**Ergebnis der Phase:** Problemdarstellung beschreiben, analysieren und auswerten

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Systemspezifikation

**Ergebnis der Phase:** Anforderungen der Eigenschaften des Systems sammeln und festlegen

- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen

## Systemkonstruktion

**Ergebnis der Phase:** Planung der Architektur und technischem Aufbau

- Datenbank, Programmiersprache und Web-Framework auswählen
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Implementierung

**Ergebnis der Phase:** Programmieren des Systems

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Einzelteile zusammenführen, testen und das System in Betrieb nehmen

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen

## Wartung

**Ergebnis der Phase:** Fehler beheben, aktualisieren und weiterentwickeln

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=integration k05=wartung k22=spezifikation k06=spezifikation k07=studie k08=integration k09=konstruktion k10=studie k11=wartung k12=implementierung k23=spezifikation k13=konstruktion k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=konstruktion k24=wartung k20=studie k21=wartung | unsicher: – -->
