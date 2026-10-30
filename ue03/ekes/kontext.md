# Stakeholder und Systemkontext — Terminplaner für die THM

## Stakeholder

| Stakeholder | Worauf hat er Einfluss? |
|---|---|
| Studierende | Wie einfach sich Sprechstunden und Prüfungstermine finden und buchen lassen. |
| Lehrende | Wie sie Sprechstunden und Prüfungstermine anbieten, ändern und absagen. |
| Sekretariate der Fachbereiche | Welche Übersicht über Prüfungstermine sie brauchen, um die Prüfungen ihres Fachbereichs zu organisieren. |
| Hochschulleitung der THM (Auftraggeberin) | Auf Umfang, Budget und Zeitpunkt der Einführung. |
| Rechenzentrum der THM | Auf Betrieb, Anmeldung über das Hochschulkonto und die Anbindung an vorhandene Systeme. |
| Datenschutzbeauftragte der THM | Welche personenbezogenen Daten gespeichert, wem gezeigt und wann gelöscht werden. |
| Personalrat | Ob und wie sich aus den Daten die Arbeit der Lehrenden auswerten lässt. |
| Beauftragte für Studierende mit Behinderung | Dass sich der Terminplaner barrierefrei bedienen lässt. |
| Gesetzgeber (EU-DSGVO, Hessisches Datenschutzgesetz) | Welche Regeln für die Verarbeitung personenbezogener Daten gelten. |

## Systemkontext

| Aspekt | Art | Warum gehört er zum Kontext? |
|---|---|---|
| Studierende, Lehrende und Sekretariate als Nutzer | Person | Sie bedienen den Terminplaner, sind aber nicht Teil von ihm. |
| Hochschulkonto (Anmeldedienst der THM) | System im Betrieb | Der Terminplaner muss die Anmeldung darüber abwickeln, betreibt den Dienst aber nicht selbst. |
| Kalenderprogramme der Beteiligten (z.B. Outlook, Apple Kalender) | System im Betrieb | Sie müssen die iCal-Dateien des Terminplaners einlesen können, gehören aber den Nutzern. |
| KI-Agenten, die über die API zugreifen | System im Betrieb | Sie fragen Termine ab und buchen im Namen von Personen, sind aber fremde Systeme. |
| E-Mail-System der THM | System im Betrieb | Darüber erfahren Beteiligte z.B. von abgesagten Terminen, es ist aber ein eigenes System. |
| Prüfungsanmeldung | Ereignis | In diesem Zeitraum buchen sehr viele Studierende zugleich, darauf muss der Terminplaner ausgelegt sein. |
| Organisation der Prüfungen im Fachbereich | Prozess | Der Terminplaner unterstützt diesen Ablauf, der Ablauf selbst liegt aber beim Fachbereich. |
| Prüfungsordnungen und Datenschutzvorgaben der THM | Dokument | Sie legen Regeln fest, an die sich der Terminplaner halten muss, ohne dass er sie ändern kann. |

## Irrelevante Umgebung

- Der Speiseplan der Mensa — er hat mit dem Vereinbaren von Terminen nichts zu tun.
- Die Ausleihe in der Bibliothek — sie hat eigene Fristen und ein eigenes System, mit dem der Terminplaner nichts austauschen muss.
