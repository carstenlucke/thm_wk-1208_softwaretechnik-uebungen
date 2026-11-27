# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @…drwf20

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## Nutzergruppe

| Nutzergruppe | was sie im Terminplaner tut |
|------ |----- |
| Lehrende | bietet Sprechstunde an |
| Studierende | können die sprechstunden buchen |
| Sekretariate | behält einen Überblick über das system |


## Nachbarsysteme
 - KI-Agent über das API : darf Termine abfragen und buchen aber keine Prüfungstermine absagen 

 - Hochschulkonto für die Anmeldung 
 - Kalender, zuerst als iCal-Datei, später vielleicht direkt

## Funktionen 

1. Über dasHochschulkonto anmelden 

2. Angeboten Sprechstunden und Prüfungstermin ansehen und welche frei  sind

3. Einen Termin auswählen und das System prüft,ob es noch frei Platz gibt

4. Wenn ein Platz frei ist, wird der Termin gebucht. Wenn nicht, wird die Studentin informiert, dass die Buchung nicht möglich ist.

5. Den Termin bei Bedarf absagen. Die Sekretariate  sehen, wer welchen Termin abgesagt hat.


## Daten 
| Angaben | Beispiel |
|-----|-----|
|Art bzw. Beschreibung| Sprchstunde oder Prüfung |
| Datum und Uhrzeit| 27.11.2026 um 13:00 |
| die oder der Lehrende | FR oder Herr.....|
| Der Raum | AA4.11.09 |
| Anzahl der Plätze | 40 |

