# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e5e7e4bdcffe5y3Q3Bkbl7TN7J
**Created:** 11/3/2026, 2:03:14 PM
**Updated:** 11/3/2026, 2:03:40 PM

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

The user asks: "What's in this repository, and which files are mine?" I need to explore. Also need to check git branch, user's branch, directories.

Let me explore the repo.

Ich schaue mir zuerst die Struktur, den aktuellen Branch und die Git-Historie an.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current; git status --short; git log --oneline -15"
}
```

ue04-1lawand
?? ue04/1lawand/
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
5ae12b6 Übung 2: Ergebnisse von thng (#279)
78dd5f7 Ue02 div (#278)
b049c60 Übung 2: Ergebnisse von jsug (#277)
d7dc0ea Übung 2 - Ergebnisse von Jemy  (#276)
8768bd6 Abschnitt 2 wurde erneut auf github gemacht (#282)


**Tool: read**

**Input:**
```json
{
  "path": ".../README.md"
}
```

Read file .../README.md, lines 1-74
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

Current branch ue04-1lawand, and untracked ue04/1lawand/. Need to see what's in repo, and which files are from this user. Let's list directories and see ue01/1lawand, ue02/1lawand etc. Also check git log for user commits.

**Tool: shell**

**Input:**
```json
{
  "command": "ls -1; echo \"---\"; for d in ue01 ue02 ue03 ue04; do echo \"$d:\"; ls -1 \"$d\" 2>/dev/null; done"
}
```

AGENTS.md
README.md
ue01
ue02
ue03
ue04
---
ue01:
README.md
steckbriefe
ue02:
_vorlage
_zugabe
aayd
abdu113
af
agbr
Agub
ahyi
akyf
anas23088
anddun
andel0
anpa
anushka
athr
avon507
ayue
bblj09
bima
datr03
div
dlm28
dmmh1710
dsc
dsch
dszp
emrano
en7-mj
ezen
fahm
flk
fortnitepro
hams
hfdr12
iaa
iesp
ilias04j
ivlbs
IY69
janp
javu11
jemy
jp26
jsug
jvng
kraz
lebr
lom
Lpr
mabl
masalabyte
maxbarrosschauer
mbgrn04
mduc
meq
mf23
mjab
mjas
mk
mkon
mpal
mu
mw
my55
ngh
nicolino
nko
nly50
NN
nohl
NUAli
oubou
pdam
pgml
pz01
qdb
qho
README.md
real
renn
sahmad
sahmed
sam
skrl78
skt435
snab
sngu
ssda78
sshj44
ssng61
stmx
talh
TariqK2004
tcam
thm-nos
thng
tiger
tnd
tngan
trry
ttpr21
tyfncc
uwar
vic26
virus
wnga
ygue
ysbi82
zcbn
zcoel
zsh
ue03:
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
azm96
bblj09
bogh233
cms
davn68
dlm28
dmmh1710
dsch
ecib
emrano
en7-mj
ezen
fahm
flk
hfdr12
iaa
ilias04j
IY69
janp
javu
jemy
jsug
jvng
kraz
lkrs
lom
Lpr
masalabyte
maxbarrosschauer
mduc
meq
mjab
MK
mken
mkon
moh
mpal
mskk15
mu
mw
my55
nicolino
nko
nly50
NN
nohl
NUAli
onzj
oubou
pdam
pgml
pz01
qho
README.md
real
sahmad
sahmed
sam
skrl78
snab
sngu
sraks
ssda78
sshj44
stmx
talh
TariqK2004
tcam
tiger
tnd
trry
tyfncc
uwar
val
vic26
virus
wnga
ygue
ykar
z-266
zc
zcbn
zcoel
zsh
ue04:
_vorlage
1lawand
README.md


**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline --author=\"$(git config user.name)\" -20; echo \"--- alle Commits mit 1lawand im Branch ---\"; git log --oneline --all -- . ':(exclude)ue04/1lawand' | head -5; echo \"--- untracked ---\"; find ue04/1lawand -type f 2>/dev/null"
}
```

--- alle Commits mit 1lawand im Branch ---
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)
--- untracked ---
ue04/1lawand/einrichtung.md


---

## Assistant

_Thinking:_

