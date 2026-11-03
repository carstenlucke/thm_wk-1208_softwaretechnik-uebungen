# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e5ea034c2ffedi22Ok37HhJHGT
**Created:** 3.11.2026, 13:26:12
**Updated:** 3.11.2026, 13:26:34

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

Let me explore the repository.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current; git status --short; git remote -v"
}
```

ue04-DLM28
 M ue03/dlm28/zuordnung.md
?? ue04/DLM28/
origin	https://github.com/DLM28/thm_wk-1208_softwaretechnik-uebungen.git (fetch)
origin	https://github.com/DLM28/thm_wk-1208_softwaretechnik-uebungen.git (push)
upstream	https://github.com/carstenlucke/thm_wk-1208_softwaretechnik-uebungen (fetch)
upstream	https://github.com/carstenlucke/thm_wk-1208_softwaretechnik-uebungen (push)


**Tool: read**

**Input:**
```json
{
  "path": "README.md"
}
```

Read file README.md, lines 1-74
1: # Softwaretechnik — Übungsrepository
2: 
3: Dieses Repository gehört zu den Übungen der Veranstaltung **Softwaretechnik**
4: (THM, Campus Friedberg, Fachbereich MND). Hier reichen Sie ein, was in den
5: Übungen entsteht — auf dem Weg, auf dem in Softwareprojekten gearbeitet wird:
6: über einen eigenen Fork, einen Branch und einen Pull Request.
7: 
8: ## Aufbau
9: 
10: Jede Übung hat ein eigenes Verzeichnis mit einer eigenen `README.md`, die
11: sagt, was dort einzureichen ist.
12: 
13: | Verzeichnis | Übung |
14: |---|---|
15: | [`ue01/`](ue01/) | Erste Schritte mit Git und GitHub |
16: | [`ue02/`](ue02/) | Das Projektmodell am Fall |
17: | [`ue03/`](ue03/) | Anforderungen an den Terminplaner |
18: | [`ue04/`](ue04/) | Einen Coding Agent einrichten |
19: 
20: ## So reichen Sie etwas ein
21: 
22: 1. Legen Sie einmalig einen **Fork** dieses Repositorys an und **klonen** Sie
23:    ihn auf Ihren Rechner.
24: 2. Legen Sie für jedes Vorhaben einen eigenen **Branch** an.
25: 3. Halten Sie Ihre Änderungen als **Commits** fest und übertragen Sie sie per
26:    **Push** in Ihren Fork.
27: 4. Stellen Sie einen **Pull Request** an dieses Repository.
28: 
29: Den Weg Schritt für Schritt beschreibt das
30: [Übungsblatt zur Übung 1](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/).
31: 
32: ## Vor jeder weiteren Übung
33: 
34: Dieses Repository wächst mit jeder Übung. Bringen Sie vorher Ihren Fork und
35: Ihren Rechner auf den neuen Stand:
36: 
37: 1. Klicken Sie auf der Startseite Ihres Forks auf **Sync fork → Update
38:    branch**.
39: 2. Holen Sie den neuen Stand aus dem Fork auf Ihren Rechner:
40: 
41:    ```console
42:    $ git switch main
43:    $ git pull
44:    ```
45: 
46: Den Branch für die neue Übung zweigen Sie erst danach ab.
47: 
48: ## Spielregeln
49: 
50: - **Ihr GitHub-Benutzername als Kennung.** Ihre Datei- und Verzeichnisnamen
51:   sowie Ihre Branches tragen Ihren GitHub-Benutzernamen, und zwar in
52:   Kleinbuchstaben: Aus `MMustermann` wird `mmustermann`. Anders als ein
53:   selbst gewähltes Kürzel ist er eindeutig, und er steht ohnehin an jedem
54:   Pull Request. Ihren Benutzernamen sehen Sie auf GitHub, wenn Sie oben
55:   rechts auf Ihr Profilbild klicken.
56: - **Öffentlich ist mehr als der Benutzername.** In jedem Commit stehen Name
57:   und E-Mail-Adresse aus Ihrer Git-Einrichtung. Wie Sie Ihre Adresse
58:   verbergen, steht in
59:   [Aufgabe 0 des Übungsblatts](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/#aufgabe-0--einrichten).
60:   Schreiben Sie auch in Ihre Dateien nichts, was nicht jeder lesen darf —
61:   keine Matrikelnummer, keine Anschrift.
62: - **Nur eigene Dateien.** Sie ändern ausschließlich, was Sie selbst angelegt
63:   haben; Vorlagen und die Dateien anderer bleiben unberührt. So kommen sich
64:   die Pull Requests nicht in die Quere.
65: - **Nicht auf `main` arbeiten.** `main` Ihres Forks folgt allein dem Stand
66:   dieses Repositorys; nur so lässt er sich später abgleichen.
67: - **Ein Anliegen je Pull Request**, mit einem Titel, der sagt, was sich
68:   ändert.
69: - **Aussagekräftige Commit-Nachrichten**, etwa `Steckbrief für mmustermann anlegen`.
70: 
71: Arbeiten Sie mit einem KI-Agenten, gelten die Spielregeln auch für ihn. Die
72: Datei [`AGENTS.md`](AGENTS.md) fasst sie für Agenten zusammen; opencode und
73: andere Coding Agents lesen sie, wenn sie in diesem Repository gestartet
74: werden.

---

## Assistant

_Thinking:_

The user's GitHub username appears to be DLM28 (branch ue04-DLM28, directory ue03/dlm28, ue04/DLM28). Let's list repo contents and their files.

**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files | Select-String -Pattern \"(?i)dlm28\"; git log --oneline -10; git log --format=\"%h %s\" --author=DLM28 -10 2>$null"
}
```


