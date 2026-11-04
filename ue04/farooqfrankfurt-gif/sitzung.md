# Repository-Struktur kurz zusammengefasst

**Session ID:** ses_e59f33b7dffe35N3nXl8vAdUql
**Created:** 11/4/2026, 11:13:37 AM
**Updated:** 11/4/2026, 11:15:27 AM

---

## User

Untersuche dieses Repository. Welche Dateien und Ordner gibt es, und wofür sind sie da? Fasse die Struktur kurz zusammen.

---

## Assistant

Ich schaue mir zuerst die oberste Ebene und die README an.



**Tool: shell**

**Input:**
```json
{
  "command": "ls -la"
}
```

total 16
drwxr-xr-x    9 Benutzer  staff   288 Nov  3 18:18 .
drwxr-xr-x+  50 Benutzer   staff  1600 Nov  4 11:10 ..
drwxr-xr-x   15 Benutzer   staff   480 Nov  4 11:05 .git
-rw-r--r--@   1 Benutzer   staff  2172 Nov  3 18:18 AGENTS.md
-rw-r--r--@   1 Benutzer   staff  3212 Nov  3 18:18 README.md
drwxr-xr-x    4 Benutzer   staff   128 Nov  3 18:18 ue01
drwxr-xr-x  113 Benutzer   staff  3616 Nov  3 18:18 ue02
drwxr-xr-x@  99 Benutzer   staff  3168 Nov  3 18:18 ue03
drwxr-xr-x@   5 Benutzer   staff   160 Nov  4 11:06 ue04


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

Let me explore the structure. There are many directories in ue02 and ue03 (one per student). Let's get a compact view.

**Tool: shell**

**Input:**
```json
{
  "command": "find ue01 ue04 -maxdepth 3 | head -50; echo; ls ue02 | head -20; echo \"ue02 Anzahl: $(ls ue02 | wc -l)\"; ls ue03 | head -20; echo \"ue03 Anzahl: $(ls ue03 | wc -l)\""
}
```

ue01
ue01/README.md
ue01/steckbriefe
ue01/steckbriefe/ivlbs.md
ue01/steckbriefe/sahmed.md
ue01/steckbriefe/hams.md
ue01/steckbriefe/my55.md
ue01/steckbriefe/zcoel.md
ue01/steckbriefe/Z-266.md
ue01/steckbriefe/jp26.md
ue01/steckbriefe/jsug.md
ue01/steckbriefe/aalg.md
ue01/steckbriefe/nly50.md
ue01/steckbriefe/agbr.md
ue01/steckbriefe/AR.md
ue01/steckbriefe/azm96.md
ue01/steckbriefe/jk04.md
ue01/steckbriefe/anddun.md
ue01/steckbriefe/mu.md
ue01/steckbriefe/bima.md
ue01/steckbriefe/mkon.md
ue01/steckbriefe/Fahm.md
ue01/steckbriefe/iaa.md
ue01/steckbriefe/uwar.md
ue01/steckbriefe/ekes.md
ue01/steckbriefe/meq.md
ue01/steckbriefe/mbgrn04.md
ue01/steckbriefe/yoibr42.md
ue01/steckbriefe/skt435.md
ue01/steckbriefe/javu.md
ue01/steckbriefe/yamekk.md
ue01/steckbriefe/nblh.md
ue01/steckbriefe/lpr2.md
ue01/steckbriefe/fpz.md
ue01/steckbriefe/nohl.md
ue01/steckbriefe/dmal2004.md
ue01/steckbriefe/ygue.md
ue01/steckbriefe/asi.md
ue01/steckbriefe/uk.md
ue01/steckbriefe/sahmad.md
ue01/steckbriefe/jvng.md
ue01/steckbriefe/datr03.md
ue01/steckbriefe/wnga.md
ue01/steckbriefe/flk.md
ue01/steckbriefe/kraz.md
ue01/steckbriefe/peng.md
ue01/steckbriefe/zc.md
ue01/steckbriefe/mjab.md
ue01/steckbriefe/tyfncc.md
ue01/steckbriefe/TariqK2004.md

Agub
IY69
Lpr
NN
NUAli
README.md
TariqK2004
_vorlage
_zugabe
aayd
abdu113
af
agbr
ahyi
akyf
anas23088
anddun
andel0
anpa
anushka
ue02 Anzahl:      111
IY69
Lpr
MK
NN
NUAli
README.md
TariqK2004
_vorlage
aayd
af
agbr
ahyi
akyf
anas23088
anddun
andel0
anpa
anushka
avon507
ayue
ue03 Anzahl:       97