Interesting: git log --author returned nothing? The output starts with "--- alle Commits..." meaning first command empty. So local branch has no commits authored by user.name? Maybe user.name config differs. Let's check git config, and check if ue01/1lawand or ue02/1lawand exist. In ue01 there's steckbriefe; need check. Let's look.

Branch ue04-1lawand, so username likely "1lawand". But ue01/ue02/ue03 directories don't show 1lawand. Maybe a different abbreviation previously. Let's check ue01/steckbriefe, and whether any commits by the user exist across all branches. Also check git config, remotes, and README of ue04 and _vorlage.

**Tool: shell**

**Input:**
```json
{
  "command": "git config user.name; git config user.email; echo \"--- branches ---\"; git branch -a; echo \"--- Steckbriefe ---\"; ls -1 ue01/steckbriefe | head -40; echo \"--- Treffer 1lawand im Repo ---\"; grep -ril \"1lawand\" --exclude-dir=.git . | head -20"
}
```

Lawand Omar 
...
--- branches ---
  main
  steckbrief-lom
  ue02-lom
  ue03-lom
* ue04-1lawand
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/steckbrief-lom
  remotes/origin/ue02-lom
  remotes/origin/ue02-lom-korrektur
  remotes/origin/ue03-lom
--- Steckbriefe ---
_beispiel.md
_vorlage.md
aalg.md
aayd.md
adni.md
AF.md
agbr.md
Agub.md
ahyi.md
akyf.md
ale563.md
Anas23088.md
anddun.md
andel0.md
anpa.md
anushka.md
AR.md
asi.md
asng24.md
athr.md
avon507.md
Aza.md
azm96.md
Bblj09.md
bima.md
bunter95.md
cms.md
datr03.md
davn68.md
dhfn1611.md
div.md
dlm28.md
dmal2004.md
dmmh1710.md
dsc.md
dsch.md
dszp.md
ecib.md
ekes.md
emalj.md
--- Treffer 1lawand im Repo ---
./ue02/lom/spezifikation.md


**Tool: shell**

**Input:**
```json
{
  "command": "cat ue04/README.md; echo \"=== VORLAGE ===\"; find ue04/_vorlage -type f | head; echo \"=== einrichtung.md ===\"; cat ue04/1lawand/einrichtung.md"
}
```

# Übung 4 — Einen Coding Agent einrichten

In dieser Übung installieren Sie einen Coding Agent — das Übungsblatt
beschreibt opencode —, verbinden ihn mit einem Sprachmodell und setzen ihn
zum ersten Mal in Ihrem lokalen Klon dieses Repositorys ein. Die Aufgaben stehen im
[Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue04-coding-agent/).

## Was Sie einreichen

Einzureichen ist ein Verzeichnis `ue04/<benutzername>/` mit zwei Dateien,
und zwar als Pull Request vom Branch `ue04-<benutzername>`. Gemeint ist Ihr
GitHub-Benutzername in Kleinbuchstaben.

| Datei | Aufgabe | Woher |
|---|---|---|
| `einrichtung.md` | 1 und 2 — womit Sie arbeiten, und ob die Antwort des Agenten stimmt | aus `_vorlage/` |
| `sitzung.md` | 2 — die Sitzung mit dem Agenten | entsteht mit `/export` in Ihrem Agenten |

1. Kopieren Sie das Verzeichnis `_vorlage` nach `<benutzername>`. Die Vorlage
   selbst bleibt unverändert.
2. Füllen Sie `einrichtung.md` im Lauf der Übung aus und legen Sie
   `sitzung.md` hinzu. Entfernen Sie dort vor dem Commit Pfade mit dem
   Namen Ihres Kontos auf dem Rechner, Namen und E-Mail-Adressen; das
   Repository ist öffentlich.

Läuft Ihr Agent nicht, reichen Sie trotzdem ein: nur
`einrichtung.md`, mit *nein* oder *teilweise* bei „Läuft der Agent?“ und
einem Beleg im Abschnitt „Wenn es nicht läuft“ — Schritt, Befehl samt Ausgabe (wörtlich)
und was Sie bereits versucht haben.

Das Übungsblatt beschreibt opencode, schreibt es aber nicht vor. Wer schon
mit einem anderen Agenten arbeitet — Claude Code, Codex, GitHub Copilot in
VS Code oder als Copilot CLI, eine andere Erweiterung —, darf ihn verwenden
und trägt ihn in `einrichtung.md` unter „Werkzeug“ ein.