ue01/steckbriefe/dlm28.md
ue02/dlm28/notiz.md
ue02/dlm28/phasenplan.md
ue02/dlm28/spezifikation.md
ue03/dlm28/anforderungen.md
ue03/dlm28/kontext.md
ue03/dlm28/zuordnung.md
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)
8cfd580 Übung 2: Formatierung der Gesprächsnotiz korrigiert (#286)
baaa2b8 Ergebnisse der Phasen ergänzt in phasenplan.md (#284)
c55409f Übung 2 : Ergebnisse von akyf (#283)
9db8067 Ue02 zsh (#281)
724bbb5 Übung 2: Ergebnisse von nohl (#280)
f471c58 Übung 3: Ergebnisse von dlm28 (#369)
f467e7f Übung 2: Ergebnisse von DLM28 (#211)
109cd6f Steckbrief dlm28 (#90)




**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Force | Select-Object Mode,Name; git ls-files | ForEach-Object { ($_ -split '/')[0] } | Group-Object | Select-Object Name,Count"
}
```


Mode   Name     
----   ----     
d--h-- .git     
d----- ue01     
d----- ue02     
d----- ue03     
d----- ue04     
-a---- AGENTS.md
-a---- README.md
       AGENTS.md
       README.md
       ue01     
       ue02     
       ue03     
       ue04     




---

## Assistant

_Thinking:_

Interesting: ue04/DLM28/ is untracked. The convention says lowercase dlm28. Let me inspect ue04 contents and the untracked directory, plus ue04 README to know what was expected.

Also the modified ue03/dlm28/zuordnung.md. Let me view diff.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Recurse -Force ue04 | Select-Object FullName; git diff -- ue03/dlm28/zuordnung.md"
}
```


warning: in the working copy of 'ue03/dlm28/zuordnung.md', LF will be replaced by CRLF the next time Git touches it
diff --git a/ue03/dlm28/zuordnung.md b/ue03/dlm28/zuordnung.md
index 5c05e75..896f769 100644
--- a/ue03/dlm28/zuordnung.md
+++ b/ue03/dlm28/zuordnung.md
 -1,4 +1,4 
-# Anforderung oder Lösung? — Terminplaner für die THM
+g# Anforderung oder Lösung? — Terminplaner für die THM
 
 Kürzel: DLM28
 
FullName                                                                                                               
--------                                                                                                               
C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\DLM28        
C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage     
C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\README.md    
C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\DLM28\einr...
C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage\e...




**Tool: read**

**Input:**
```json
{
  "path": "ue04/README.md"
}
```

Read file ue04/README.md, lines 1-40
1: # Übung 4 — Einen Coding Agent einrichten
2: 
3: In dieser Übung installieren Sie einen Coding Agent — das Übungsblatt
4: beschreibt opencode —, verbinden ihn mit einem Sprachmodell und setzen ihn
5: zum ersten Mal in Ihrem lokalen Klon dieses Repositorys ein. Die Aufgaben stehen im
6: [Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue04-coding-agent/).
7: 
8: ## Was Sie einreichen
9: 
10: Einzureichen ist ein Verzeichnis `ue04/<benutzername>/` mit zwei Dateien,
11: und zwar als Pull Request vom Branch `ue04-<benutzername>`. Gemeint ist Ihr
12: GitHub-Benutzername in Kleinbuchstaben.
13: 
14: | Datei | Aufgabe | Woher |
15: |---|---|---|
16: | `einrichtung.md` | 1 und 2 — womit Sie arbeiten, und ob die Antwort des Agenten stimmt | aus `_vorlage/` |
17: | `sitzung.md` | 2 — die Sitzung mit dem Agenten | entsteht mit `/export` in Ihrem Agenten |
18: 
19: 1. Kopieren Sie das Verzeichnis `_vorlage` nach `<benutzername>`. Die Vorlage
20:    selbst bleibt unverändert.
21: 2. Füllen Sie `einrichtung.md` im Lauf der Übung aus und legen Sie
22:    `sitzung.md` hinzu. Entfernen Sie dort vor dem Commit Pfade mit dem
23:    Namen Ihres Kontos auf dem Rechner, Namen und E-Mail-Adressen; das
24:    Repository ist öffentlich.
25: 
26: Läuft Ihr Agent nicht, reichen Sie trotzdem ein: nur
27: `einrichtung.md`, mit *nein* oder *teilweise* bei „Läuft der Agent?“ und
28: einem Beleg im Abschnitt „Wenn es nicht läuft“ — Schritt, Befehl samt Ausgabe (wörtlich)
29: und was Sie bereits versucht haben.
30: 
31: Das Übungsblatt beschreibt opencode, schreibt es aber nicht vor. Wer schon
32: mit einem anderen Agenten arbeitet — Claude Code, Codex, GitHub Copilot in
33: VS Code oder als Copilot CLI, eine andere Erweiterung —, darf ihn verwenden
34: und trägt ihn in `einrichtung.md` unter „Werkzeug“ ein.
35: 
36: Weitere Dateien, welche der Agent anlegt, gehören nicht in den Pull Request.
37: 
38: > [!IMPORTANT]
39: > Für diese Übung gibt es 1 Bonuspunkt. Diesen erhält nur, wer bis zur
40: > Frist im Moodle-Kurs selbst einen Pull Request mit Inhalten gestellt hat.

---

## Assistant

_Thinking:_

The username is DLM28, but per convention it must be lowercase dlm28. So ue04/DLM28 should be ue04/dlm28. Let me look at the files in there, and confirm whether they are identical to _vorlage. Also check ue04/_vorlage.

Also the modified zuordnung.md has a stray "g" — this is an accidental change presumably. I should report, not necessarily fix (it's their file, and it's their own — I could fix, but user only asked what's there and which files are theirs). Answer question, mention findings.

Let me list untracked files and compare.

**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files -o --exclude-standard; git ls-files ue04; Get-Content ue04/DLM28/einrichtung.md -TotalCount 40"
}
```

ue04/DLM28/einrichtung.md
ue04/README.md
ue04/_vorlage/einrichtung.md
# Einrichtung �?" Coding Agent

<!-- Aufgaben 1 und 2 des �obungsblatts. Ersetzen Sie jedes �?z�?݃?o durch Ihre
     Angabe; die �oberschriften bleiben stehen. L��schen Sie die Kommentare,
     sobald Sie fertig sind. Die Sitzung mit dem Agenten geh��rt nicht
     hierher, sondern als Export in die Datei sitzung.md daneben. -->

## Aufbau

| Angabe | Ihre Angabe |
|---|---|
| L��uft der Agent? | �?� |
| Werkzeug | �?� |
| Version | �?� |
| Betriebssystem | �?� |
| Modellzugang | �?� |
| Modell | �?� |

<!-- L��uft der Agent?: ja, teilweise oder nein. Teilweise hei�Yt, er
     startet, aber ein Schritt danach scheitert (Anmeldung, Antwort,
     Export). Bei teilweise und nein belegen Sie unten unter �?zWenn es nicht
     l��uft�?o, woran es scheitert; ohne laufenden Agenten entf��llt sitzung.md.
     Werkzeug: opencode, oder wer schon damit arbeitet, Claude Code, Codex,
     GitHub Copilot (in VS Code oder als Copilot CLI) oder ein anderer
     Agent. Version: Ausgabe von `opencode --version` bzw.
     die Versionsangabe Ihres Werkzeugs.
     Betriebssystem: macOS, Windows, Windows mit WSL oder Linux.
     Modellzugang: GitHub Copilot, ChatGPT, OpenCode Zen (kostenlos), Claude
     oder ein anderer. Modell: so, wie es in der Auswahl hei�Yt, in opencode
     unter /models. -->

## Antwort des Agenten geprǬft

<!-- Aufgabe 2, Schritt 8: Vergleichen Sie die Antwort des Agenten in
     sitzung.md mit dem, was Sie selbst wissen. Hat er alle Ihre Dateien
     gefunden? Hat er etwas Fremdes fǬr Ihres gehalten oder etwas erfunden?
     Zwei bis drei S��tze. -->

�?�



**Tool: read**

**Input:**
```json
{
  "path": "ue04/_vorlage/einrichtung.md"
}
```

Read file ue04/_vorlage/einrichtung.md, lines 1-55
1: # Einrichtung — Coding Agent
2: 
3: <!-- Aufgaben 1 und 2 des Übungsblatts. Ersetzen Sie jedes „…“ durch Ihre
4:      Angabe; die Überschriften bleiben stehen. Löschen Sie die Kommentare,
5:      sobald Sie fertig sind. Die Sitzung mit dem Agenten gehört nicht
6:      hierher, sondern als Export in die Datei sitzung.md daneben. -->
7: 
8: ## Aufbau
9: 
10: | Angabe | Ihre Angabe |
11: |---|---|
12: | Läuft der Agent? | … |
13: | Werkzeug | … |
14: | Version | … |
15: | Betriebssystem | … |
16: | Modellzugang | … |
17: | Modell | … |
18: 
19: <!-- Läuft der Agent?: ja, teilweise oder nein. Teilweise heißt, er
20:      startet, aber ein Schritt danach scheitert (Anmeldung, Antwort,
21:      Export). Bei teilweise und nein belegen Sie unten unter „Wenn es nicht
22:      läuft“, woran es scheitert; ohne laufenden Agenten entfällt sitzung.md.
23:      Werkzeug: opencode, oder wer schon damit arbeitet, Claude Code, Codex,
24:      GitHub Copilot (in VS Code oder als Copilot CLI) oder ein anderer
25:      Agent. Version: Ausgabe von `opencode --version` bzw.
26:      die Versionsangabe Ihres Werkzeugs.
27:      Betriebssystem: macOS, Windows, Windows mit WSL oder Linux.
28:      Modellzugang: GitHub Copilot, ChatGPT, OpenCode Zen (kostenlos), Claude
29:      oder ein anderer. Modell: so, wie es in der Auswahl heißt, in opencode
30:      unter /models. -->
31: 
32: ## Antwort des Agenten geprüft
33: 
34: <!-- Aufgabe 2, Schritt 8: Vergleichen Sie die Antwort des Agenten in
35:      sitzung.md mit dem, was Sie selbst wissen. Hat er alle Ihre Dateien
36:      gefunden? Hat er etwas Fremdes für Ihres gehalten oder etwas erfunden?
37:      Zwei bis drei Sätze. -->
38: 
39: …
40: 
41: ## Wenn es nicht läuft
42: 
43: <!-- Pflicht bei „teilweise“ und „nein“; bei „ja“ löschen Sie alles unter
44:      der Überschrift. In den Kasten gehört der Befehl, der scheitert, samt
45:      seiner Ausgabe, wörtlich aus dem Terminal kopiert. -->
46: 
47: **Schritt, an dem es scheitert:** …
48: 
49: **Befehl und Ausgabe:**
50: 
51: ```text
52: …
53: ```
54: 
55: **Bereits versucht:** …

---

## Assistant

_Thinking:_

The ue04/DLM28/einrichtung.md appears to be copied but encoding-mangled and truncated? The Get-Content showed through "Antwort des Agenten geprüft" and "…" but not "Wenn es nicht läuft" section — maybe truncated at 40 lines. Let me check file size/lines and compare bytes. It seems encoding is broken (UTF-8 read as something else, mojibake). Actually the read tool output shows mojibake, which may be because the file itself is UTF-8 but PowerShell console encoding. The read tool showed ue04/_vorlage fine. Let me read ue04/DLM28/einrichtung.md with the read tool to see actual content.

**Tool: read**

**Input:**
```json
{
  "path": "ue04/DLM28/einrichtung.md"
}
```

Read file ue04/DLM28/einrichtung.md, lines 1-55
1: # Einrichtung — Coding Agent
2: 
3: <!-- Aufgaben 1 und 2 des Übungsblatts. Ersetzen Sie jedes „…“ durch Ihre
4:      Angabe; die Überschriften bleiben stehen. Löschen Sie die Kommentare,
5:      sobald Sie fertig sind. Die Sitzung mit dem Agenten gehört nicht
6:      hierher, sondern als Export in die Datei sitzung.md daneben. -->
7: 
8: ## Aufbau
9: 
10: | Angabe | Ihre Angabe |
11: |---|---|
12: | Läuft der Agent? | … |
13: | Werkzeug | … |
14: | Version | … |
15: | Betriebssystem | … |
16: | Modellzugang | … |
17: | Modell | … |
18: 
19: <!-- Läuft der Agent?: ja, teilweise oder nein. Teilweise heißt, er
20:      startet, aber ein Schritt danach scheitert (Anmeldung, Antwort,
21:      Export). Bei teilweise und nein belegen Sie unten unter „Wenn es nicht
22:      läuft“, woran es scheitert; ohne laufenden Agenten entfällt sitzung.md.
23:      Werkzeug: opencode, oder wer schon damit arbeitet, Claude Code, Codex,
24:      GitHub Copilot (in VS Code oder als Copilot CLI) oder ein anderer
25:      Agent. Version: Ausgabe von `opencode --version` bzw.
26:      die Versionsangabe Ihres Werkzeugs.
27:      Betriebssystem: macOS, Windows, Windows mit WSL oder Linux.
28:      Modellzugang: GitHub Copilot, ChatGPT, OpenCode Zen (kostenlos), Claude
29:      oder ein anderer. Modell: so, wie es in der Auswahl heißt, in opencode
30:      unter /models. -->
31: 
32: ## Antwort des Agenten geprüft
33: 
34: <!-- Aufgabe 2, Schritt 8: Vergleichen Sie die Antwort des Agenten in
35:      sitzung.md mit dem, was Sie selbst wissen. Hat er alle Ihre Dateien
36:      gefunden? Hat er etwas Fremdes für Ihres gehalten oder etwas erfunden?
37:      Zwei bis drei Sätze. -->
38: 
39: …
40: 
41: ## Wenn es nicht läuft
42: 
43: <!-- Pflicht bei „teilweise“ und „nein“; bei „ja“ löschen Sie alles unter
44:      der Überschrift. In den Kasten gehört der Befehl, der scheitert, samt
45:      seiner Ausgabe, wörtlich aus dem Terminal kopiert. -->
46: 
47: **Schritt, an dem es scheitert:** …
48: 
49: **Befehl und Ausgabe:**
50: 
51: ```text
52: …
53: ```
54: 
55: **Bereits versucht:** …

**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files ue01 ue02 ue03 | Select-String -Pattern \"dlm28\"; Get-ChildItem ue01,ue02,ue03,ue04 -Directory | Select-Object FullName"
}
```


ue01/steckbriefe/dlm28.md
ue02/dlm28/notiz.md
ue02/dlm28/phasenplan.md
ue02/dlm28/spezifikation.md
ue03/dlm28/anforderungen.md
ue03/dlm28/kontext.md
ue03/dlm28/zuordnung.md

FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\aayd


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\abdu113


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\af


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\agbr


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\Agub


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ahyi


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\akyf


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\anas23088


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\anddun


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\andel0


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\anpa


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\anushka


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\athr


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\bima


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\datr03


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\div


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\flk


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\hams


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ivlbs


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\janp


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\jemy


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\jsug


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\lom


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\meq


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mk


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mu


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\mw


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\my55


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\nko


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\NN


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\nohl


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\pz01


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\qho


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\real


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\renn


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\sam


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\skt435


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\snab


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ssda78


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ssng61


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\talh


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\thm-nos


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\thng


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\trry


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\virus


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue02\_zugabe


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\af


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\cms


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\flk


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\janp


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\javu


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\lom


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\meq


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\MK


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mken


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\moh


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mskk15


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mu


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\mw


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\my55


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\nko


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\NN


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\qho


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\real


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\sam


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\snab


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\talh


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\trry


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\val


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\virus


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266


FullName : C:\Users\DLM28\Documents\THM\3. Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\zc


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\DLM28


FullName : C:\Users\DLM28\Documents\THM\3. 
           Semester\Softwaretechnik\�bung1\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage





---

## Assistant

_Thinking:_

We have enough. Key points:

- Repo: THM Softwaretechnik exercises, ue01-ue04, plus AGENTS.md/README.
- User's files: ue01/steckbriefe/dlm28.md, ue02/dlm28/{notiz,phasenplan,spezifikation}.md, ue03/dlm28/{anforderungen,kontext,zuordnung}.md, and untracked ue04/DLM28/einrichtung.md.
- Notes: branch is ue04-DLM28 (capitalized, convention wants lowercase ue04-dlm28). Directory ue04/DLM28 violates lowercase convention; README explicitly says ue04/<benutzername>/ lowercase and branch ue04-<benutzername>.
- einrichtung.md is just the unmodified template (all "…"), no sitzung.md yet.
- Modified ue03/dlm28/zuordnung.md contains accidental "g" before heading — likely an unintended change that should be reverted.
- User is DLM28 based on remote.

Answer in German, concise. No changes made. Ask if they want fix? Just mention. The question only asks what's there and which files are theirs. Provide overview.

Let me maybe count files per exercise quickly? Not necessary but helpful: ue02 has ~100 dirs. Let me get counts.

**Tool: shell**

**Input:**
```json
{
  "command": "foreach ($d in 'ue01','ue02','ue03','ue04') { $n = (git ls-files \"$d\" | Measure-Object).Count; \"$d : $n versionierte Dateien\" }"
}
```

ue01 : 152 versionierte Dateien
ue02 : 339 versionierte Dateien
ue03 : 287 versionierte Dateien
ue04 : 2 versionierte Dateien


---

## Assistant

_Thinking:_

Now answer. Mention mojibake? No, that was just PowerShell display. Actually the read tool shows einrichtung fine, so no encoding issue.

Also note: the user's ue04 directory uses uppercase, and it's untracked. Should I offer to rename? The instructions say ask if unclear which dirs belong to them, but here it's clear (remote user DLM28). Still, user only asked a question. I'll note the deviations and offer.

Keep it structured in German.

## Was im Repository liegt

Das ist der Übungs-Fork für **Softwaretechnik (THM)**. Aufbau:

| Verzeichnis | Inhalt | Versionierte Dateien |
|---|---|---|
| `ue01/` | Steckbriefe (Git/GitHub) | 152 |
| `ue02/` | Projektmodell, je ein Unterordner pro Person | 339 |
| `ue03/` | Anforderungen, je ein Unterordner pro Person | 287 |
| `ue04/` | Coding Agent einrichten (`README.md`, `_vorlage/`) | 2 |
| `README.md`, `AGENTS.md` | Spielregeln des Repositorys | – |

Das `ue02/`- und `ue03/`-Verzeichnis enthalten also die Beiträge aller Kommilitoninnen und Kommilitonen.

## Deine Dateien

Dein GitHub-Benutzername ist **DLM28**, laut Remote `origin`. Dir gehören damit:

- `ue01/steckbriefe/dlm28.md`
- `ue02/dlm28/notiz.md`
- `ue02/dlm28/phasenplan.md`
- `ue02/dlm28/spezifikation.md`
- `ue03/dlm28/anforderungen.md`
- `ue03/dlm28/kontext.md`
- `ue03/dlm28/zuordnung.md`
- `ue04/DLM28/einrichtung.md` — **noch nicht versioniert** (untracked)

Die Commits dazu stammen aus `Steckbrief dlm28 (#90)`, `Übung 2: Ergebnisse von DLM28 (#211)` und `Übung 3: Ergebnisse von dlm28 (#369)`.

## Drei Auffälligkeiten

1. **`ue03/dlm28/zuordnung.md` ist geändert**, aber offenbar versehentlich: In der ersten Zeile steht jetzt `g# Anforderung oder Lösung?` statt `# Anforderung oder Lösung?`. Das würde ich zurücknehmen.
2. **`ue04/DLM28/` ist groß geschrieben.** Die Übung 4 verlangt ausdrücklich `ue04/<benutzername>/` in Kleinbuchstaben, also `ue04/dlm28/`. Ebenso heißt dein Branch `ue04-DLM28` statt `ue04-dlm28`.
3. **`ue04/DLM28/einrichtung.md` ist noch die unveränderte Vorlage** (überall `…`), und `sitzung.md` fehlt noch – Übung 4 ist also inhaltlich noch nicht ausgefüllt.

Soll ich die versehentliche Änderung in `zuordnung.md` zurücknehmen und das Verzeichnis zu `ue04/dlm28/` umbenennen?