**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current; git log --oneline -10; git status --short | head -20"
}
```

ue04-farooqfrankfurt-gif
36dab57 Merge branch 'carstenlucke:main' into main
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)
8cfd580 Übung 2: Formatierung der Gesprächsnotiz korrigiert (#286)
baaa2b8 Ergebnisse der Phasen ergänzt in phasenplan.md (#284)
c55409f Übung 2 : Ergebnisse von akyf (#283)
9db8067 Ue02 zsh (#281)
?? ue04/farooqfrankfurt-gif/


---

## Assistant

_Thinking:_

Let's look at the READMEs of each exercise, and the _vorlage/_zugabe folders, plus ue04 contents.

**Tool: read**

**Input:**
```json
{
  "path": "ue01/README.md"
}
```

Read file ue01/README.md, lines 1-23
1: # Übung 1 — Erste Schritte mit Git und GitHub
2: 
3: In dieser Übung gehen Sie den Weg einer Änderung einmal vollständig: vom
4: eigenen Rechner bis in dieses Repository. Die Anleitung steht im
5: [Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/).
6: 
7: ## Was Sie einreichen
8: 
9: Einzureichen ist Ihr Steckbrief als Datei `steckbriefe/<benutzername>.md`,
10: und zwar als Pull Request vom Branch `steckbrief-<benutzername>`. Gemeint
11: ist Ihr GitHub-Benutzername in Kleinbuchstaben.
12: 
13: 1. Kopieren Sie `steckbriefe/_vorlage.md` nach
14:    `steckbriefe/<benutzername>.md` und ersetzen Sie in der Überschrift
15:    `<benutzername>` durch Ihren GitHub-Benutzernamen in Kleinbuchstaben. Die
16:    Vorlage selbst bleibt unverändert.
17: 2. Füllen Sie die drei Abschnitte aus — im Lauf der Übung einen nach dem
18:    anderen, jeweils als eigenen Commit.
19: 
20: `steckbriefe/_beispiel.md` zeigt, wie ein ausgefüllter Steckbrief aussehen kann.
21: 
22: Für den rechtzeitig gestellten Pull Request gibt es Bonuspunkte; die
23: Bedingungen stehen im Übungsblatt.

**Tool: read**

**Input:**
```json
{
  "path": "ue02/README.md"
}
```

Read file ue02/README.md, lines 1-36
1: # Übung 2 — Das Projektmodell am Fall
2: 
3: In dieser Übung schreiben Sie Markdown und wenden das Projektmodell auf
4: einen konkreten Fall an, d.h. auf einen Terminplaner für die THM. Die
5: Aufgaben stehen im
6: [Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue02-projektmodell/).
7: 
8: ## Was Sie einreichen
9: 
10: Einzureichen ist ein Verzeichnis `ue02/<benutzername>/` mit drei Dateien,
11: und zwar als Pull Request vom Branch `ue02-<benutzername>`. Gemeint ist Ihr
12: GitHub-Benutzername in Kleinbuchstaben.
13: 
14: | Datei | Aufgabe | Woher |
15: |---|---|---|
16: | `notiz.md` | 1 — eine Gesprächsnotiz in Markdown bringen | aus `_vorlage/` |
17: | `phasenplan.md` | 2 — Tätigkeiten den Phasen zuordnen | entsteht im Übungsblatt und wird dort heruntergeladen |
18: | `spezifikation.md` | 3 — Gliederung einer Spezifikation | aus `_vorlage/` |
19: | `rollen.md` | 5 — Zugabe, freiwillig: Rollen besetzen | aus `_zugabe/` |
20: 
21: 1. Kopieren Sie das Verzeichnis `_vorlage` nach `<benutzername>`. Die Vorlage
22:    selbst bleibt unverändert.
23: 2. Bearbeiten Sie die Dateien im Lauf der Übung und legen Sie
24:    `phasenplan.md` hinzu.
25: 
26: Die Aufgaben 3 und 5 bearbeiten Sie allein oder in einer Gruppe bis vier
27: Personen. Im Kopf von `spezifikation.md` und `rollen.md` stehen die
28: GitHub-Benutzernamen aller Personen, die mitgearbeitet haben.
29: 
30: > [!IMPORTANT]
31: > Für diese Übung gibt es 1 Bonuspunkt. Diesen erhält nur, wer bis zur
32: > Frist im Moodle-Kurs selbst einen Pull Request mit Inhalten gestellt hat.
33: > Daher reicht jedes Mitglied einer Gruppe selbst ein: Es legt die gemeinsamen
34: > Dateien in seinem eigenen Verzeichnis ab, überträgt sie in seinen eigenen
35: > Fork und stellt einen eigenen Pull Request. Die Benutzernamen im Kopf der
36: > Dateien ergänzen dies lediglich.

**Tool: read**

**Input:**
```json
{
  "path": "ue03/README.md"
}
```

Read file ue03/README.md, lines 1-30
1: # Übung 3 — Anforderungen an den Terminplaner
2: 
3: In dieser Übung bestimmen Sie Stakeholder und Systemkontext des Terminplaners
4: für die THM, unterscheiden Anforderungen von Lösungen und formulieren eigene
5: Anforderungen. Die Aufgaben stehen im
6: [Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue03-anforderungen/).
7: 
8: ## Was Sie einreichen
9: 
10: Einzureichen ist ein Verzeichnis `ue03/<benutzername>/` mit drei Dateien,
11: und zwar als Pull Request vom Branch `ue03-<benutzername>`. Gemeint ist Ihr
12: GitHub-Benutzername in Kleinbuchstaben.
13: 
14: | Datei | Aufgabe | Woher |
15: |---|---|---|
16: | `kontext.md` | 1 — Stakeholder und Systemkontext | aus `_vorlage/` |
17: | `zuordnung.md` | 2 — Anforderung oder Lösung? | entsteht im Übungsblatt und wird dort heruntergeladen |
18: | `anforderungen.md` | 3 — Eigene Anforderungen | aus `_vorlage/` |
19: 
20: 1. Kopieren Sie das Verzeichnis `_vorlage` nach `<benutzername>`. Die Vorlage
21:    selbst bleibt unverändert.
22: 2. Bearbeiten Sie die Dateien im Lauf der Übung und legen Sie
23:    `zuordnung.md` hinzu.
24: 
25: Alle Aufgaben bearbeiten Sie allein. Ihre Gesprächsnotiz aus Übung 2 lesen
26: Sie nur; ändern Sie dort nichts.
27: 
28: > [!IMPORTANT]
29: > Für diese Übung gibt es 1 Bonuspunkt. Diesen erhält nur, wer bis zur
30: > Frist im Moodle-Kurs selbst einen Pull Request mit Inhalten gestellt hat.

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

Now inspect _vorlage folders and ue04/farooqfrankfurt-gif, and check any hidden files / configs. Also the ue01/steckbriefe folder with _vorlage, _beispiel.

Also check .git for hooks etc. probably not needed. Let's list contents of ue02/_vorlage, ue02/_zugabe, ue03/_vorlage, ue04/_vorlage, ue04/farooqfrankfurt-gif, ue01/steckbriefe/_vorlage.md etc.

Also see if there's any .gitignore, .github workflows. Top-level listing showed none besides .git.

**Tool: shell**

**Input:**
```json
{
  "command": "ls -la ue02/_vorlage ue02/_zugabe ue03/_vorlage ue04/_vorlage ue04/farooqfrankfurt-gif 2>&1"
}
```

ue02/_vorlage:
total 16
drwxr-xr-x    4 Benutzer  staff   128 Oct 24 20:45 .
drwxr-xr-x  113 Benutzer  staff  3616 Nov  3 18:18 ..
-rw-r--r--    1 Benutzer  staff  1523 Oct 24 20:45 notiz.md
-rw-r--r--    1 Benutzer  staff   463 Oct 24 20:45 spezifikation.md

ue02/_zugabe:
total 8
drwxr-xr-x    3 Benutzer  staff    96 Oct 24 21:34 .
drwxr-xr-x  113 Benutzer  staff  3616 Nov  3 18:18 ..
-rw-r--r--    1 Benutzer  staff  1008 Oct 24 20:45 rollen.md

ue03/_vorlage:
total 16
drwxr-xr-x@  4 Benutzer  staff   128 Oct 27 10:31 .
drwxr-xr-x@ 99 Benutzer  staff  3168 Nov  3 18:18 ..
-rw-r--r--@  1 Benutzer  staff   709 Oct 27 10:31 anforderungen.md
-rw-r--r--@  1 Benutzer  staff   837 Oct 27 10:31 kontext.md

ue04/_vorlage:
total 8
drwxr-xr-x@ 3 Benutzer  staff    96 Nov  3 18:18 .
drwxr-xr-x@ 5 Benutzer  staff   160 Nov  4 11:06 ..
-rw-r--r--@ 1 Benutzer  staff  1946 Nov  3 18:18 einrichtung.md

ue04/farooqfrankfurt-gif:
total 8
drwxr-xr-x@ 3 Benutzer  staff    96 Nov  4 11:06 .
drwxr-xr-x@ 5 Benutzer  staff   160 Nov  4 11:06 ..
-rw-r--r--@ 1 Benutzer  staff  1946 Nov  4 11:06 einrichtung.md


**Tool: shell**

**Input:**
```json
{
  "command": "ls ue01/steckbriefe | grep '^_' ; echo \"--- Anzahl Steckbriefe: $(ls ue01/steckbriefe | wc -l)\"; echo \"--- Beispiel ue02-Eintrag:\"; ls ue02/agbr; echo \"--- Beispiel ue03-Eintrag:\"; ls ue03/agbr"
}
```

_beispiel.md
_vorlage.md
--- Anzahl Steckbriefe:      151
--- Beispiel ue02-Eintrag:
notiz.md
phasenplan.md
spezifikation.md
--- Beispiel ue03-Eintrag:
anforderungen.md
kontext.md
zuordnung.md


---

## Assistant

_Thinking:_

Let me also check if there are nested dirs in student folders (some may have extra files). And check counts of folders, and whether the repo has any other hidden files like .gitignore. Also .git/hooks? Not relevant.

Quick check for nested directories and file types across.

**Tool: shell**

**Input:**
```json
{
  "command": "find ue02 ue03 -mindepth 2 -type d | head; echo \"--- Dateitypen:\"; find ue01 ue02 ue03 ue04 -type f | sed 's/.*\\.//' | sort | uniq -c | sort -rn"
}
```

--- Dateitypen:
 781 md


**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files | grep -v '^ue0[123]/' ; echo \"--- getrackte Dateien gesamt: $(git ls-files | wc -l)\""
}
```