Weitere Dateien, welche der Agent anlegt, gehören nicht in den Pull Request.

> [!IMPORTANT]
> Für diese Übung gibt es 1 Bonuspunkt. Diesen erhält nur, wer bis zur
> Frist im Moodle-Kurs selbst einen Pull Request mit Inhalten gestellt hat.
=== VORLAGE ===
ue04/_vorlage/einrichtung.md
=== einrichtung.md ===
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


---

## Assistant

_Thinking:_

The user is "lom" (based on branches steckbrief-lom, ue02-lom, ue03-lom) and GitHub username? Branch ue04-1lawand suggests GitHub username "1lawand". But earlier dirs are lom. Let's confirm README AGENTS says older dirs can carry earlier chosen abbreviation. Need identify user's files. Let's inspect commits by author.

git log --author returned nothing because maybe commits authored with different name/email. Let's search commits touching ue01/steckbriefe/lom.md, ue02/lom, ue03/lom. And check git log for branch.

**Tool: shell**

**Input:**
```json
{
  "command": "ls ue01/steckbriefe | grep -i '^lom'; echo \"--- ue02/lom ---\"; find ue02/lom -type f; echo \"--- ue03/lom ---\"; find ue03/lom -type f; echo \"--- ue04 ---\"; find ue04/1lawand -type f"
}
```

lom.md
--- ue02/lom ---
ue02/lom/spezifikation.md
ue02/lom/notiz.md
ue02/lom/phasenplan.md
--- ue03/lom ---
ue03/lom/zuordnung.md
ue03/lom/kontext.md
ue03/lom/anforderungen.md
--- ue04 ---
ue04/1lawand/einrichtung.md


