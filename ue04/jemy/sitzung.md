# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e4f040e89ffeMpkbEiW7whn424
**Created:** 11/6/2026, 2:11:03 PM
**Updated:** 11/6/2026, 2:11:27 PM

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?


---

## Assistant

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current"
}
```

ue04-jemy


---

## Assistant

**Tool: read**

**Input:**
```json
{
  "path": "../README.md"
}
```

Read file ../README.md, lines 1-74
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
  "path": ".."
}
```

Read directory .., entries 1-7
.git/
ue01/
ue02/
ue03/
ue04/
AGENTS.md
README.md

**Tool: shell**

**Input:**
```json
{
  "command": "git status --short"
}
```

?? jemy/


**Tool: glob**

**Input:**
```json
{
  "pattern": "**/jemy/**",
  "path": "..",
  "limit": 200
}
```

/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue02/jemy/phasenplan.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue02/jemy/notiz.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue02/jemy/spezifikation.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue02/jemy/rollen.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue04/jemy/einrichtung.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue03/jemy/anforderungen.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue03/jemy/kontext.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue03/jemy/zuordnung.md

**Tool: glob**

**Input:**
```json
{
  "pattern": "**/AGENTS.md",
  "path": ".."
}
```

/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/AGENTS.md

---

## Assistant

**Tool: read**

**Input:**
```json
{
  "path": "../ue01"
}
```

Read directory ../ue01, entries 1-2
steckbriefe/
README.md

**Tool: read**

**Input:**
```json
{
  "path": "../ue02"
}
```

Read directory ../ue02, entries 1-111
_vorlage/
_zugabe/
aayd/
abdu113/
af/
agbr/
Agub/
ahyi/
akyf/
anas23088/
anddun/
andel0/
anpa/
anushka/
athr/
avon507/
ayue/
bblj09/
bima/
datr03/
div/
dlm28/
dmmh1710/
dsc/
dsch/
dszp/
emrano/
en7-mj/
ezen/
fahm/
flk/
fortnitepro/
hams/
hfdr12/
iaa/
iesp/
ilias04j/
ivlbs/
IY69/
janp/
javu11/
jemy/
jp26/
jsug/
jvng/
kraz/
lebr/
lom/
Lpr/
mabl/
masalabyte/
maxbarrosschauer/
mbgrn04/
mduc/
meq/
mf23/
mjab/
mjas/
mk/
mkon/
mpal/
mu/
mw/
my55/
ngh/
nicolino/
nko/
nly50/
NN/
nohl/
NUAli/
oubou/
pdam/
pgml/
pz01/
qdb/
qho/
real/
renn/
sahmad/
sahmed/
sam/
skrl78/
skt435/
snab/
sngu/
ssda78/
sshj44/
ssng61/
stmx/
talh/
TariqK2004/
tcam/
thm-nos/
thng/
tiger/
tnd/
tngan/
trry/
ttpr21/
tyfncc/
uwar/
vic26/
virus/
wnga/
ygue/
ysbi82/
zcbn/
zcoel/
zsh/
README.md

**Tool: read**

**Input:**
```json
{
  "path": "../ue03"
}
```

Read directory ../ue03, entries 1-97
_vorlage/
aayd/
af/
agbr/
ahyi/
akyf/
anas23088/
anddun/
andel0/
anpa/
anushka/
avon507/
ayue/
azm96/
bblj09/
bogh233/
cms/
davn68/
dlm28/
dmmh1710/
dsch/
ecib/
emrano/
en7-mj/
ezen/
fahm/
flk/
hfdr12/
iaa/
ilias04j/
IY69/
janp/
javu/
jemy/
jsug/
jvng/
kraz/
lkrs/
lom/
Lpr/
masalabyte/
maxbarrosschauer/
mduc/
meq/
mjab/
MK/
mken/
mkon/
moh/
mpal/
mskk15/
mu/
mw/
my55/
nicolino/
nko/
nly50/
NN/
nohl/
NUAli/
onzj/
oubou/
pdam/
pgml/
pz01/
qho/
real/
sahmad/
sahmed/
sam/
skrl78/
snab/
sngu/
sraks/
ssda78/
sshj44/
stmx/
talh/
TariqK2004/
tcam/
tiger/
tnd/
trry/
tyfncc/
uwar/
val/
vic26/
virus/
wnga/
ygue/
ykar/
z-266/
zc/
zcbn/
zcoel/
zsh/
README.md