AGENTS.md
README.md
ue04/README.md
ue04/_vorlage/einrichtung.md
--- getrackte Dateien gesamt:      782


---

## Assistant

_Thinking:_

So ue04/farooqfrankfurt-gif is untracked (the current student's work). Everything is markdown.

Let me peek at the vorlage contents briefly to describe purpose.

**Tool: shell**

**Input:**
```json
{
  "command": "head -15 ue01/steckbriefe/_vorlage.md; echo \"###\"; head -12 ue02/_vorlage/notiz.md; echo \"###\"; head -10 ue03/_vorlage/kontext.md; echo \"###\"; head -12 ue04/_vorlage/einrichtung.md"
}
```

# Steckbrief <benutzername>

## Studiengang und Semester

…

## Meine bisherige Erfahrung mit Softwareentwicklung

…

## Das erwarte ich von der Veranstaltung

…
###
<!-- Diese Notiz hat noch keine Form. Bringen Sie sie in Markdown, wie es
     Aufgabe 1 des Übungsblatts beschreibt, ohne am Inhalt etwas zu ändern.
     Löschen Sie diesen Kommentar, sobald Sie fertig sind. -->

Gesprächsnotiz: Terminplaner für die THM
Worum es geht
Die THM möchte eine Software zur Planung und Vereinbarung von Terminen. Lehrende bieten Sprechstunden und Prüfungstermine an, Studierende buchen sie, Sekretariate behalten den Überblick.
Die Software soll sich über das Hochschulkonto bedienen lassen. Zunächst soll sie Termine als iCal-Datei zum Herunterladen anbieten, später vielleicht direkt in die Kalender der Beteiligten eintragen.
Außerdem soll sie eine API bekommen, über die KI-Agenten sie steuern können.
Die THM sagte dazu wörtlich: Wir wollen nicht noch ein Werkzeug, das am Ende keiner benutzt.
Wichtig: Noch ist nichts beauftragt, wir sollen zuerst einen Vorschlag machen.
Was heute benutzt wird
###
# Stakeholder und Systemkontext — Terminplaner für die THM

<!-- Aufgabe 1 des Übungsblatts. Ersetzen Sie die Platzhalter … und fügen
     Sie so viele Zeilen hinzu, wie Sie benötigen. Löschen Sie die
     Kommentare, sobald Sie fertig sind. -->

## Stakeholder

<!-- Mindestens sechs Stakeholder, je mit einem Satz dazu, worauf sie
     Einfluss haben. -->
###
# Einrichtung — Coding Agent

<!-- Aufgaben 1 und 2 des Übungsblatts. Ersetzen Sie jedes „…“ durch Ihre
     Angabe; die Überschriften bleiben stehen. Löschen Sie die Kommentare,
     sobald Sie fertig sind. Die Sitzung mit dem Agenten gehört nicht
     hierher, sondern als Export in die Datei sitzung.md daneben. -->

## Aufbau

| Angabe | Ihre Angabe |
|---|---|
| Läuft der Agent? | … |


---

## Assistant

_Thinking:_

Now I can summarize. Also note branch is ue04-farooqfrankfurt-gif, untracked ue04/farooqfrankfurt-gif/einrichtung.md. Mention that.

Let me count the number of ue02/ue03 subfolders excluding _vorlage/_zugabe/README. ue02: 111 entries, minus README.md, _vorlage, _zugabe = 108 folders. ue03: 97 - README - _vorlage = 95 folders. ue01: 151 files - 2 underscore = 149 steckbriefe. I could verify quickly but fine; let me compute properly.

**Tool: shell**

**Input:**
```json
{
  "command": "echo \"ue01 Steckbriefe: $(ls ue01/steckbriefe/*.md | grep -v '/_' | wc -l)\"; echo \"ue02 Verzeichnisse: $(find ue02 -mindepth 1 -maxdepth 1 -type d | grep -v '/_' | wc -l)\"; echo \"ue03 Verzeichnisse: $(find ue03 -mindepth 1 -maxdepth 1 -type d | grep -v '/_' | wc -l)\""
}
```

ue01 Steckbriefe:      149
ue02 Verzeichnisse:      108
ue03 Verzeichnisse:       95


---

## Assistant

## Überblick

Das Repository ist das Übungsrepository zur Vorlesung **Softwaretechnik** (THM Friedberg). Es enthält ausschließlich Markdown-Dateien (781 getrackte `.md`-Dateien) und ist nach Übungen gegliedert. Jede Übung hat ein eigenes Verzeichnis mit eigener `README.md`, die die Abgabe beschreibt.

```
.
├── AGENTS.md          Regeln für KI-Agenten (deutsch, nur eigene Dateien, nicht auf main, kein Persönliches)
├── README.md          Gesamtüberblick, Ablauf über Fork → Branch → PR, Spielregeln
├── ue01/              Erste Schritte mit Git und GitHub
│   ├── README.md
│   └── steckbriefe/   149 Steckbriefe + _vorlage.md + _beispiel.md
├── ue02/              Das Projektmodell am Fall (Terminplaner)
│   ├── README.md
│   ├── _vorlage/      notiz.md, spezifikation.md
│   ├── _zugabe/       rollen.md (freiwillige Aufgabe 5)
│   └── <benutzername>/ 108 Abgabeverzeichnisse, je notiz.md, phasenplan.md, spezifikation.md (+ ggf. rollen.md)
├── ue03/              Anforderungen an den Terminplaner
│   ├── README.md
│   ├── _vorlage/      kontext.md, anforderungen.md
│   └── <benutzername>/ 95 Abgabeverzeichnisse, je kontext.md, zuordnung.md, anforderungen.md
└── ue04/              Einen Coding Agent einrichten
    ├── README.md
    ├── _vorlage/      einrichtung.md
    └── farooqfrankfurt-gif/  (dein Abgabeverzeichnis, noch nicht committet)
```

## Zweck der Teile

- **`ue01/steckbriefe/`** – Ein Steckbrief pro Studierendem (`<benutzername>.md`) mit Studiengang, Vorerfahrung und Erwartungen. `_vorlage.md` ist die leere Vorlage, `_beispiel.md` ein Muster.
- **`ue02/<benutzername>/`** – Projektmodell am Fall „Terminplaner für die THM“: eine Gesprächsnotiz in Markdown (`notiz.md`), die Zuordnung von Tätigkeiten zu Projektphasen (`phasenplan.md`) und eine Spezifikationsgliederung (`spezifikation.md`); optional `rollen.md` aus `_zugabe/`.
- **`ue03/<benutzername>/`** – Anforderungsanalyse: Stakeholder und Systemkontext (`kontext.md`), Unterscheidung Anforderung/Lösung (`zuordnung.md`), eigene Anforderungen (`anforderungen.md`).
- **`ue04/<benutzername>/`** – Dokumentation der Einrichtung eines Coding Agenten (`einrichtung.md`) und der Sitzung mit ihm (`sitzung.md`).

## Konventionen

- Ein Verzeichnis bzw. eine Datei pro GitHub-Benutzername (klein geschrieben); Vorlagen beginnen mit `_` und bleiben unverändert.
- Abgabe jeweils über einen Branch `ueNN-<benutzername>` und Pull Request; `main` bleibt unberührt.
- Nichts Persönliches (Klarnamen, E-Mail, Matrikelnummer, lokale Pfade) in Dateien oder Commits.

## Aktueller Stand deiner Arbeit

Du bist auf dem Branch `ue04-farooqfrankfurt-gif`. Neu und noch nicht versioniert ist `ue04/farooqfrankfurt-gif/einrichtung.md` – die Vorlage ist dorthin kopiert, aber inhaltlich noch nicht ausgefüllt (überall `…`), und `sitzung.md` fehlt noch.

---

## User

Hast du bei deiner Untersuchung alle wichtigen Dateien und Ordner im Repository berücksichtigt? Prüfe insbesondere auch die Ordner ue02, ue03 und ue04. Nenne die wichtigsten Dateien und ihren Zweck. 

---

## Assistant

_Thinking:_

The user asks whether I considered all important files/folders, especially ue02, ue03, ue04. I should do a deeper check: hidden files, files not .md, nested directories, unusual files in student folders, ue04 contents, maybe .github workflows, .gitignore, etc. Let me be thorough.

Let me check:
- `git ls-files` full listing structure
- hidden files anywhere (`find . -name '.*' -not -path './.git/*'`)
- any non-md files tracked
- files inside ue02/ue03 student folders beyond the expected 3
- ue04 complete tree
- .gitignore / .github

Let's run.

Gute Frage — ich prüfe das systematisch nach, statt mich auf den ersten Eindruck zu verlassen.



**Tool: shell**

**Input:**
```json
{
  "command": "echo \"=== Alle nicht-.git-Dateien, die nicht auf .md enden ===\"; find . -path ./.git -prune -o -type f ! -name '*.md' -print; echo; echo \"=== Versteckte Dateien/Ordner (außer .git) ===\"; find . -path ./.git -prune -o -name '.*' -print"
}
```

=== Alle nicht-.git-Dateien, die nicht auf .md enden ===

=== Versteckte Dateien/Ordner (außer .git) ===
.


**Tool: shell**

**Input:**
```json
{
  "command": "echo \"=== ue04 komplett ===\"; find ue04 -print | sort; echo; echo \"=== ue02-Dateien, die nicht zur erwarteten Menge gehören ===\"; find ue02 -mindepth 2 -type f ! -name 'notiz.md' ! -name 'phasenplan.md' ! -name 'spezifikation.md' ! -name 'rollen.md' -print; echo; echo \"=== ue03-Dateien, die nicht zur erwarteten Menge gehören ===\"; find ue03 -mindepth 2 -type f ! -name 'kontext.md' ! -name 'zuordnung.md' ! -name 'anforderungen.md' -print"
}
```

=== ue04 komplett ===
ue04
ue04/README.md
ue04/_vorlage
ue04/_vorlage/einrichtung.md
ue04/farooqfrankfurt-gif
ue04/farooqfrankfurt-gif/einrichtung.md

=== ue02-Dateien, die nicht zur erwarteten Menge gehören ===

=== ue03-Dateien, die nicht zur erwarteten Menge gehören ===


---

## Assistant

_Thinking:_

Good. Now check nested directories: none found earlier (find -mindepth 2 -type d gave nothing? earlier command output showed nothing before "--- Dateitypen"). So flat.

Check counts of files: how many have rollen.md, phasenplan.md etc. Also check whether there are tracked vs untracked files. And check git status fully. Also check if ue02/ue03 student folders are all tracked. Also check names that start with underscore at student level.

Also important: `_vorlage`/`_zugabe` files, `README.md` in each. Check whether there are any directories in ue01 besides steckbriefe. Already known.

Let me also verify git status --short full (untracked dir). And check for case variations in folder names (e.g., ue01 steckbriefe have uppercase names, which is allowed? README says lowercase... but not my business).

Also check that ue02/ue03 each student folder has all expected files — completeness stats might be useful but not needed. However "wichtigste Dateien und ihren Zweck" — I should name README, AGENTS, vorlagen, and describe per-exercise files. Maybe show an example student folder.

Let me run a few checks: counts of rollen.md, missing phasenplan, etc. And full git status.

**Tool: shell**

**Input:**
```json
{
  "command": "echo \"=== git status ===\"; git status --short; echo; echo \"=== Dateizahlen in ue02 ===\"; for f in notiz.md phasenplan.md spezifikation.md rollen.md; do echo \"$f: $(find ue02 -mindepth 2 -name $f | wc -l)\"; done; echo \"=== Dateizahlen in ue03 ===\"; for f in kontext.md zuordnung.md anforderungen.md; do echo \"$f: $(find ue03 -mindepth 2 -name $f | wc -l)\"; done"
}
```

=== git status ===
?? ue04/farooqfrankfurt-gif/

=== Dateizahlen in ue02 ===
notiz.md:      108
phasenplan.md:      103
spezifikation.md:      108
rollen.md:       19
=== Dateizahlen in ue03 ===
kontext.md:       96
zuordnung.md:       94
anforderungen.md:       96


**Tool: shell**

**Input:**
```json
{
  "command": "echo \"=== Ordner mit Unterordnern? ===\"; find ue02 ue03 -mindepth 2 -type d; echo \"(keine Ausgabe = flach)\"; echo; echo \"=== Namen mit Unterstrich auf oberster Ebene ===\"; ls -d ue0*/_* 2>/dev/null; echo; echo \"=== Vorlagen-Dateien mit Inhalt ===\"; wc -l ue01/steckbriefe/_*.md ue02/_vorlage/*.md ue02/_zugabe/*.md ue03/_vorlage/*.md ue04/_vorlage/*.md"
}
```

=== Ordner mit Unterordnern? ===
(keine Ausgabe = flach)

=== Namen mit Unterstrich auf oberster Ebene ===
ue02/_vorlage
ue02/_zugabe
ue03/_vorlage
ue04/_vorlage

=== Vorlagen-Dateien mit Inhalt ===
      17 ue01/steckbriefe/_beispiel.md
      13 ue01/steckbriefe/_vorlage.md
      26 ue02/_vorlage/notiz.md
      16 ue02/_vorlage/spezifikation.md
      34 ue02/_zugabe/rollen.md
      19 ue03/_vorlage/anforderungen.md
      31 ue03/_vorlage/kontext.md
      55 ue04/_vorlage/einrichtung.md
     211 total


---

## Assistant

_Thinking:_

Interesting: ue03 has 95 directories but kontext.md 96 — because _vorlage also has kontext.md (find -mindepth 2 includes _vorlage). So student counts: 95 each minus vorlage = kontext 95, zuordnung 94, anforderungen 95. Wait kontext.md count 96 includes ue03/_vorlage/kontext.md → 95 student files. anforderungen.md 96 → 95 student. zuordnung.md 94 → one missing. Let me verify which. Also ue02: 108 notiz (no vorlage notiz? ue02/_vorlage/notiz.md counts → so 107 student notiz?). Hmm: ue02/_vorlage/notiz.md is at depth 2 (ue02/_vorlage/notiz.md), yes find -mindepth 2 -name notiz.md includes it. So 108 - 1 = 107 student notiz, 103 - 0 (no phasenplan in vorlage) = 103 student phasenplan, 108 - 1 = 107 spezifikation, rollen 19 - 1 (zugabe) = 18. But 108 student directories. So one directory lacks notiz/spezifikation? Which one? Probably a folder with only README? Let me check. Also missing phasenplan in 5 dirs, missing zuordnung in 1.

This is worth checking to name precisely. Let me find directories missing expected files.

**Tool: shell**

**Input:**
```json
{
  "command": "cd ue02 && for d in */; do d=${d%/}; [ \"$d\" = \"_vorlage\" ] && continue; [ \"$d\" = \"_zugabe\" ] && continue; for f in notiz.md phasenplan.md spezifikation.md; do [ -f \"$d/$f\" ] || echo \"ue02/$d fehlt $f\"; done; done; cd ../ue03 && for d in */; do d=${d%/}; [ \"$d\" = \"_vorlage\" ] && continue; for f in kontext.md zuordnung.md anforderungen.md; do [ -f \"$d/$f\" ] || echo \"ue03/$d fehlt $f\"; done; done"
}
```

ue02/jvng fehlt phasenplan.md
ue02/mk fehlt notiz.md
ue02/mk fehlt spezifikation.md
ue02/skt435 fehlt phasenplan.md
ue02/ssda78 fehlt phasenplan.md
ue02/ssng61 fehlt phasenplan.md
ue02/ysbi82 fehlt phasenplan.md
ue03/mskk15 fehlt zuordnung.md


---

## Assistant

_Thinking:_

What's in ue02/mk? Let's check. Maybe a stray file? Earlier the "unexpected files" check found none — so ue02/mk may be empty? find -mindepth 2 -type f found no unexpected files. So mk is an empty directory (or contains only subdirs, but no subdirs). Empty dirs aren't tracked by git, so maybe mk exists locally empty and not tracked. Let me check.

**Tool: shell**

**Input:**
```json
{
  "command": "ls -la ue02/mk; echo \"--- getrackt unter ue02/mk:\"; git ls-files ue02/mk | head; echo \"--- mk im Index/HEAD?\"; git ls-tree HEAD ue02/ | grep -w mk"
}
```

total 8
drwxr-xr-x@   3 Benutzer  staff    96 Oct 27 10:31 .
drwxr-xr-x  113 Benutzer  staff  3616 Nov  3 18:18 ..
-rw-r--r--@   1 Benutzer  staff  3691 Oct 27 10:31 phasenplan.md
--- getrackt unter ue02/mk:
ue02/mk/phasenplan.md
--- mk im Index/HEAD?
040000 tree d2383ca72819393fcf4eb318bd8af75b2a73534d	ue02/mk


**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files | awk -F/ '{print $1\"/\"$2}' | sort | uniq -c | sort -rn | head -5; echo \"--- ue04 getrackt:\"; git ls-files ue04"
}
```

 151 ue01/steckbriefe
   4 ue02/wnga
   4 ue02/tyfncc
   4 ue02/trry
   4 ue02/talh
--- ue04 getrackt:
ue04/README.md
ue04/_vorlage/einrichtung.md


---

## Assistant

_Thinking:_

So `ue02/mk` only contains phasenplan.md (an incomplete submission). That's a real detail worth naming? Maybe not critical but it is an anomaly.

Now let's look at what's actually inside the vorlagen to describe purpose accurately, plus the README files. I already read READMEs. Let me read the vorlage files fully to describe them (short). Also ue04/farooqfrankfurt-gif/einrichtung.md content (student's own, same as template presumably).

Also check ue01 steckbriefe uppercase names — some violate lowercase rule; not necessary to mention but could note as anomaly? The question is about structure, not review. Maybe mention briefly.

Let me read the templates quickly.

**Tool: shell**

**Input:**
```json
{
  "command": "cat ue02/_vorlage/spezifikation.md; echo \"=====ROLLEN\"; cat ue02/_zugabe/rollen.md; echo \"=====ANFORDERUNGEN\"; cat ue03/_vorlage/anforderungen.md"
}
```

# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @…

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## …

…

## …

…
=====ROLLEN
# Rollen — Terminplaner für die THM

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @…

## Der Kunde

| Bereich | Wer ist das an der THM? | Woran machen Sie es fest? |
|---|---|---|
| Fachbereich (eigentlicher Auftraggeber) | … | … |
| IT-Bereich | … | … |

## Das Projektteam

Vier Personen: A, B, C und D.

| Rolle | Wer |
|---|---|
| Projektmanager | … |
| Projektleiter | … |
| Chefdesigner | … |
| Entwickler | … |
| Qualitätsbeauftragter | … |

Diese Rollen haben wir zusammengelegt, da …

Diese Rollen halten wir getrennt, da …

## Drei Situationen

| Situation | Wer entscheidet? | Wer muss davon erfahren? |
|---|---|---|
| Ein Sekretariat wünscht sich während der Implementierung zusätzlich eine Raumbuchung. | … | … |
| Der Systemtest zeigt, dass Benachrichtigungen bei vielen gleichzeitigen Buchungen erst nach Minuten ankommen. | … | … |
| Um den Einführungstermin zu halten, braucht das Projekt zwei weitere Entwickler. | … | … |
=====ANFORDERUNGEN
# Anforderungen — Terminplaner für die THM

<!-- Aufgabe 3 des Übungsblatts, ohne Hilfsmittel. Je Zeile eine
     Anforderung in einem Satz, dazu der Stakeholder, von dem sie stammt,
     und die Art: FA, QA oder RB. Mindestens acht Anforderungen, davon
     mindestens zwei je Art; die Nummern laufen A01, A02 … Löschen Sie die
     Kommentare, sobald Sie fertig sind. -->

| Nr. | Anforderung | Stakeholder | Art |
|---|---|---|---|
| A01 | … | … | … |

## Eine Anforderung, die niemand ausgesprochen hat

<!-- Nummer der Anforderung aus der Tabelle, welche im Gespräch niemand
     ausgesprochen hat, obwohl sie gilt, und in ein bis zwei Sätzen, warum
     sie niemand genannt hat. -->

…


**Tool: shell**

**Input:**
```json
{
  "command": "sed -n '1,55p' ue04/_vorlage/einrichtung.md; echo \"=====VERGLEICH mit Abgabe\"; diff ue04/_vorlage/einrichtung.md ue04/farooqfrankfurt-gif/einrichtung.md && echo \"identisch\""
}
```

# Einrichtung — Coding Agent

<!-- Aufgaben 1 und 2 des Übungsblatts. Ersetzen Sie jedes „…“ durch Ihre
     Angabe; die Überschriften bleiben stehen. Löschen Sie die Kommentare,
     sobald Sie fertig sind. Die Sitzung mit dem Agenten gehört nicht
     hierher, sondern als Export in die Datei sitzung.md daneben. -->

## Aufbau

| Angabe | Ihre Angabe |
|---|---|
| Läuft der Agent? | … |
| Werkzeug | … |
| Version | … |
| Betriebssystem | … |
| Modellzugang | … |
| Modell | … |

<!-- Läuft der Agent?: ja, teilweise oder nein. Teilweise heißt, er
     startet, aber ein Schritt danach scheitert (Anmeldung, Antwort,
     Export). Bei teilweise und nein belegen Sie unten unter „Wenn es nicht
     läuft“, woran es scheitert; ohne laufenden Agenten entfällt sitzung.md.
     Werkzeug: opencode, oder wer schon damit arbeitet, Claude Code, Codex,
     GitHub Copilot (in VS Code oder als Copilot CLI) oder ein anderer
     Agent. Version: Ausgabe von `opencode --version` bzw.
     die Versionsangabe Ihres Werkzeugs.
     Betriebssystem: macOS, Windows, Windows mit WSL oder Linux.
     Modellzugang: GitHub Copilot, ChatGPT, OpenCode Zen (kostenlos), Claude
     oder ein anderer. Modell: so, wie es in der Auswahl heißt, in opencode
     unter /models. -->

## Antwort des Agenten geprüft

<!-- Aufgabe 2, Schritt 8: Vergleichen Sie die Antwort des Agenten in
     sitzung.md mit dem, was Sie selbst wissen. Hat er alle Ihre Dateien
     gefunden? Hat er etwas Fremdes für Ihres gehalten oder etwas erfunden?
     Zwei bis drei Sätze. -->

…

## Wenn es nicht läuft

<!-- Pflicht bei „teilweise“ und „nein“; bei „ja“ löschen Sie alles unter
     der Überschrift. In den Kasten gehört der Befehl, der scheitert, samt
     seiner Ausgabe, wörtlich aus dem Terminal kopiert. -->

**Schritt, an dem es scheitert:** …

**Befehl und Ausgabe:**

```text
…
```

**Bereits versucht:** …
=====VERGLEICH mit Abgabe
identisch


---

## Assistant

_Thinking:_

I have a full picture now. Let me also check ue01/steckbriefe counts and whether some names are uppercase (inconsistent with rule) — could mention as anomaly but not essential. The user asks: "Hast du bei deiner Untersuchung alle wichtigen Dateien und Ordner im Repository berücksichtigt? Prüfe insbesondere auch die Ordner ue02, ue03 und ue04. Nenne die wichtigsten Dateien und ihren Zweck."

So answer: yes, now verified comprehensively. Present a complete inventory with purpose. Include:
- Top-level: README.md, AGENTS.md, .git (version control).
- ue01: README, steckbriefe/ with 149 profiles + _vorlage + _beispiel.
- ue02: README, _vorlage (notiz, spezifikation), _zugabe (rollen), 108 student dirs.
- ue03: README, _vorlage (kontext, anforderungen), 95 dirs.
- ue04: README, _vorlage/einrichtung.md, farooqfrankfurt-gif/einrichtung.md (untracked, identical to template).
- No hidden files, no non-md files, no nested dirs.
- Anomalies found: ue02/mk only phasenplan.md; 5 dirs missing phasenplan; ue03/mskk15 missing zuordnung; ue04 abgabe still empty template, sitzung.md missing.

Also maybe note ue01 has 149 profiles while ue02 108 and ue03 95 — repo grows per exercise, normal.

I should be honest: in my first pass I looked at the top level and READMEs, plus counts and a sample folder, but not every single student folder. Now I checked all. So answer "Ja, jetzt vollständig" and describe what the check covered.

Format: concise German, with structure and a table of most important files. Avoid dumping 300 filenames. Mention 781 tracked + 1 untracked.

Let me double check whether ue01/steckbriefe contains only files (no dirs) — earlier find showed flat. Fine.

One more check: are there student folders in ue02 that are empty? No, mk has phasenplan. Fine.

Also check whether ue03/mskk15 has other files. Not needed.

Let me write the answer.

Ja — jetzt vollständig. Meine erste Antwort stützte sich auf die oberste Ebene, die `README.md`-Dateien, Zählungen und ein Beispielverzeichnis. Ich habe deshalb alle Übungsordner einzeln nachgeprüft: jede Datei, jede Unterebene, versteckte Dateien, Nicht-Markdown-Dateien und den Git-Status.

## Prüfergebnis vorab

- **Keine versteckten Dateien** außer `.git/` (kein `.gitignore`, kein `.github/`, keine Workflows).
- **Keine Nicht-Markdown-Dateien**: alle 781 getrackten Dateien sind `.md`.
- **Keine verschachtelten Unterordner** in `ue01`–`ue04`; die Abgaben liegen flach in `ueNN/<benutzername>/`.
- **Genau eine unversionierte Datei**: `ue04/farooqfrankfurt-gif/einrichtung.md` (deine Abgabe).
- Vorlagen-Ordner heißen einheitlich `_vorlage` bzw. `_zugabe` und liegen nur auf Übungsebene.

## Wichtigste Dateien und ihr Zweck

### Wurzel

| Datei | Zweck |
|---|---|
| `README.md` | Gesamtüberblick: Aufbau, Einreichungsweg (Fork → Branch → PR), Spielregeln |
| `AGENTS.md` | Regeln für KI-Agenten (deutsch, nur eigene Dateien, nicht auf `main`, nichts Persönliches) |
| `.git/` | Versionsverwaltung; aktueller Branch `ue04-farooqfrankfurt-gif` |

### `ue01/` — Git und GitHub

| Datei/Ordner | Zweck |
|---|---|
| `README.md` | Aufgabe: Steckbrief als PR von `steckbrief-<benutzername>` |
| `steckbriefe/_vorlage.md` | Leere Vorlage (Studiengang, Vorerfahrung, Erwartungen) |
| `steckbriefe/_beispiel.md` | Ausgefülltes Muster |
| `steckbriefe/<benutzername>.md` | **149** abgegebene Steckbriefe |

### `ue02/` — Projektmodell am Fall „Terminplaner“

| Datei/Ordner | Zweck |
|---|---|
| `README.md` | Aufgabe: Verzeichnis `ue02/<benutzername>/` mit drei Dateien |
| `_vorlage/notiz.md` | Unformatierte Gesprächsnotiz → in Markdown bringen (Aufgabe 1) |
| `_vorlage/spezifikation.md` | Gliederung einer Spezifikation mit Beispielen (Aufgabe 3) |
| `_zugabe/rollen.md` | Freiwillige Aufgabe 5: Kunde, Projektteam, drei Situationen |
| `<benutzername>/notiz.md` | Formatierte Gesprächsnotiz (107×) |
| `<benutzername>/phasenplan.md` | Tätigkeiten den Projektphasen zugeordnet, im Übungsblatt erstellt (103×) |
| `<benutzername>/spezifikation.md` | Spezifikationsgliederung (107×) |
| `<benutzername>/rollen.md` | Optionale Rollenbesetzung (18×) |

Insgesamt **108 Abgabeverzeichnisse**.

### `ue03/` — Anforderungen

| Datei/Ordner | Zweck |
|---|---|
| `README.md` | Aufgabe: Verzeichnis `ue03/<benutzername>/` mit drei Dateien |
| `_vorlage/kontext.md` | Stakeholder (mind. sechs) und Systemkontext (Aufgabe 1) |
| `_vorlage/anforderungen.md` | Eigene Anforderungen A01… mit Stakeholder und Art FA/QA/RB (Aufgabe 3) |
| `<benutzername>/kontext.md` | Ausgefüllter Kontext (95×) |
| `<benutzername>/zuordnung.md` | Anforderung oder Lösung?, im Übungsblatt erstellt (94×) |
| `<benutzername>/anforderungen.md` | Eigene Anforderungen (95×) |

Insgesamt **95 Abgabeverzeichnisse**.

### `ue04/` — Coding Agent

| Datei/Ordner | Zweck |
|---|---|
| `README.md` | Aufgabe: `ue04/<benutzername>/` mit `einrichtung.md` und `sitzung.md` |
| `_vorlage/einrichtung.md` | Erfassung von Werkzeug, Version, OS, Modellzugang, Modell; Prüfung der Agentenantwort; Fehlerbeleg bei „teilweise/nein“ |
| `farooqfrankfurt-gif/einrichtung.md` | **Deine Abgabe** – noch unverändert identisch mit der Vorlage, alle Felder `…` |

## Auffälligkeiten in den Abgaben

- `ue02/mk/` enthält **nur** `phasenplan.md`; `notiz.md` und `spezifikation.md` fehlen.
- `phasenplan.md` fehlt außerdem bei `jvng`, `skt435`, `ssda78`, `ssng61`, `ysbi82`.
- `ue03/mskk15/` fehlt `zuordnung.md`.
- In `ue01/steckbriefe/` gibt es Dateien mit Großbuchstaben (`AR.md`, `Fahm.md`, `TariqK2004.md` …), obwohl die README Kleinbuchstaben verlangt.

Für deine eigene Übung 4 heißt das: `einrichtung.md` ist noch nicht ausgefüllt, und `sitzung.md` fehlt – beides entsteht laut `ue04/README.md` erst im Lauf der Übung.
