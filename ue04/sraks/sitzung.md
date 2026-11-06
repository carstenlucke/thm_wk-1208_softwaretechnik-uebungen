# Sitzung — Repository untersuchen

| Angabe | Wert |
|---|---|
| Datum | 06.11.2026 |
| Werkzeug | opencode |
| Modell | DeepSeek V4.1 Flash Free |
| Branch | `ue04-sraks` |
| Arbeitsverzeichnis | `C:\Users\<benutzername>\thm_wk-1208_softwaretechnik-uebungen` |

## Auftrag

> Untersuche dieses Repository. Erkläre mir kurz die Ordnerstruktur, den
> Zweck des Projekts und welche Programmiersprachen und Technologien
> verwendet werden. Nimm zunächst keine Änderungen an Dateien vor.

## Antwort des Agenten

Das Repository ist das Übungsrepository der Veranstaltung Softwaretechnik
(THM, Campus Friedberg, Fachbereich MND). Es enthält keine Anwendung und
keinen Quellcode, sondern die von Studierenden eingereichten
Übungsartefakte. Der Ablauf ist wie in einem Softwareprojekt: eigener Fork,
Branch, Commits, Push, Pull Request.

Aufbau:

- `README.md` — zentrale Anleitung: Aufbau, Einreichungsweg, Spielregeln
- `AGENTS.md` — zusammengefasste Regeln für KI-Agenten
- `ue01/` — Git und GitHub; Steckbriefe unter `steckbriefe/<benutzername>.md`
- `ue02/` — Projektmodell am Fall „Terminplaner für die THM“; je Person
  `notiz.md`, `phasenplan.md`, `spezifikation.md`, freiwillig `rollen.md`
- `ue03/` — Anforderungen an den Terminplaner; je Person `kontext.md`,
  `zuordnung.md`, `anforderungen.md`
- `ue04/` — Coding Agent einrichten; je Person `einrichtung.md` und
  `sitzung.md`

Jede Übung hat ein eigenes Verzeichnis mit eigener `README.md`. Pro Person
gibt es ein Verzeichnis, benannt nach dem GitHub-Benutzernamen in
Kleinbuchstaben. Dateien und Ordner, die mit `_` beginnen, sind Vorlagen und
bleiben unverändert. Zum Zeitpunkt der Untersuchung enthält das Repository
782 Dateien, alle im Markdown-Format (`ue01`: 152, `ue02`: 339, `ue03`: 287,
`ue04`: 2).

Sprachen und Technologien:

- Keine Programmiersprache im Sinne von Quellcode; alle Dateien sind
  Markdown (`.md`).
- Markdown als Arbeitsmittel: Inhalte, Tabellen, Kommentare
  (`<!-- -->`), GitHub-Hinweise (`> [!IMPORTANT]`).
- Git und GitHub als Werkzeuge und Prozess: Branches, Commits, Forks,
  Pull Requests; Branch-Namen nach dem Muster `ueNN-<benutzername>`.
- Coding Agents als Inhalt von Übung 4; opencode wird im Übungsblatt
  beschrieben, andere Agenten sind erlaubt.
- Keine Build-Werkzeuge, Paketmanager, CI-Konfiguration oder Testframeworks.

Bei dieser Untersuchung hat der Agent keine Dateien geändert.

## Vom Agenten ausgeführte Befehle

```console
$ git branch --show-current
ue04-sraks

$ git log --oneline -10
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
...

$ Get-ChildItem -Recurse -File -Force
# Auflistung aller 782 Markdown-Dateien

$ Get-ChildItem -Recurse -File -Force | Group-Object Extension
Count Name
  782 .md
```

Gelesen wurden unter anderem `README.md`, `AGENTS.md`, die `README.md` der
Übungen 1 bis 4, `ue01/steckbriefe/_vorlage.md`, `ue03/sraks/anforderungen.md`
und `ue04/_vorlage/einrichtung.md`.

## Weiterer Verlauf

### Sitzungsprotokoll anlegen

> **Nutzer:** ue04/sraks/sitzung.md

Der Agent hat dieses Protokoll angelegt. Der lokale Pfad im Kopf ist als
`C:\Users\<benutzername>\…` anonymisiert; Klarnamen, E-Mail-Adressen und
Matrikelnummern kommen nicht vor. Geändert wurde nur diese Datei im eigenen
Verzeichnis auf dem Branch `ue04-sraks`; committet oder gepusht wurde nichts.

### Einrichtung anlegen

> **Nutzer:** Ja, bitte kopiere die Vorlage aus `ue04/_vorlage/einrichtung.md`
> nach `ue04/sraks/einrichtung.md` und fülle sie anhand meiner tatsächlich
> durchgeführten Einrichtung aus. Verwende keine erfundenen Angaben.

Der Agent hat die Vorlage übernommen, die Kommentare entfernt und die Tabelle
mit geprüften Werten gefüllt:

| Angabe | Wert | Beleg |
|---|---|---|
| Läuft der Agent? | ja | Die Sitzung läuft |
| Werkzeug | opencode | Laufende Umgebung |
| Version | v2.2.5 | `opencode --version` |
| Betriebssystem | Windows 11 | `Win32_OperatingSystem` (NT 10.0.26200) |
| Modellzugang | OpenCode (kostenlos) | Provider `opencode`, keine separate Anmeldung |
| Modell | DeepSeek V4.1 Flash Free | Modell-ID `opencode/deepseek-v4.1-flash-free` |

Der Abschnitt „Wenn es nicht läuft“ bleibt leer, weil der Agent läuft.
Anschließend hat der Agent geprüft, dass die Datei vollständig und korrekt
kodiert (UTF-8) vorliegt.

### Modellzugang korrigiert

> **Nutzer:** Bitte korrigiere den Modellzugang. Ich habe mich nicht separat
> bei OpenCode Zen angemeldet, sondern den kostenlosen Anbieter OpenCode mit
> dem Modell DeepSeek V4.1 Flash Free verwendet.

Der Agent hat in der Tabelle „Modellzugang“ von „OpenCode Zen (kostenlos)“ auf
„OpenCode (kostenlos)“ geändert. Die übrigen Angaben blieben unverändert.

### Abgabedateien geprüft

> **Nutzer:** Bitte überprüfe, dass folgende Dateien existieren:
> `ue04/sraks/einrichtung.md` und `ue04/sraks/sitzung.md`. Kopiere fehlende
> Dateien aus der Vorlage und ergänze die tatsächlichen Informationen. Bitte
> keine Angaben erfinden und keine anderen Dateien verändern.

Beide Dateien waren vorhanden (`einrichtung.md` 622 Bytes, `sitzung.md`
2943 Bytes), sodass nichts kopiert werden musste. `git status` zeigte nur
`?? ue04/sraks/`; die Dateien sind noch nicht committet. Anschließend wurde
dieses Protokoll um den weiteren Verlauf ergänzt.
