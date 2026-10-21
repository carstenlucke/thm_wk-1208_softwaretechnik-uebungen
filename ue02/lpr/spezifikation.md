# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen): @Yosefhub

## 1. Ziel und Abgrenzung

Der Terminplaner unterstützt die Vereinbarung von Sprechstunden und Prüfungsterminen an der THM. In der ersten Ausbaustufe können Beteiligte Termine als iCal-Datei herunterladen; eine direkte Kalenderintegration ist für eine spätere Ausbaustufe vorgesehen.

## 2. Beteiligte und Berechtigungen

Lehrende bieten Termine an, Studierende buchen sie, Sekretariate behalten den Überblick. Die Anmeldung erfolgt über das Hochschulkonto; die Ansicht und Aktionen richten sich nach der jeweiligen Rolle.

## 3. Anwendungsfälle

Eine studierende Person meldet sich an, sucht einen verfügbaren Sprechstundentermin und bucht ihn. Eine Lehrperson legt zuvor Zeitfenster fest; das Sekretariat kann den Terminbestand für den Fachbereich überblicken.

## 4. Funktionale Anforderungen und Regeln

Ein Terminangebot enthält mindestens Terminart, Zeit und anbietende Lehrperson; eine Buchung verbindet eine studierende Person mit einem verfügbaren Termin. Ein KI-Agent darf über die API freie Termine abfragen und Sprechstunden buchen, aber keine Prüfungstermine absagen.

## 5. Daten und Beziehungen

Beispielhafte Beziehungen: Eine Lehrperson bietet mehrere Termine an; ein Termin kann einer oder mehreren Buchungen zugeordnet werden, abhängig von der noch festzulegenden Kapazität. Räume und Personen werden mit Terminen verknüpft, damit Sekretariate die Planung nachvollziehen können.

## 6. Schnittstellen

Die erste Ausbaustufe stellt einen Termin als iCal-Datei zum Herunterladen bereit. Die API bietet dem KI-Agenten klar begrenzte Aktionen zum Abfragen freier Termine und Buchen einer Sprechstunde; direkte Kalender-Synchronisierung bleibt zunächst außerhalb des Umfangs.

## 7. Qualität, Datenschutz und Betrieb

Das System muss die Anmeldung über das Hochschulkonto nutzen und Buchungsdaten nur den jeweils berechtigten Rollen zeigen. Die THM installiert das System in ihrer eigenen Umgebung und prüft es dort; konkrete Verfügbarkeits- und Leistungswerte sind mit der THM noch festzulegen.

## 8. Abnahme und Prüffälle

Beispiel: Ist eine Sprechstunde frei und eine studierende Person angemeldet, kann sie den Termin buchen und erhält eine Bestätigung; anschließend lässt sich der Termin als iCal-Datei herunterladen. Zusätzlich wird geprüft, dass ein KI-Agent keine Prüfungstermine absagen kann.