**Tool: read**

**Input:**
```json
{
  "path": "."
}
```

Read directory ., entries 1-3
_vorlage/
jemy/
README.md

---

## Assistant

**Tool: glob**

**Input:**
```json
{
  "pattern": "*",
  "path": "../ue01/steckbriefe",
  "limit": 200
}
```

/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/jat01.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/_beispiel.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/emalj.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/adni.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ngh.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ecib.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/nko.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mpal.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sngu.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/oubou.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/tngan.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mnag.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/pz01.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/renn.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/qdb.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/aayd.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/anpa.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/iesp.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/NN.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ahyi.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sshj44.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mskk15.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/janp.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mjas.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/val.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/cms.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/fortnitepro.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Lpr.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/pgml.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/bunter95.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ttpr21.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ssng61.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/hfdr12.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/MK.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/_vorlage.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/lom.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/pdam.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dsc.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/anushka.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/HussainButt7.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/lswl60.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Anas23088.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mken.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mw.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/jemy.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dlm28.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/real.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/snab.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/emrano.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mosm.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/en7-mj.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mks24.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ysbi82.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/davn68.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mduc.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/lkrs.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/shiva.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/onzj.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/IY69.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/qho.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/maxbarrosschauer.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mf23.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Tiger.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/trry.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/masalabyte.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/AF.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sd99.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/avon507.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ezen.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dsch.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/athr.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/zcbn.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/div.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/NUAli.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/nicolino.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dmmh1710.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Agub.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ZahraGit12.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Smu.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/tcam.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/virus.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/stmx.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/akyf.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dhfn1611.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sazy1.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dszp.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/skrl78.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mabl.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sam.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/vic26.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/zomj.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/vkab.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/lebr.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/andel0.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/hjri.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Bblj09.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ale563.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ilias04j.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Aza.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/slr63.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/tnd.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/thng.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ykar.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/asng24.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/TariqK2004.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/tyfncc.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mjab.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/zc.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/peng.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/kraz.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/flk.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/wnga.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/datr03.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/jvng.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sahmad.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/uk.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/asi.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ygue.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/dmal2004.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/nohl.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/fpz.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/lpr2.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/nblh.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/yamekk.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/javu.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/skt435.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/yoibr42.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mbgrn04.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/meq.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ekes.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/uwar.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/iaa.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Fahm.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mkon.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/bima.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/mu.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/anddun.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/jk04.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/azm96.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/AR.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/agbr.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/nly50.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/aalg.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/jsug.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/jp26.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/Z-266.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/zcoel.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/my55.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/hams.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/sahmed.md
/Users/EMLR1011/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/ivlbs.md

---

## Assistant

## Was liegt im Repository?

Das Repository enthält Abgaben zu den **Softwaretechnik-Übungen der THM**:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | Git und GitHub, persönliche Steckbriefe |
| `ue02/` | Projektmodell am Fall |
| `ue03/` | Anforderungen an einen Terminplaner |
| `ue04/` | Einen Coding Agent einrichten |

Dazu kommen Aufgabenbeschreibungen (`README.md`), Vorlagen (`_vorlage/`), Zusatzmaterial (`_zugabe/`) und Agentenregeln (`AGENTS.md`).

## Welche Dateien gehören dir?

Dein aktueller Branch heißt **`ue04-jemy`**. Nach der Namenskonvention sind dir diese Dateien zugeordnet, jeweils relativ zur Repository-Wurzel:

```text
ue01/steckbriefe/jemy.md

ue02/jemy/notiz.md
ue02/jemy/phasenplan.md
ue02/jemy/rollen.md
ue02/jemy/spezifikation.md

ue03/jemy/anforderungen.md
ue03/jemy/kontext.md
ue03/jemy/zuordnung.md

ue04/jemy/einrichtung.md
```

**Aktueller Git-Status:** `ue04/jemy/` ist noch nicht versioniert, also noch nicht in einem Commit enthalten. Sonst werden keine lokalen Änderungen angezeigt.

Falls du früher ein anderes Kürzel verwendet hast, könnten weitere Dateien dir gehören; das lässt sich aus dem Branchnamen allein nicht erkennen. Ich habe nichts verändert.
