# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @erhankesbic

**Zur Reihenfolge:** Die Gliederung geht von außen nach innen. Zuerst
steht, wozu das System da ist und wer es benutzt, dann, was es tun soll,
mit welchen Daten und über welche Wege. Danach folgen die Anforderungen an
das Wie gut und die festen Vorgaben, und am Schluss, woran sich die
Erfüllung prüfen lässt und was noch offen ist. So kann das Entwicklerteam
das Dokument von vorn lesen, ohne auf Begriffe zu stoßen, die erst später
erklärt werden.

## 1 Einleitung

### 1.1 Zweck und Ziele

Der Terminplaner ersetzt Listen an der Bürotür, E-Mail-Absprachen sowie
Doodle und den DFN-Terminplaner. Lehrende bieten darin Sprechstunden und
Prüfungstermine an, Studierende buchen sie, Sekretariate behalten den Überblick.

### 1.2 Abgrenzung

- Gehört dazu: Termine anbieten, buchen, absagen und als iCal-Datei herunterladen.
- Gehört nicht dazu: Termine direkt in fremde Kalender eintragen (frühestens
  in einer späteren Version), Räume buchen, Noten verwalten.

### 1.3 Begriffe

| Begriff | Bedeutung |
|---|---|
| Zeitfenster | Ein buchbarer Abschnitt einer Sprechstunde, z.B. 10:00–10:15 Uhr |
| Buchung | Die Reservierung genau eines Zeitfensters durch genau eine Person |

## 2 Rollen und Berechtigungen

| Rolle | Darf |
|---|---|
| Lehrende | Sprechstunden und Prüfungstermine anlegen, ändern, absagen |
| Studierende | freie Zeitfenster buchen und eigene Buchungen stornieren |
| Sekretariat | alle Termine ihres Fachbereichs sehen und im Auftrag von Lehrenden pflegen |
| KI-Agent | im Namen einer Person handeln, aber nur im Umfang von Abschnitt 6.3 |

## 3 Funktionale Anforderungen

### 3.1 Anwendungsfälle

**Sprechstundentermin buchen** — Akteur: Studierende. Vorbedingung: angemeldet.
Ablauf: Lehrende suchen → freies Zeitfenster wählen → Anliegen in einer Zeile
angeben → bestätigen. Ergebnis: Zeitfenster belegt, Bestätigung mit iCal-Datei.

### 3.2 Geschäftsregeln

- R1: Pro Sprechstunde bucht eine Person höchstens ein Zeitfenster.
- R2: Studierende können bis 2 Stunden vor Beginn selbst stornieren, danach nur noch per Nachricht an die Lehrenden.

### 3.3 Benachrichtigungen

| Ereignis | Wer wird benachrichtigt | Wie |
|---|---|---|
| Lehrende sagen eine Sprechstunde ab | alle, die darin gebucht haben | E-Mail an die Hochschuladresse, spätestens 5 Minuten nach der Absage |

## 4 Daten

### 4.1 Datenmodell

Beschriebene Skizze: Eine *Person* bietet 0..n *Termine* an. Ein Termin
(Sprechstunde oder Prüfung) hat Ort, Beginn, Ende und besteht aus
1..n *Zeitfenstern*; jedes Zeitfenster hat höchstens eine *Buchung* durch eine Person.

### 4.2 Datenschutz und Aufbewahrung

Studierende sehen bei einem Zeitfenster nur „frei“ oder „belegt“, nie den
Namen anderer Studierender. Buchungen werden 6 Monate nach dem Termin gelöscht.

## 5 Benutzungsoberfläche

Beschriebene Skizze der Buchungsseite: oben Name und Raum der Lehrperson,
darunter eine Wochenansicht; freie Zeitfenster sind anklickbar und
hervorgehoben, belegte grau. Ein Klick öffnet ein kleines Formular mit Feld „Anliegen“ und Knopf „Buchen“.

## 6 Schnittstellen zu anderen Systemen

### 6.1 Anmeldung über das Hochschulkonto

Alle Menschen melden sich ausschließlich mit ihrem Hochschulkonto über das
zentrale Anmeldeverfahren der THM an. Der Terminplaner verwaltet keine eigenen Passwörter.

### 6.2 iCal-Export

Zu jeder Buchung und jedem angebotenen Termin gibt es eine iCal-Datei
(RFC 5545) mit mindestens Titel, Beginn, Ende, Ort und Name der Lehrperson.

### 6.3 API für KI-Agenten

| Vorgang | Erlaubt? |
|---|---|
| Freie Zeitfenster abfragen, buchen, eigene Buchung stornieren | ja |
| Prüfungstermine anlegen, verschieben oder absagen | nein, nur durch Menschen |

## 7 Qualitätsanforderungen

- Bedienbarkeit: Eine Buchung gelingt in höchstens 4 Klicks ab der Startseite, auch auf dem Smartphone.
- Last: Zu Semesterbeginn bleiben die Seiten bei 1.000 gleichzeitigen Nutzern unter 2 Sekunden Antwortzeit.
- Barrierefreiheit: Die Oberfläche erfüllt die BITV 2.0.

## 8 Randbedingungen

- Das System läuft auf Servern der THM, die THM installiert und betreibt es selbst.
- Oberfläche auf Deutsch und Englisch; Datenverarbeitung nach DSGVO.

## 9 Abnahmekriterien

| Nr. | Ausgangslage | Aktion | Erwartetes Ergebnis |
|---|---|---|---|
| T1 | Zeitfenster 10:00 ist frei | Zwei Studierende buchen es fast gleichzeitig | Genau eine Buchung gelingt, die andere Person erhält „bereits belegt“ |
| T2 | Ein KI-Agent ist für eine Lehrperson angemeldet | Er versucht, eine Prüfung abzusagen | Abgelehnt, Prüfung bleibt bestehen |

## 10 Offene Punkte

| Punkt | Wer klärt | Bis wann |
|---|---|---|
| Bis wann soll der Terminplaner eingeführt sein? | Die THM | Vor Beginn der Konstruktion |
