# Stakeholder und Systemkontext — Terminplaner für die THM


## Stakeholder

| Stakeholder | Worauf hat er Einfluss? |
|---|---|
| Lehrende | Bieten Termine an und legen fest, wie flexibel Zeiten und Sprechstunden einstellbar sein müssen |
| Entwicklerteam | Setzt die Spezifikation um und braucht eindeutige, vollständige Anforderungen | 
| Datenschutzbeauftragte | Legen fest, welche personenbezogene Daten gespeichert werden dürfen und wie lange |
| Hochschulleitung | Beauftragt und finanziert das System und gibt Ziele und Budget vor |
| Sekretariat | Behalten den Überblick über die Planung und brauchen Übersichten über alle Termine |
| IT-Abteilung | Betreibt das System später und bestimmt technische Vorgaben |

## Systemkontext

| Aspekt | Art | Warum gehört er zum Kontext? |
|---|---|---|
| Kalender der Beteiligten | System im Betrieb | Der Terminplaner muss sich darüber bedienen lassen, ist aber nicht Teil davon  |
| KI-Agenten | System im Betrieb | Sie steuern das System über die API, gehören aber nicht dazu |
| Hochschulkonto | System im Betrieb | Der Terminplaner muss sich darüber bedienen lassen, ist aber nicht Teil davon |
| iCal-Datei | Dokument | Das Format ist vorgegeben, das System muss es erzeugen | 
| Prüfungs und Sprechstundenzeiten | Ereignis | Sie bestimmen, wann Termine möglich sind, und stehen nicht unter der Kontrolle des Systems |
| Bisherige Terminvergabe | Prozess | Das System ersetzt diesen Ablauf und muss in ihn übergehen |

## Irrelevante Umgebung

- Bibliothek - Eigenes System ohne Bezug zu den Sprechstunden oder Prüfungen, der Terminplaner muss damit nicht zusammenarbeiten.
- Mensa — Hat keinen Bezug zur Terminvergabe, es werden weder Daten ausgetauscht noch Funktionen gebraucht.