**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline --all -- ue01/steckbriefe/lom.md ue02/lom ue03/lom ue04/1lawand; echo \"--- Autoren dieser Dateien ---\"; git log --format='%h %an <%ae> %s' --all -- ue01/steckbriefe/lom.md ue02/lom ue03/lom | cat"
}
```

8cfd580 Übung 2: Formatierung der Gesprächsnotiz korrigiert (#286)
1975b93 ue03: Abgabe lom (#303)
b44a300 ue03: Kontext und Zuordnung für lom ergänzen
38a5920 ue03: Anforderungen für lom ergänzen
7d760c7 Übung 2: Formatierung der Gesprächsnotiz korrigiert
0602364 Übung 2: Formatierung der Gesprächsnotiz korrigiert
20cfbbc Übung 2: Gesprächsnotiz erstellt (#143)
f200e6f Steckbrief lom hinzufügen (#59)
d4b4a2a Steckbrief an die vorgesehene Stelle legen
f31b3fc Aufgabe 3: Spezifikation erstellt
88bacee Remove template comment from notiz.md
8a728ed Add phase plan for exercise 2
1994942 Übung 2: Gesprächsnotiz erstellt
--- Autoren dieser Dateien ---
8cfd580 1Lawand <......> Übung 2: Formatierung der Gesprächsnotiz korrigiert (#286)
1975b93 1Lawand <......> ue03: Abgabe lom (#303)
b44a300 Lawand Omar <...> ue03: Kontext und Zuordnung für lom ergänzen
38a5920 Lawand Omar <...> ue03: Anforderungen für lom ergänzen
7d760c7 1Lawand <......> Übung 2: Formatierung der Gesprächsnotiz korrigiert
0602364 1Lawand <......> Übung 2: Formatierung der Gesprächsnotiz korrigiert
20cfbbc 1Lawand <......> Übung 2: Gesprächsnotiz erstellt (#143)
f200e6f 1Lawand <......> Steckbrief lom hinzufügen (#59)
d4b4a2a Carsten Lucke <...> Steckbrief an die vorgesehene Stelle legen
f31b3fc Lawand Omar <...> Aufgabe 3: Spezifikation erstellt
88bacee Lawand Omar <...> Remove template comment from notiz.md
8a728ed Lawand Omar <...> Add phase plan for exercise 2
1994942 Lawand Omar <...> Übung 2: Gesprächsnotiz erstellt


---

## Assistant

_Thinking:_

So user's files: ue01/steckbriefe/lom.md, ue02/lom/*, ue03/lom/*, ue04/1lawand/einrichtung.md (untracked, incomplete template). Need maybe overview of repo content. Let's read ue01 README, ue02 README, ue03 README briefly to summarize what's in repo. Also maybe count of submissions. Let's check READMEs.

**Tool: shell**

**Input:**
```json
{
  "command": "for f in ue01/README.md ue02/README.md ue03/README.md; do echo \"=== $f ===\"; sed -n '1,40p' \"$f\"; done"
}
```

=== ue01/README.md ===
# Übung 1 — Erste Schritte mit Git und GitHub

In dieser Übung gehen Sie den Weg einer Änderung einmal vollständig: vom
eigenen Rechner bis in dieses Repository. Die Anleitung steht im
[Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/).

## Was Sie einreichen

Einzureichen ist Ihr Steckbrief als Datei `steckbriefe/<benutzername>.md`,
und zwar als Pull Request vom Branch `steckbrief-<benutzername>`. Gemeint
ist Ihr GitHub-Benutzername in Kleinbuchstaben.

1. Kopieren Sie `steckbriefe/_vorlage.md` nach
   `steckbriefe/<benutzername>.md` und ersetzen Sie in der Überschrift
   `<benutzername>` durch Ihren GitHub-Benutzernamen in Kleinbuchstaben. Die
   Vorlage selbst bleibt unverändert.
2. Füllen Sie die drei Abschnitte aus — im Lauf der Übung einen nach dem
   anderen, jeweils als eigenen Commit.

`steckbriefe/_beispiel.md` zeigt, wie ein ausgefüllter Steckbrief aussehen kann.

Für den rechtzeitig gestellten Pull Request gibt es Bonuspunkte; die
Bedingungen stehen im Übungsblatt.
=== ue02/README.md ===
# Übung 2 — Das Projektmodell am Fall

In dieser Übung schreiben Sie Markdown und wenden das Projektmodell auf
einen konkreten Fall an, d.h. auf einen Terminplaner für die THM. Die
Aufgaben stehen im
[Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue02-projektmodell/).

## Was Sie einreichen

Einzureichen ist ein Verzeichnis `ue02/<benutzername>/` mit drei Dateien,
und zwar als Pull Request vom Branch `ue02-<benutzername>`. Gemeint ist Ihr
GitHub-Benutzername in Kleinbuchstaben.

| Datei | Aufgabe | Woher |
|---|---|---|
| `notiz.md` | 1 — eine Gesprächsnotiz in Markdown bringen | aus `_vorlage/` |
| `phasenplan.md` | 2 — Tätigkeiten den Phasen zuordnen | entsteht im Übungsblatt und wird dort heruntergeladen |
| `spezifikation.md` | 3 — Gliederung einer Spezifikation | aus `_vorlage/` |
| `rollen.md` | 5 — Zugabe, freiwillig: Rollen besetzen | aus `_zugabe/` |

1. Kopieren Sie das Verzeichnis `_vorlage` nach `<benutzername>`. Die Vorlage
   selbst bleibt unverändert.
2. Bearbeiten Sie die Dateien im Lauf der Übung und legen Sie
   `phasenplan.md` hinzu.

Die Aufgaben 3 und 5 bearbeiten Sie allein oder in einer Gruppe bis vier
Personen. Im Kopf von `spezifikation.md` und `rollen.md` stehen die
GitHub-Benutzernamen aller Personen, die mitgearbeitet haben.

> [!IMPORTANT]
> Für diese Übung gibt es 1 Bonuspunkt. Diesen erhält nur, wer bis zur
> Frist im Moodle-Kurs selbst einen Pull Request mit Inhalten gestellt hat.
> Daher reicht jedes Mitglied einer Gruppe selbst ein: Es legt die gemeinsamen
> Dateien in seinem eigenen Verzeichnis ab, überträgt sie in seinen eigenen
> Fork und stellt einen eigenen Pull Request. Die Benutzernamen im Kopf der
> Dateien ergänzen dies lediglich.
=== ue03/README.md ===
# Übung 3 — Anforderungen an den Terminplaner

In dieser Übung bestimmen Sie Stakeholder und Systemkontext des Terminplaners
für die THM, unterscheiden Anforderungen von Lösungen und formulieren eigene
Anforderungen. Die Aufgaben stehen im
[Übungsblatt](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue03-anforderungen/).

## Was Sie einreichen

Einzureichen ist ein Verzeichnis `ue03/<benutzername>/` mit drei Dateien,
und zwar als Pull Request vom Branch `ue03-<benutzername>`. Gemeint ist Ihr
GitHub-Benutzername in Kleinbuchstaben.

| Datei | Aufgabe | Woher |
|---|---|---|
| `kontext.md` | 1 — Stakeholder und Systemkontext | aus `_vorlage/` |
| `zuordnung.md` | 2 — Anforderung oder Lösung? | entsteht im Übungsblatt und wird dort heruntergeladen |
| `anforderungen.md` | 3 — Eigene Anforderungen | aus `_vorlage/` |

1. Kopieren Sie das Verzeichnis `_vorlage` nach `<benutzername>`. Die Vorlage
   selbst bleibt unverändert.
2. Bearbeiten Sie die Dateien im Lauf der Übung und legen Sie
   `zuordnung.md` hinzu.

Alle Aufgaben bearbeiten Sie allein. Ihre Gesprächsnotiz aus Übung 2 lesen
Sie nur; ändern Sie dort nichts.

> [!IMPORTANT]
> Für diese Übung gibt es 1 Bonuspunkt. Diesen erhält nur, wer bis zur
> Frist im Moodle-Kurs selbst einen Pull Request mit Inhalten gestellt hat.


**Tool: shell**

**Input:**
```json
{
  "command": "echo \"Steckbriefe: $(ls ue01/steckbriefe/*.md | wc -l)\"; echo \"ue02-Abgaben: $(find ue02 -mindepth 1 -maxdepth 1 -type d ! -name '_*' | wc -l)\"; echo \"ue03-Abgaben: $(find ue03 -mindepth 1 -maxdepth 1 -type d ! -name '_*' | wc -l)\"; echo \"--- git status ---\"; git status"
}
```

Steckbriefe:      151
ue02-Abgaben:      108
ue03-Abgaben:       95
--- git status ---
On branch ue04-1lawand
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	ue04/1lawand/

nothing added to commit but untracked files present (use "git add" to track)


---

## Assistant

_Thinking:_

I now can answer. Need be careful about privacy: user's own name/email is in repo? AGENTS says don't include Klarnamen/email in files/commits, but in the answer to the user? It says "In Dateien und Commit-Nachrichten gehören keine Klarnamen..." Answer isn't a file. Still, better avoid displaying email. But mention there is an email in git history? Actually git config email differs from commit author. Not necessary. Could mention commits under "1Lawand" and "Lawand Omar" — that's personal name but the user knows. Maybe avoid repeating full name, just GitHub username 1lawand.

Need note the branch is ue04-1lawand (not main) so fine. Untracked ue04/1lawand/einrichtung.md is still the template, not filled in. Also there is no sitzung.md yet.

Should I mention that ue02/lom and ue03/lom use older abbreviation "lom", which per AGENTS belongs to them, and ue04 begins with 1lawand. The user asked which files are mine. Let me list exactly.

Could check whether lom.md and files are tracked/clean, yes git status only untracked ue04. Let's maybe check content briefly to characterize? Maybe not needed but useful to summarize. Let's read headings of user's files to describe.

**Tool: shell**

**Input:**
```json
{
  "command": "for f in ue01/steckbriefe/lom.md ue02/lom/notiz.md ue02/lom/phasenplan.md ue02/lom/spezifikation.md ue03/lom/kontext.md ue03/lom/zuordnung.md ue03/lom/anforderungen.md; do echo \"=== $f ===\"; grep -m 8 '^#' \"$f\"; done"
}
```

=== ue01/steckbriefe/lom.md ===
# Mein Steckbrief
=== ue02/lom/notiz.md ===
# Gesprächsnotiz: Terminplaner für die THM
## Worum es geht
## Was heute benutzt wird
## Nächste Schritte
## Offene Punkte
=== ue02/lom/phasenplan.md ===
# Phasenplan — Terminplaner für die THM
## Studie
## Systemspezifikation
## Systemkonstruktion
## Implementierung
## Integration & Einführung
## Wartung
## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?
=== ue02/lom/spezifikation.md ===
# Spezifikation des Terminplaners – Gliederung und Beispiele
## 1. Ziel und Zweck des Systems
## 2. Benutzer und Rollen
## 3. Funktionale Anforderungen
## 4. Nichtfunktionale Anforderungen
## 5. Daten und Informationsmodell
## 6. Benutzeroberfläche
## 7. Schnittstellen zu anderen Systemen
=== ue03/lom/kontext.md ===
# Stakeholder und Systemkontext — Terminplaner für die THM
## Stakeholder
## Systemkontext
## Irrelevante Umgebung
=== ue03/lom/zuordnung.md ===
# Anforderung oder Lösung? — Terminplaner für die THM
## Funktionale Anforderung (FA)
## Qualitätsanforderung (QA)
## Randbedingung (RB)
## Keine Anforderung — Lösung (WIE)
## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?
=== ue03/lom/anforderungen.md ===
# Anforderungen – Terminplaner der THM
## Implizite Anforderung


---

## Assistant

_Thinking:_

Now compose German answer concise. Include repo structure and "welche Dateien von mir". Mention identity mapping: branch ue04-1lawand and GitHub username 1lawand; earlier lom directories. Note ue04 file is still template. Note current branch not main.

Potential nuance: Is "1lawand" definitely GitHub username? Branch ue04-1lawand, dir ue04/1lawand. Yes. And prior "lom" abbreviation. AGENTS says older directories can carry earlier chosen abbreviation; they belong to person.

Maybe mention commits show author names (1Lawand / Lawand Omar) — avoid. Also user's files are tracked and clean, except new untracked.

Let me also note counts. Could mention 151 Steckbriefe, 108/95 submissions. But "Was liegt in diesem Repository" – summary of exercises suffices, maybe counts nice.

Should not push/commit. No changes made.

## Was im Repository liegt

Das ist das Übungsrepository **Softwaretechnik** der THM (Campus Friedberg). Es wächst mit jeder Übung und enthält je ein Verzeichnis mit eigener `README.md`:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | Steckbriefe der Studierenden (`ue01/steckbriefe/`, 151 Dateien) |
| `ue02/` | Projektmodell am Fall „Terminplaner“ (`ue02/<name>/`, 108 Abgaben) |
| `ue03/` | Anforderungen an den Terminplaner (`ue03/<name>/`, 95 Abgaben) |
| `ue04/` | Einrichtung eines Coding Agenten (`ue04/<name>/`, aktuell nur Vorlage und deine Abgabe) |

Dazu kommen `README.md`, `AGENTS.md` sowie die Vorlagen `_vorlage/`, `_zugabe/` und Beispiel-Dateien (Namen mit `_`).

Aktueller Branch: **`ue04-1lawand`** (nicht `main`). Arbeitsstand ist sauber, nur dein neues Verzeichnis ist noch untracked.

## Deine Dateien

Du arbeitest unter dem GitHub-Benutzernamen **`1lawand`**. Die älteren Abgaben liegen noch unter dem früheren Kürzel **`lom`** – laut `AGENTS.md` gehören diese Verzeichnisse trotzdem dir:

- `ue01/steckbriefe/lom.md` — dein Steckbrief
- `ue02/lom/notiz.md` — Gesprächsnotiz zum Terminplaner
- `ue02/lom/phasenplan.md` — Zuordnung der Tätigkeiten zu den Phasen
- `ue02/lom/spezifikation.md` — Gliederung der Spezifikation
- `ue03/lom/kontext.md` — Stakeholder und Systemkontext
- `ue03/lom/zuordnung.md` — Anforderung oder Lösung?
- `ue03/lom/anforderungen.md` — eigene Anforderungen
- `ue04/1lawand/einrichtung.md` — **neu und noch unbearbeitet**: Die Datei enthält derzeit nur den unveränderten Text aus `ue04/_vorlage/`. `sitzung.md` fehlt noch.

Die Git-Historie bestätigt das: Commits zu `lom.md`, `ue02/lom/` und `ue03/lom/` stammen von dir (GitHub-Nutzername `1Lawand`).

Alles andere im Repository gehört anderen Studierenden bzw. der Lehrveranstaltung und bleibt unberührt.
