# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e5e3ca0fbffegg1IDGFAhKqmzz
**Created:** 11/3/2026, 3:14:58 PM
**Updated:** 11/3/2026, 3:15:21 PM

---

## User

Was liegt in diesem Repository und welche Dateien stammen von mir?

---

## Assistant

I'll start by checking the repository state and structure.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current && git status --short && git log --oneline -10"
}
```

main
?? ue04/52yuyu/
00d88ac Merge branch 'carstenlucke:main' into main
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)
8cfd580 Übung 2: Formatierung der Gesprächsnotiz korrigiert (#286)
baaa2b8 Ergebnisse der Phasen ergänzt in phasenplan.md (#284)
c55409f Übung 2 : Ergebnisse von akyf (#283)
9db8067 Ue02 zsh (#281)


**Tool: read**

**Input:**
```json
{
  "path": "/Users/52younes/Steckbrief-ygue"
}
```

Read directory /Users/52younes/Steckbrief-ygue, entries 1-7
.git/
ue01/
ue02/
ue03/
ue04/
AGENTS.md
README.md

---

## Assistant

_Thinking:_

We're on main. Per AGENTS.md, nothing should be changed on main. The user is asking a read-only question, which is fine.

There's an untracked directory ue04/52yuyu/ — likely the user's. Let me look at the structure.

Ich schaue mir die Struktur genauer an — insbesondere die Übungsverzeichnisse und das untracked Verzeichnis.

**Tool: read**

**Input:**
```json
{
  "path": "/Users/52younes/Steckbrief-ygue/README.md"
}
```

Read file /Users/52younes/Steckbrief-ygue/README.md, lines 1-74
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

**Tool: read**

**Input:**
```json
{
  "path": "/Users/52younes/Steckbrief-ygue/ue04"
}
```

Read directory /Users/52younes/Steckbrief-ygue/ue04, entries 1-3
_vorlage/
52yuyu/
README.md

**Tool: read**

**Input:**
```json
{
  "path": "/Users/52younes/Steckbrief-ygue/ue04/52yuyu"
}
```

Read directory /Users/52younes/Steckbrief-ygue/ue04/52yuyu, entries 1-1
einrichtung.md

---

## Assistant

_Thinking:_

Let me look at the ue04 README, the template, and the einrichtung.md. Also check git config user, branches, remotes to determine identity. Careful with personal info in output.

Let me also check each ue directory for a 52yuyu folder.

**Tool: shell**

**Input:**
```json
{
  "command": "for d in ue01 ue02 ue03 ue04; do echo \"== $d\"; ls -1 \"$d\"; done"
}
```

== ue01
README.md
steckbriefe
== ue02
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
== ue03
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
== ue04
_vorlage
52yuyu
README.md


**Tool: read**

**Input:**
```json
{
  "path": "/Users/52younes/Steckbrief-ygue/ue04/README.md"
}
```

Read file /Users/52younes/Steckbrief-ygue/ue04/README.md, lines 1-40
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

**Tool: read**

**Input:**
```json
{
  "path": "/Users/52younes/Steckbrief-ygue/ue04/52yuyu/einrichtung.md"
}
```

Read file /Users/52younes/Steckbrief-ygue/ue04/52yuyu/einrichtung.md, lines 1-23
1: # Einrichtung Coding Agent – Übung 4
2: 
3: ## Aufbau
4: 
5: | Frage / Eigenschaft | Antwort / Wert |
6: | :--- | :--- |
7: | **Werkzeug** | opencode (CLI Agent) |
8: | **Modellzugang** | OpenCode Zen (DeepSeek V4.1 Flash Free) |
9: | **Läuft der Agent?** | ja |
10: 
11: ## Antworten zu den Kontrollfragen
12: 
13: 1. **Was prüft `opencode --version`, was prüft „Sag Hallo und nenne dein Modell.“ – und warum genügt das eine nicht ohne das andere?**
14:    * `opencode --version` prüft nur, ob das CLI-Werkzeug auf dem Rechner lokal installiert ist[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span).
15:    * „Sag Hallo...“ prüft die Netzwerkverbindung, Authentifizierung und Erreichbarkeit des Sprachmodells im Backend[span_8](start_span)[span_8](end_span)[span_9](start_span)[span_9](end_span).
16:    * Beides ist nötig: Ein installiertes Tool ohne Modellverbindung funktioniert nicht, und ein erreichbares Modell bringt nichts ohne das CLI-Werkzeug[span_10](start_span)[span_10](end_span)[span_11](start_span)[span_11](end_span).
17: 
18: 2. **Warum lässt sich opencode mit Modellen ganz verschiedener Anbieter betreiben?**
19:    * Weil `opencode` entkoppelt konzipiert ist[span_12](start_span)[span_12](end_span)[span_13](start_span)[span_13](end_span). Es nutzt einheitliche API-Schnittstellen, um Prompts an beliebige LLM-Anbieter (OpenAI, Anthropic, OpenCode Zen etc.) zu senden und die Antworten lokal im Repository zu verarbeiten[span_14](start_span)[span_14](end_span)[span_15](start_span)[span_15](end_span).
20: 
21: 3. **Wer ein Claude-Abo hat, kann damit in opencode nicht arbeiten. Was spräche dagegen, stattdessen einen API-Schlüssel zu nehmen?**
22:    * **Abo:** Nutzungsbedingungen von Anthropic verbieten die Verwendung des Web-/App-Abos in Dritthersteller-Tools[span_16](start_span)[span_16](end_span).
23:    * **API-Schlüssel:** Rechnet strikt nach Token-Verbrauch ab[span_17](start_span)[span_17](end_span). Da Agenten bei jeder Aktion große Teile des Projektkontextes mitsenden, können die Kosten schnell sehr hoch werden im Vergleich zu einer Flatrate[span_18](start_span)[span_18](end_span).

---

## Assistant

_Thinking:_

The user's directory appears to be ue04/52yuyu/ — likely their GitHub username is 52yuyu. Let me confirm: git config user.name/email, remotes, branches. Also check whether "52yuyu" or "ygue" appears in other ue directories. The repo folder is Steckbrief-ygue — ygue exists in ue02 and ue03! The local account name is "52younes". Hmm. So which is the user's? AGENTS.md says: older directories may carry an earlier-chosen abbreviation; they still belong to that person. Is unclear → ask.

There's ue02/ygue and ue03/ygue. And the untracked ue04/52yuyu. The folder name Steckbrief-ygue suggests GitHub username "ygue". But ue04 dir is 52yuyu, which may be a wrong/other username. Actually maybe 52yuyu is a typo attempt. Need to check git remote and config.

Let me gather evidence: remote URL, git config, contents of ue02/ygue and ue03/ygue, and git log for authors.

**Tool: shell**

**Input:**
```json
{
  "command": "git remote -v; echo \"-- config\"; git config user.name; git config user.email; echo \"-- branches\"; git branch -a | head -20; echo \"-- ue02/ygue\"; ls -1 ue02/ygue 2>/dev/null; echo \"-- ue03/ygue\"; ls -1R ue03/ygue 2>/dev/null"
}
```

origin	https://github.com/52yuyu/Steckbrief-ygue.git (fetch)
origin	https://github.com/52yuyu/Steckbrief-ygue.git (push)
upstream	https://github.com/carstenlucke/thm_wk-1208_softwaretechnik-uebungen.git (fetch)
upstream	https://github.com/carstenlucke/thm_wk-1208_softwaretechnik-uebungen.git (push)
-- config
-- branches
* main
  ue02-ygue
  ue03-ygue
  uebung1
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/ue02-ygue
  remotes/origin/ue03-ygue
  remotes/origin/uebung1
  remotes/origin/Übung1
  remotes/upstream/HEAD -> upstream/main
  remotes/upstream/main
  remotes/upstream/steckbrief-clu
-- ue02/ygue
notiz.md
phasenplan.md
spezifikation.md
-- ue03/ygue
anforderungen.md
kontext.md
zuordnung.md


**Tool: shell**

**Input:**
```json
{
  "command": "git log --format='%h %an <%ae> %s' -3; echo \"-- commits touching ygue\"; git log --oneline -- ue02/ygue ue03/ygue | head -10"
}
```

00d88ac 52yuyu <younes.guerinat@mnd.thm.de> Merge branch 'carstenlucke:main' into main
b5dbd3a THM-Nos <nossair.belhaj@mnd.thm.de> Ü2: Ergebnisse von thm-nos (#400)
122ab21 Nathan <nathan.ghebretensae@mnd.thm.de> Ergebnisse der Phasen ergänzen (#396)
-- commits touching ygue
a5ce6a5 Ue03-ygue (#320)
91e52cb Ue02 ygue (#206)


---

## Assistant

_Thinking:_

So GitHub username is 52yuyu (origin remote). Yet branches are named ue02-ygue and ue03-ygue, and directories ue02/ygue, ue03/ygue. Perhaps "ygue" is an earlier abbreviation. But ue04/52yuyu is the current one matching the GitHub username.

Let me verify the content of ue02/ygue and ue03/ygue commits' authors, and check git log for commits by this person. Also check ue01 for a steckbrief.

**Tool: shell**

**Input:**
```json
{
  "command": "git log --format='%h %an %s' --author='52yuyu' --all | head -20; echo \"-- ygue commits\"; git show --stat --oneline a5ce6a5 | head -10; git show --stat --oneline 91e52cb | head -10"
}
```

00d88ac 52yuyu Merge branch 'carstenlucke:main' into main
a5ce6a5 52yuyu Ue03-ygue (#320)
91e52cb 52yuyu Ue02 ygue (#206)
f0c0d4d 52yuyu Merge branch 'carstenlucke:main' into main
e8b89e6 52yuyu Steckbrief für ygue anlegen (#85)
9924f69 52yuyu Add initial entry for ygue with no experience
-- ygue commits
a5ce6a5 Ue03-ygue (#320)
 ue03/ygue/anforderungen.md | 15 +++++++++++++++
 ue03/ygue/kontext.md       | 24 ++++++++++++++++++++++++
 ue03/ygue/zuordnung.md     | 39 +++++++++++++++++++++++++++++++++++++++
 3 files changed, 78 insertions(+)
91e52cb Ue02 ygue (#206)
 ue02/ygue/notiz.md         | 20 +++++++++++++++
 ue02/ygue/phasenplan.md    | 64 ++++++++++++++++++++++++++++++++++++++++++++++
 ue02/ygue/spezifikation.md | 22 ++++++++++++++++
 3 files changed, 106 insertions(+)


**Tool: shell**

**Input:**
```json
{
  "command": "ls -1 ue01/steckbriefe | head -40; echo \"--\"; ls -1 ue01/steckbriefe | grep -i -E 'ygu|yuyu|younes'"
}
```

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
--
ygue.md


---

## Assistant

_Thinking:_

Confirmed: user's GitHub username is 52yuyu, earlier abbreviation ygue. Files: ue01/steckbriefe/ygue.md, ue02/ygue/*, ue03/ygue/*, and untracked ue04/52yuyu/einrichtung.md.

Let me quickly check contents summaries of each to describe them. Also note the naming inconsistency: ue04 should be ue04/52yuyu per current rule (matches GitHub username) — that's fine actually. The branches ue02-ygue/ue03-ygue are older.

Let me read the files briefly to summarize (first lines only).

**Tool: shell**

**Input:**
```json
{
  "command": "for f in ue01/steckbriefe/ygue.md ue02/ygue/notiz.md ue02/ygue/phasenplan.md ue02/ygue/spezifikation.md ue03/ygue/anforderungen.md ue03/ygue/kontext.md ue03/ygue/zuordnung.md; do echo \"===== $f ($(wc -l < \"$f\") Zeilen)\"; head -6 \"$f\"; done"
}
```

===== ue01/steckbriefe/ygue.md (      10 Zeilen)
# Steckbrief ygue

## Studiengang und Semester
Wirtschaftsinformatik (B.Sc.) im 3. Semester an der THM in Friedberg.

## Meine bisherige Erfahrung mit Softwareentwicklung
===== ue02/ygue/notiz.md (      20 Zeilen)
# Gesprächsnotiz
## Ausgangslage
Bisher wird der Ablauf weitgehend manuell koordiniert.
## Was heute benutzt wird
* E-Mail
* Werkzeuge im Netz
===== ue02/ygue/phasenplan.md (      64 Zeilen)
# Phasenplan — Terminplaner für die THM

Kürzel: ygue

## Studie

===== ue02/ygue/spezifikation.md (      22 Zeilen)
# Spezifikation Terminplaner

* Beteiligte: @52yuyu

## 1. Ziel und Zweck
Das System soll Studierenden und Lehrenden der THM ermöglichen, Sprechstunden- und Prüfungstermine digital zu vereinbaren und zu verwalten.
===== ue03/ygue/anforderungen.md (      15 Zeilen)
# Anforderungen – Terminplaner für die THM

## Anforderungen

| Nr. | Anforderung | Stakeholder | Art |
| :--- | :--- | :--- | :--- |
===== ue03/ygue/kontext.md (      24 Zeilen)
# Aufgabe 1: Stakeholder und Systemkontext

## 1. Stakeholder
| Stakeholder | Einfluss auf die Anforderungen |
| :--- | :--- |
| **Studierende** | Wollen vor allem, dass die App unterwegs auf dem Handy flüssig läuft und man schnell Termine buchen kann. |
===== ue03/ygue/zuordnung.md (      39 Zeilen)
# Anforderung oder Lösung? — Terminplaner für die THM

Kürzel: ygue

## Funktionale Anforderung (FA)



---

## Assistant

_Thinking:_

Now compose the answer in German. Mention: repo structure (ue01–ue04), templates, many student dirs. The user's GitHub username is 52yuyu (origin remote), earlier abbreviation ygue. Files belonging to them:

- ue01/steckbriefe/ygue.md
- ue02/ygue/{notiz,phasenplan,spezifikation}.md
- ue03/ygue/{anforderungen,kontext,zuordnung}.md
- ue04/52yuyu/einrichtung.md (untracked, not yet committed; sitzung.md still missing per ue04 README)

Also note: on main, untracked change exists. Per AGENTS.md, don't commit. Mention that ue04 must be submitted on branch ue04-52yuyu and sitzung.md is missing.

Should I flag the naming mismatch? ue04 dir uses 52yuyu (correct per current rule), older ones use ygue (older abbreviations). That's fine — AGENTS.md says older dirs may carry earlier chosen abbreviation and still belong to the person. Ask if unclear? It's fairly clear from commits (all authored by 52yuyu, branch names ue02-ygue). I could mention assumption and ask for confirmation rather than blocking.

Keep concise with a table.

## Das Repository

Es ist das Übungsrepository der Veranstaltung Softwaretechnik (THM Friedberg). Alles ist nach Übungen gegliedert, jede mit eigener `README.md`:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | `steckbriefe/` – je eine Steckbrief-Datei pro Person, dazu `_vorlage.md` und `_beispiel.md` |
| `ue02/` | Projektmodell am Fall „Terminplaner“ – pro Person ein Unterverzeichnis, dazu `_vorlage/` und `_zugabe/` |
| `ue03/` | Anforderungen – ebenfalls ein Unterverzeichnis pro Person, dazu `_vorlage/` |
| `ue04/` | Coding Agent einrichten – `_vorlage/` und bisher nur ein Personenverzeichnis |
| `README.md`, `AGENTS.md` | Spielregeln des Repos (Fork, Branch, PR, nur eigene Dateien) |

`ue02` und `ue03` enthalten die Beiträge von rund 100 Kommilitoninnen und Kommilitonen; die sind für dich nur zum Lesen da.

## Deine Dateien

Dein GitHub-Benutzername ist **52yuyu** (so steht es in `origin`), früher hast du das Kürzel **ygue** verwendet. Dazu passen auch deine Branches `ue02-ygue` und `ue03-ygue`. Von dir stammen:

| Datei | Übung / Inhalt |
|---|---|
| `ue01/steckbriefe/ygue.md` | Ü1 – Steckbrief (Wirtschaftsinformatik, 3. Semester) |
| `ue02/ygue/notiz.md` | Ü2 – Gesprächsnotiz zur Ausgangslage |
| `ue02/ygue/phasenplan.md` | Ü2 – Phasenplan Terminplaner |
| `ue02/ygue/spezifikation.md` | Ü2 – Spezifikation Terminplaner |
| `ue03/ygue/anforderungen.md` | Ü3 – Anforderungstabelle |
| `ue03/ygue/kontext.md` | Ü3 – Stakeholder und Systemkontext |
| `ue03/ygue/zuordnung.md` | Ü3 – Anforderung oder Lösung? |
| `ue04/52yuyu/einrichtung.md` | Ü4 – Einrichtung opencode, **noch nicht committet** |

Alles davon ist bereits committet und über Pull Requests eingegangen – außer der letzten Datei.

## Zwei Hinweise

1. Du stehst auf `main`, und `ue04/52yuyu/` ist noch ungetrackt. Laut `AGENTS.md` ändere und committe ich auf `main` nichts. Für die Abgabe bräuchtest du einen Branch `ue04-52yuyu`.
2. In `ue04/` fehlt noch `sitzung.md` (die exportierte Agenten-Sitzung); laut Übungs-README gehören beide Dateien zum Pull Request.

Soll ich einen Branch `ue04-52yuyu` anlegen und die Einreichung dort vorbereiten?
