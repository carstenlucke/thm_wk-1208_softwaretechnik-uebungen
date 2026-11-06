# Stakeholder und Systemkontext — Terminplaner für die THM

## Stakeholder

- **THM (Auftraggeber):** Entscheidet, was das System können soll und ob es umgesetzt wird.
- **Lehrende:** Bieten die Termine an und bestimmen, wann und wie lange Sprechstunden sind.
- **Studierende:** Buchen die Termine, deshalb muss das Buchen für sie einfach sein.
- **Sekretariate:** Wollen sehen, welche Termine es gibt und wer gebucht hat.
- **IT der THM:** Betreibt das System und das Hochschulkonto, über das der Login läuft.
- **Datenschutzbeauftragte (indirekt):** Bestimmt, welche Daten gespeichert werden dürfen.
- **Entwicklerteam der Hochschule (indirekt):** Muss das System später bauen und braucht dafür eine verständliche Beschreibung.

## Systemkontext

- **Studierende** (Person): Buchen Termine im System und sagen sie wieder ab.
- **Lehrende** (Person): Stellen ihre Termine ins System.
- **Hochschulkonto** (System im Betrieb): Darüber meldet man sich an.
- **Kalender, z. B. Outlook** (System im Betrieb): Da kommen die Termine als iCal-Datei rein.
- **KI-Agenten** (System im Betrieb): Sollen das System über eine API benutzen können.
- **Sprechstunde buchen** (Prozess): Das ist der Hauptablauf, den das System unterstützt.
- **Termin wird abgesagt** (Ereignis): Dann muss der Termin wieder frei werden.
- **iCal-Datei** (Dokument): Wird vom System erstellt und heruntergeladen.

## Irrelevante Umgebung

- **Mensa:** Hat mit Terminen nichts zu tun.
- **Bibliothek (Ausleihe):** Da geht es um Bücher, nicht um Termine.