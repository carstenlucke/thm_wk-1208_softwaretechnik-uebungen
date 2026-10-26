---
title: Spezifikation Terminplaner (Gliederung mit Beispielen)
mitwirkende:
  - DEIN-GITHUB-BENUTZERNAME
---

# Spezifikation Terminplaner

> **Begründung der Reihenfolge:** Vom Groben zum Feinen. Zuerst Zweck, Begriffe und Ziele, damit das Entwicklerteam den Kontext versteht. Dann *was* das System tun soll (Rollen, Funktionen, Daten, Oberfläche, Schnittstellen), danach *wie gut* und *unter welchen Bedingungen* (Qualität, Randbedingungen). Zum Schluss, woran man erkennt, dass es fertig ist (Abnahme), und was noch offen ist.

## 1 Einleitung

### 1.1 Zweck des Dokuments
Dieses Dokument beschreibt vollständig, was der Terminplaner leisten soll. Es ist die einzige Grundlage für Konstruktion und Implementierung durch das Entwicklerteam der THM.

### 1.2 Begriffe (Glossar)
| Begriff | Bedeutung |
|---|---|
| Termin | Zeitraum mit Beginn, Ende, Ort und Teilnehmenden |
| Terminumfrage | Mehrere Terminvorschläge, über die Teilnehmende abstimmen |
| Slot | Buchbarer Zeitabschnitt, z.B. 15 min einer Sprechstunde |

### 1.3 Referenzen
- Gesprächsprotokolle mit der THM vom [Datum]
- DSGVO, Barrierefreiheitsrichtlinien der THM

## 2 Ausgangslage und Ziele

### 2.1 Ist-Zustand
Termine werden derzeit per E-Mail und externen Umfragetools abgestimmt; Sprechstunden werden über Listen an der Bürotür vergeben.

### 2.2 Ziele
- Z1: Ein Termin mit bis zu 30 Personen lässt sich in unter 5 Minuten abstimmen.
- Z2: Keine personenbezogenen Daten landen bei externen Anbietern.

### 2.3 Abgrenzung (nicht Bestandteil)
- Raumbuchung und Stundenplanung sind **nicht** Teil des Systems.
- Keine App für Smartphones, nur Web (responsiv).

## 3 Nutzerrollen und Nutzungskontext

### 3.1 Rollen
| Rolle | Darf |
|---|---|
| Studierende | Slots buchen, an Umfragen teilnehmen |
| Lehrende | Sprechstunden und Umfragen anlegen, Teilnehmende einladen |
| Administration | Nutzer sperren, Einstellungen verwalten |

### 3.2 Nutzungskontext
Lehrende nutzen das System meist am Arbeitsplatz-PC, Studierende überwiegend am Smartphone zwischen Veranstaltungen.

## 4 Funktionale Anforderungen

### 4.1 Anwendungsfälle
**UC-03 Sprechstundenslot buchen**
Akteur: Studierende. Vorbedingung: angemeldet. Ablauf: Sprechstunde wählen → freien Slot wählen → Anliegen eingeben → bestätigen. Ergebnis: Slot ist belegt, beide Seiten erhalten eine E-Mail.

### 4.2 Einzelanforderungen
- **F-07** (Muss): Das System muss eine Buchung bis 24 h vor Beginn stornierbar machen.
- **F-08** (Kann): Das System kann eine Erinnerung 1 h vor dem Termin senden.

### 4.3 Geschäftsregeln
- R1: Pro Sprechstunde darf eine Person höchstens einen Slot belegen.
- R2: Eine Umfrage schließt automatisch zum festgelegten Stichtag.

## 5 Fachliches Datenmodell
Beschriebene Skizze: *Lehrende* (1) bietet an (n) *Sprechstunde*; *Sprechstunde* (1) besteht aus (n) *Slot*; *Slot* (0..1) gebucht von *Studierende*.

| Attribut Slot | Typ | Pflicht |
|---|---|---|
| beginn | Datum + Uhrzeit | ja |
| dauer | Minuten (5–60) | ja |
| anliegen | Text, max. 500 Zeichen | nein |

## 6 Benutzungsschnittstelle

### 6.1 Masken
Beschriebene Skizze „Sprechstunde buchen“: oben Name der Lehrperson und Datum, darunter Liste der Slots (frei = grün, belegt = grau), rechts Feld „Anliegen“, unten Button „Verbindlich buchen“.

### 6.2 Dialogfluss
Startseite → Sprechstunde suchen → Slot wählen → Bestätigungsseite → zurück zur Startseite.

## 7 Externe Schnittstellen
| System | Zweck | Art |
|---|---|---|
| THM-Login (CAS/LDAP) | Anmeldung | Single Sign-on |
| E-Mail-Server der THM | Benachrichtigungen | SMTP |
| Kalender (Outlook etc.) | Termin übernehmen | ICS-Export |

## 8 Nichtfunktionale Anforderungen

### 8.1 Leistung
Seiten laden bei 200 gleichzeitigen Nutzern in unter 2 s.

### 8.2 Benutzbarkeit und Barrierefreiheit
Bedienbar ohne Maus; Konformität mit WCAG 2.1 Stufe AA.

### 8.3 Datenschutz und Sicherheit
Speicherung nur auf Servern der THM; Umfragedaten werden 6 Monate nach Ablauf gelöscht; Zugriff nur über HTTPS.

### 8.4 Verfügbarkeit
99 % im Semester zwischen 7 und 22 Uhr; Wartung nur außerhalb dieser Zeit.

## 9 Randbedingungen
- Betrieb im Rechenzentrum der THM (Linux-Server, Docker)
- Oberfläche auf Deutsch und Englisch
- Unterstützte Browser: aktuelle Versionen von Firefox, Chrome, Safari, Edge

## 10 Fehler- und Sonderfälle
| Situation | Verhalten |
|---|---|
| Zwei Personen buchen gleichzeitig denselben Slot | Nur die erste Buchung gilt, die zweite Person erhält „Slot inzwischen vergeben“ |
| Lehrende sagt Sprechstunde ab | Alle Gebuchten werden per E-Mail informiert |

## 11 Abnahmekriterien
**AK zu F-07:** *Gegeben* eine Buchung für morgen 14:00, *wenn* die Person heute um 13:59 storniert, *dann* ist der Slot wieder frei. Um 14:01 wird die Stornierung abgelehnt.

## 12 Priorisierung
| Priorität | Anforderungen |
|---|---|
| Muss (Version 1) | F-01 bis F-07 |
| Soll | F-08, ICS-Export |
| Kann | Mehrsprachigkeit über DE/EN hinaus |

## 13 Offene Punkte und Änderungshistorie
| Nr. | Offene Frage | Verantwortlich |
|---|---|---|
| O1 | Sollen auch Externe ohne THM-Konto teilnehmen dürfen? | THM, Prof. X |

| Version | Datum | Änderung |
|---|---|---|
| 0.1 | 26.10.2026 | Gliederung mit Beispielen |
