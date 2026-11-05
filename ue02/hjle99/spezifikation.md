# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @hjle99

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## ersten Denkanstöße 

- Was muss das Entwicklerteam über die Benutzer wissen?

- Aus welchem Fachbereich/Branche wird der Terminplaner entwickelt

- Anforderungen, Bedingungen

- Welche Zielgruppen werden bei dem Terminplaner gefragt?

- Wie hoch ist das Budget?

- Welche Systeme können gekauft/genutzt werden?

- Welche Funktionen soll der Terminplaner anbieten?

- Gibt es konkrete Unterfunktionen?

- Soll der Terminplaner auch mit anderen System interagieren?

- Welche Regeln gelten für die Terminbuchung?

- Welche Daten müssen gespeichert werden?

- Welche externen Systeme müssen berücksichtigt werden?

- Sollen die Termine automatisch von anderen Systemen eingebucht werden?

- Filter für z.B nach Veranstaltungen?

- Automatische Buchungen?


## Thematische Zusammenführung und Gliederung
1. Benutzer und Zielgruppen
Fragen: Welche Zielgruppen werden bei dem Terminplaner gefragt?

Beispiel:
- Student: Können freie Termine einsehen und Termine bei Professoren buchen.
- Professor: Können eigene Sprechzeiten festlegen, Buchungen verwalten und Termine absagen 
- Verwalter: Können Benutzer verwalten und bei organisatorischen Problemen unterstützen.


2. Funktionen des Terminplaners
Fragen: Welche Funktionen soll der Terminplaner anbieten und gibt es konkrete Unterfunktionen?

Beispiel:
- Buchung eines Termins:	Studierende können einen freien Termin bei einem Professor auswählen und buchen.
- Terminverwaltung:Professoren können Termine erstellen, bearbeiten und löschen.
- Emailversendung: Nach einer Buchung erhalten beide Parteien eine Bestätigung per E-Mail.
- Kalenderansicht: Freie und bereits belegte Termine werden übersichtlich dargestellt.

3. Anforderungen und Buchungsregeln:
Fragen: Welche Regeln gelten für die Terminbuchung und sollen diese automatisch erfolgen?

Beispiel:
- Abfrage von vertraulichen Informationen: Name, Hochschul-E-Mail-Adresse und Gesprächsgrund.
- bereits existierende Terminbuchungen: Ein bereits gebuchter Zeitraum kann nicht erneut gebucht werden.
- Stornierung: Eine Absage ist bis 24 Stunden vor dem Termin möglich.

4. Daten
Fragen: Welche Daten müssen gespeichert werden?

Beispiel:
- Studierendendaten: Name, Matrikelnummer, Hochschul-E-Mail-Adresse
- Professorendaten: Name, Fachbereich, E-Mail-Adresse
- Termindaten: Datum, Uhrzeit, Dauer und Ort
- Buchungsdaten: Buchungsnummer, Buchungszeitpunkt und Status

5. Schnittstellen und externe Systeme:
Fragen: Welche externen Systeme müssen berücksichtigt werden und soll der Terminplaner mit anderen Systemen interagieren?

Beispiel:
- iCal: Gebuchte Termine können in externe Kalender übernommen werden.
-  API für KI-Agenten: Externe Anwendungen können freie Termine abfragen oder Buchungen verwalten, sofern sie dazu berechtigt sind.
- Outlook: Termine werden mit dem Outlook-Kalender synchronisiert.

6. Rahmenbedingungen:
Fragen: Wie hoch ist das Budget und welche Systeme können gekauft/genutzt werden?

Beispiel:
- bereits existierende Systeme: Die Hochschule nutzt bereits Microsoft 365 und Outlook.
- Allgemeines Budget: Für die Einführung steht ein begrenztes Projektbudget zur Verfügung.
- Datenschutz: Die Anforderungen der DSGVO müssen erfüllt werden.
- Wartung: Updates und technische Betreuung sollen durch die Hochschul-IT erfolgen.