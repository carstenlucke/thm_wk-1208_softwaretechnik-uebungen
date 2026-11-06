# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e5396250fffeDEutKUSZMqAuqi
**Created:** 11/5/2026, 4:53:00 PM
**Updated:** 11/6/2026, 12:07:37 PM

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

Let me explore the repository. Start with listing and git info.

Ich schaue mir das Repository an.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current && git status --short && git log --oneline -5"
}
```

ue04-mskk155
?? ue04/mskk155/
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)


**Tool: shell**

**Input:**
```json
{
  "command": "ls -la"
}
```

total 16
drwxr-xr-x@   9 mariamsekkali  staff   288 Nov  5 16:46 .
drwx------@   4 mariamsekkali  staff   128 Oct 19 10:35 ..
drwxr-xr-x@  15 mariamsekkali  staff   480 Nov  5 16:46 .git
-rw-r--r--@   1 mariamsekkali  staff  2172 Nov  5 16:46 AGENTS.md
-rw-r--r--@   1 mariamsekkali  staff  3212 Nov  5 16:46 README.md
drwxr-xr-x@   4 mariamsekkali  staff   128 Nov  5 16:46 ue01
drwxr-xr-x@ 113 mariamsekkali  staff  3616 Nov  5 16:46 ue02
drwxr-xr-x@  99 mariamsekkali  staff  3168 Nov  5 16:46 ue03
drwxr-xr-x@   5 mariamsekkali  staff   160 Nov  5 16:48 ue04


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

Branch ue04-mskk155, untracked ue04/mskk155/. Let's inspect the repository structure counts and own files.

**Tool: shell**

**Input:**
```json
{
  "command": "find . -path ./.git -prune -o -type f -print | sort | sed 's|^\\./||'"
}
```

AGENTS.md
README.md
ue01/README.md
ue01/steckbriefe/_beispiel.md
ue01/steckbriefe/_vorlage.md
ue01/steckbriefe/aalg.md
ue01/steckbriefe/aayd.md
ue01/steckbriefe/adni.md
ue01/steckbriefe/AF.md
ue01/steckbriefe/agbr.md
ue01/steckbriefe/Agub.md
ue01/steckbriefe/ahyi.md
ue01/steckbriefe/akyf.md
ue01/steckbriefe/ale563.md
ue01/steckbriefe/Anas23088.md
ue01/steckbriefe/anddun.md
ue01/steckbriefe/andel0.md
ue01/steckbriefe/anpa.md
ue01/steckbriefe/anushka.md
ue01/steckbriefe/AR.md
ue01/steckbriefe/asi.md
ue01/steckbriefe/asng24.md
ue01/steckbriefe/athr.md
ue01/steckbriefe/avon507.md
ue01/steckbriefe/Aza.md
ue01/steckbriefe/azm96.md
ue01/steckbriefe/Bblj09.md
ue01/steckbriefe/bima.md
ue01/steckbriefe/bunter95.md
ue01/steckbriefe/cms.md
ue01/steckbriefe/datr03.md
ue01/steckbriefe/davn68.md
ue01/steckbriefe/dhfn1611.md
ue01/steckbriefe/div.md
ue01/steckbriefe/dlm28.md
ue01/steckbriefe/dmal2004.md
ue01/steckbriefe/dmmh1710.md
ue01/steckbriefe/dsc.md
ue01/steckbriefe/dsch.md
ue01/steckbriefe/dszp.md
ue01/steckbriefe/ecib.md
ue01/steckbriefe/ekes.md
ue01/steckbriefe/emalj.md
ue01/steckbriefe/emrano.md
ue01/steckbriefe/en7-mj.md
ue01/steckbriefe/ezen.md
ue01/steckbriefe/Fahm.md
ue01/steckbriefe/flk.md
ue01/steckbriefe/fortnitepro.md
ue01/steckbriefe/fpz.md
ue01/steckbriefe/hams.md
ue01/steckbriefe/hfdr12.md
ue01/steckbriefe/hjri.md
ue01/steckbriefe/HussainButt7.md
ue01/steckbriefe/iaa.md
ue01/steckbriefe/iesp.md
ue01/steckbriefe/ilias04j.md
ue01/steckbriefe/ivlbs.md
ue01/steckbriefe/IY69.md
ue01/steckbriefe/janp.md
ue01/steckbriefe/jat01.md
ue01/steckbriefe/javu.md
ue01/steckbriefe/jemy.md
ue01/steckbriefe/jk04.md
ue01/steckbriefe/jp26.md
ue01/steckbriefe/jsug.md
ue01/steckbriefe/jvng.md
ue01/steckbriefe/kraz.md
ue01/steckbriefe/lebr.md
ue01/steckbriefe/lkrs.md
ue01/steckbriefe/lom.md
ue01/steckbriefe/Lpr.md
ue01/steckbriefe/lpr2.md
ue01/steckbriefe/lswl60.md
ue01/steckbriefe/mabl.md
ue01/steckbriefe/masalabyte.md
ue01/steckbriefe/maxbarrosschauer.md
ue01/steckbriefe/mbgrn04.md
ue01/steckbriefe/mduc.md
ue01/steckbriefe/meq.md
ue01/steckbriefe/mf23.md
ue01/steckbriefe/mjab.md
ue01/steckbriefe/mjas.md
ue01/steckbriefe/MK.md
ue01/steckbriefe/mken.md
ue01/steckbriefe/mkon.md
ue01/steckbriefe/mks24.md
ue01/steckbriefe/mnag.md
ue01/steckbriefe/mosm.md
ue01/steckbriefe/mpal.md
ue01/steckbriefe/mskk15.md
ue01/steckbriefe/mu.md
ue01/steckbriefe/mw.md
ue01/steckbriefe/my55.md
ue01/steckbriefe/nblh.md
ue01/steckbriefe/ngh.md
ue01/steckbriefe/nicolino.md
ue01/steckbriefe/nko.md
ue01/steckbriefe/nly50.md
ue01/steckbriefe/NN.md
ue01/steckbriefe/nohl.md
ue01/steckbriefe/NUAli.md
ue01/steckbriefe/onzj.md
ue01/steckbriefe/oubou.md
ue01/steckbriefe/pdam.md
ue01/steckbriefe/peng.md
ue01/steckbriefe/pgml.md
ue01/steckbriefe/pz01.md
ue01/steckbriefe/qdb.md
ue01/steckbriefe/qho.md
ue01/steckbriefe/real.md
ue01/steckbriefe/renn.md
ue01/steckbriefe/sahmad.md
ue01/steckbriefe/sahmed.md
ue01/steckbriefe/sam.md
ue01/steckbriefe/sazy1.md
ue01/steckbriefe/sd99.md
ue01/steckbriefe/shiva.md
ue01/steckbriefe/skrl78.md
ue01/steckbriefe/skt435.md
ue01/steckbriefe/slr63.md
ue01/steckbriefe/Smu.md
ue01/steckbriefe/snab.md
ue01/steckbriefe/sngu.md
ue01/steckbriefe/sshj44.md
ue01/steckbriefe/ssng61.md
ue01/steckbriefe/stmx.md
ue01/steckbriefe/TariqK2004.md
ue01/steckbriefe/tcam.md
ue01/steckbriefe/thng.md
ue01/steckbriefe/Tiger.md
ue01/steckbriefe/tnd.md
ue01/steckbriefe/tngan.md
ue01/steckbriefe/trry.md
ue01/steckbriefe/ttpr21.md
ue01/steckbriefe/tyfncc.md
ue01/steckbriefe/uk.md
ue01/steckbriefe/uwar.md
ue01/steckbriefe/val.md
ue01/steckbriefe/vic26.md
ue01/steckbriefe/virus.md
ue01/steckbriefe/vkab.md
ue01/steckbriefe/wnga.md
ue01/steckbriefe/yamekk.md
ue01/steckbriefe/ygue.md
ue01/steckbriefe/ykar.md
ue01/steckbriefe/yoibr42.md
ue01/steckbriefe/ysbi82.md
ue01/steckbriefe/Z-266.md
ue01/steckbriefe/ZahraGit12.md
ue01/steckbriefe/zc.md
ue01/steckbriefe/zcbn.md
ue01/steckbriefe/zcoel.md
ue01/steckbriefe/zomj.md
ue02/_vorlage/notiz.md
ue02/_vorlage/spezifikation.md
ue02/_zugabe/rollen.md
ue02/aayd/notiz.md
ue02/aayd/phasenplan.md
ue02/aayd/spezifikation.md
ue02/abdu113/notiz.md
ue02/abdu113/phasenplan.md
ue02/abdu113/spezifikation.md
ue02/af/notiz.md
ue02/af/phasenplan.md
ue02/af/spezifikation.md
ue02/agbr/notiz.md
ue02/agbr/phasenplan.md
ue02/agbr/spezifikation.md
ue02/Agub/notiz.md
ue02/Agub/phasenplan.md
ue02/Agub/rollen.md
ue02/Agub/spezifikation.md
ue02/ahyi/notiz.md
ue02/ahyi/phasenplan.md
ue02/ahyi/spezifikation.md
ue02/akyf/notiz.md
ue02/akyf/phasenplan.md
ue02/akyf/spezifikation.md
ue02/anas23088/notiz.md
ue02/anas23088/phasenplan.md
ue02/anas23088/rollen.md
ue02/anas23088/spezifikation.md
ue02/anddun/notiz.md
ue02/anddun/phasenplan.md
ue02/anddun/spezifikation.md
ue02/andel0/notiz.md
ue02/andel0/phasenplan.md
ue02/andel0/spezifikation.md
ue02/anpa/notiz.md
ue02/anpa/phasenplan.md
ue02/anpa/rollen.md
ue02/anpa/spezifikation.md
ue02/anushka/notiz.md
ue02/anushka/phasenplan.md
ue02/anushka/rollen.md
ue02/anushka/spezifikation.md
ue02/athr/notiz.md
ue02/athr/phasenplan.md
ue02/athr/spezifikation.md
ue02/avon507/notiz.md
ue02/avon507/phasenplan.md
ue02/avon507/spezifikation.md
ue02/ayue/notiz.md
ue02/ayue/phasenplan.md
ue02/ayue/spezifikation.md
ue02/bblj09/notiz.md
ue02/bblj09/phasenplan.md
ue02/bblj09/spezifikation.md
ue02/bima/notiz.md
ue02/bima/phasenplan.md
ue02/bima/spezifikation.md
ue02/datr03/notiz.md
ue02/datr03/phasenplan.md
ue02/datr03/spezifikation.md
ue02/div/notiz.md
ue02/div/phasenplan.md
ue02/div/rollen.md
ue02/div/spezifikation.md
ue02/dlm28/notiz.md
ue02/dlm28/phasenplan.md
ue02/dlm28/spezifikation.md
ue02/dmmh1710/notiz.md
ue02/dmmh1710/phasenplan.md
ue02/dmmh1710/spezifikation.md
ue02/dsc/notiz.md
ue02/dsc/phasenplan.md
ue02/dsc/spezifikation.md
ue02/dsch/notiz.md
ue02/dsch/phasenplan.md
ue02/dsch/spezifikation.md
ue02/dszp/notiz.md
ue02/dszp/phasenplan.md
ue02/dszp/spezifikation.md
ue02/emrano/notiz.md
ue02/emrano/phasenplan.md
ue02/emrano/spezifikation.md
ue02/en7-mj/notiz.md
ue02/en7-mj/phasenplan.md
ue02/en7-mj/spezifikation.md
ue02/ezen/notiz.md
ue02/ezen/phasenplan.md
ue02/ezen/spezifikation.md
ue02/fahm/notiz.md
ue02/fahm/phasenplan.md
ue02/fahm/spezifikation.md
ue02/flk/notiz.md
ue02/flk/phasenplan.md
ue02/flk/spezifikation.md
ue02/fortnitepro/notiz.md
ue02/fortnitepro/phasenplan.md
ue02/fortnitepro/spezifikation.md
ue02/hams/notiz.md
ue02/hams/phasenplan.md
ue02/hams/spezifikation.md
ue02/hfdr12/notiz.md
ue02/hfdr12/phasenplan.md
ue02/hfdr12/spezifikation.md
ue02/iaa/notiz.md
ue02/iaa/phasenplan.md
ue02/iaa/spezifikation.md
ue02/iesp/notiz.md
ue02/iesp/phasenplan.md
ue02/iesp/spezifikation.md
ue02/ilias04j/notiz.md
ue02/ilias04j/phasenplan.md
ue02/ilias04j/spezifikation.md
ue02/ivlbs/notiz.md
ue02/ivlbs/phasenplan.md
ue02/ivlbs/spezifikation.md
ue02/IY69/notiz.md
ue02/IY69/phasenplan.md
ue02/IY69/spezifikation.md
ue02/janp/notiz.md
ue02/janp/phasenplan.md
ue02/janp/rollen.md
ue02/janp/spezifikation.md
ue02/javu11/notiz.md
ue02/javu11/phasenplan.md
ue02/javu11/rollen.md
ue02/javu11/spezifikation.md
ue02/jemy/notiz.md
ue02/jemy/phasenplan.md
ue02/jemy/rollen.md
ue02/jemy/spezifikation.md
ue02/jp26/notiz.md
ue02/jp26/phasenplan.md
ue02/jp26/spezifikation.md
ue02/jsug/notiz.md
ue02/jsug/phasenplan.md
ue02/jsug/spezifikation.md
ue02/jvng/notiz.md
ue02/jvng/rollen.md
ue02/jvng/spezifikation.md
ue02/kraz/notiz.md
ue02/kraz/phasenplan.md
ue02/kraz/spezifikation.md
ue02/lebr/notiz.md
ue02/lebr/phasenplan.md
ue02/lebr/spezifikation.md
ue02/lom/notiz.md
ue02/lom/phasenplan.md
ue02/lom/spezifikation.md
ue02/Lpr/notiz.md
ue02/Lpr/phasenplan.md
ue02/Lpr/spezifikation.md
ue02/mabl/notiz.md
ue02/mabl/phasenplan.md
ue02/mabl/spezifikation.md
ue02/masalabyte/notiz.md
ue02/masalabyte/phasenplan.md
ue02/masalabyte/spezifikation.md
ue02/maxbarrosschauer/notiz.md
ue02/maxbarrosschauer/phasenplan.md
ue02/maxbarrosschauer/rollen.md
ue02/maxbarrosschauer/spezifikation.md
ue02/mbgrn04/notiz.md
ue02/mbgrn04/phasenplan.md
ue02/mbgrn04/spezifikation.md
ue02/mduc/notiz.md
ue02/mduc/phasenplan.md
ue02/mduc/spezifikation.md
ue02/meq/notiz.md
ue02/meq/phasenplan.md
ue02/meq/rollen.md
ue02/meq/spezifikation.md
ue02/mf23/notiz.md
ue02/mf23/phasenplan.md
ue02/mf23/spezifikation.md
ue02/mjab/notiz.md
ue02/mjab/phasenplan.md
ue02/mjab/spezifikation.md
ue02/mjas/notiz.md
ue02/mjas/phasenplan.md
ue02/mjas/spezifikation.md
ue02/mk/phasenplan.md
ue02/mkon/notiz.md
ue02/mkon/phasenplan.md
ue02/mkon/spezifikation.md
ue02/mpal/notiz.md
ue02/mpal/phasenplan.md
ue02/mpal/spezifikation.md
ue02/mu/notiz.md
ue02/mu/phasenplan.md
ue02/mu/spezifikation.md
ue02/mw/notiz.md
ue02/mw/phasenplan.md
ue02/mw/spezifikation.md
ue02/my55/notiz.md
ue02/my55/phasenplan.md
ue02/my55/spezifikation.md
ue02/ngh/notiz.md
ue02/ngh/phasenplan.md
ue02/ngh/spezifikation.md
ue02/nicolino/notiz.md
ue02/nicolino/phasenplan.md
ue02/nicolino/spezifikation.md
ue02/nko/notiz.md
ue02/nko/phasenplan.md
ue02/nko/spezifikation.md
ue02/nly50/notiz.md
ue02/nly50/phasenplan.md
ue02/nly50/spezifikation.md
ue02/NN/notiz.md
ue02/NN/phasenplan.md
ue02/NN/spezifikation.md
ue02/nohl/notiz.md
ue02/nohl/phasenplan.md
ue02/nohl/spezifikation.md
ue02/NUAli/notiz.md
ue02/NUAli/phasenplan.md
ue02/NUAli/spezifikation.md
ue02/oubou/notiz.md
ue02/oubou/phasenplan.md
ue02/oubou/spezifikation.md
ue02/pdam/notiz.md
ue02/pdam/phasenplan.md
ue02/pdam/spezifikation.md
ue02/pgml/notiz.md
ue02/pgml/phasenplan.md
ue02/pgml/spezifikation.md
ue02/pz01/notiz.md
ue02/pz01/phasenplan.md
ue02/pz01/spezifikation.md
ue02/qdb/notiz.md
ue02/qdb/phasenplan.md
ue02/qdb/rollen.md
ue02/qdb/spezifikation.md
ue02/qho/notiz.md
ue02/qho/phasenplan.md
ue02/qho/spezifikation.md
ue02/README.md
ue02/real/notiz.md
ue02/real/phasenplan.md
ue02/real/spezifikation.md
ue02/renn/notiz.md
ue02/renn/phasenplan.md
ue02/renn/spezifikation.md
ue02/sahmad/notiz.md
ue02/sahmad/phasenplan.md
ue02/sahmad/spezifikation.md
ue02/sahmed/notiz.md
ue02/sahmed/phasenplan.md
ue02/sahmed/rollen.md
ue02/sahmed/spezifikation.md
ue02/sam/notiz.md
ue02/sam/phasenplan.md
ue02/sam/spezifikation.md
ue02/skrl78/notiz.md
ue02/skrl78/phasenplan.md
ue02/skrl78/rollen.md
ue02/skrl78/spezifikation.md
ue02/skt435/notiz.md
ue02/skt435/spezifikation.md
ue02/snab/notiz.md
ue02/snab/phasenplan.md
ue02/snab/spezifikation.md
ue02/sngu/notiz.md
ue02/sngu/phasenplan.md
ue02/sngu/spezifikation.md
ue02/ssda78/notiz.md
ue02/ssda78/spezifikation.md
ue02/sshj44/notiz.md
ue02/sshj44/phasenplan.md
ue02/sshj44/spezifikation.md
ue02/ssng61/notiz.md
ue02/ssng61/spezifikation.md
ue02/stmx/notiz.md
ue02/stmx/phasenplan.md
ue02/stmx/spezifikation.md
ue02/talh/notiz.md
ue02/talh/phasenplan.md
ue02/talh/rollen.md
ue02/talh/spezifikation.md
ue02/TariqK2004/notiz.md
ue02/TariqK2004/phasenplan.md
ue02/TariqK2004/spezifikation.md
ue02/tcam/notiz.md
ue02/tcam/phasenplan.md
ue02/tcam/spezifikation.md
ue02/thm-nos/notiz.md
ue02/thm-nos/phasenplan.md
ue02/thm-nos/spezifikation.md
ue02/thng/notiz.md
ue02/thng/phasenplan.md
ue02/thng/spezifikation.md
ue02/tiger/notiz.md
ue02/tiger/phasenplan.md
ue02/tiger/spezifikation.md
ue02/tnd/notiz.md
ue02/tnd/phasenplan.md
ue02/tnd/spezifikation.md
ue02/tngan/notiz.md
ue02/tngan/phasenplan.md
ue02/tngan/spezifikation.md
ue02/trry/notiz.md
ue02/trry/phasenplan.md
ue02/trry/rollen.md
ue02/trry/spezifikation.md
ue02/ttpr21/notiz.md
ue02/ttpr21/phasenplan.md
ue02/ttpr21/spezifikation.md
ue02/tyfncc/notiz.md
ue02/tyfncc/phasenplan.md
ue02/tyfncc/rollen.md
ue02/tyfncc/spezifikation.md
ue02/uwar/notiz.md
ue02/uwar/phasenplan.md
ue02/uwar/spezifikation.md
ue02/vic26/notiz.md
ue02/vic26/phasenplan.md
ue02/vic26/spezifikation.md
ue02/virus/notiz.md
ue02/virus/phasenplan.md
ue02/virus/spezifikation.md
ue02/wnga/notiz.md
ue02/wnga/phasenplan.md
ue02/wnga/rollen.md
ue02/wnga/spezifikation.md
ue02/ygue/notiz.md
ue02/ygue/phasenplan.md
ue02/ygue/spezifikation.md
ue02/ysbi82/notiz.md
ue02/ysbi82/spezifikation.md
ue02/zcbn/notiz.md
ue02/zcbn/phasenplan.md
ue02/zcbn/spezifikation.md
ue02/zcoel/notiz.md
ue02/zcoel/phasenplan.md
ue02/zcoel/spezifikation.md
ue02/zsh/notiz.md
ue02/zsh/phasenplan.md
ue02/zsh/spezifikation.md
ue03/_vorlage/anforderungen.md
ue03/_vorlage/kontext.md
ue03/aayd/anforderungen.md
ue03/aayd/kontext.md
ue03/aayd/zuordnung.md
ue03/af/anforderungen.md
ue03/af/kontext.md
ue03/af/zuordnung.md
ue03/agbr/anforderungen.md
ue03/agbr/kontext.md
ue03/agbr/zuordnung.md
ue03/ahyi/anforderungen.md
ue03/ahyi/kontext.md
ue03/ahyi/zuordnung.md
ue03/akyf/anforderungen.md
ue03/akyf/kontext.md
ue03/akyf/zuordnung.md
ue03/anas23088/anforderungen.md
ue03/anas23088/kontext.md
ue03/anas23088/zuordnung.md
ue03/anddun/anforderungen.md
ue03/anddun/kontext.md
ue03/anddun/zuordnung.md
ue03/andel0/anforderungen.md
ue03/andel0/kontext.md
ue03/andel0/zuordnung.md
ue03/anpa/anforderungen.md
ue03/anpa/kontext.md
ue03/anpa/zuordnung.md
ue03/anushka/anforderungen.md
ue03/anushka/kontext.md
ue03/anushka/zuordnung.md
ue03/avon507/anforderungen.md
ue03/avon507/kontext.md
ue03/avon507/zuordnung.md
ue03/ayue/anforderungen.md
ue03/ayue/kontext.md
ue03/ayue/zuordnung.md
ue03/azm96/anforderungen.md
ue03/azm96/kontext.md
ue03/azm96/zuordnung.md
ue03/bblj09/anforderungen.md
ue03/bblj09/kontext.md
ue03/bblj09/zuordnung.md
ue03/bogh233/anforderungen.md
ue03/bogh233/kontext.md
ue03/bogh233/zuordnung.md
ue03/cms/anforderungen.md
ue03/cms/kontext.md
ue03/cms/zuordnung.md
ue03/davn68/anforderungen.md
ue03/davn68/kontext.md
ue03/davn68/zuordnung.md
ue03/dlm28/anforderungen.md
ue03/dlm28/kontext.md
ue03/dlm28/zuordnung.md
ue03/dmmh1710/anforderungen.md
ue03/dmmh1710/kontext.md
ue03/dmmh1710/zuordnung.md
ue03/dsch/anforderungen.md
ue03/dsch/kontext.md
ue03/dsch/zuordnung.md
ue03/ecib/anforderungen.md
ue03/ecib/kontext.md
ue03/ecib/zuordnung.md
ue03/emrano/anforderungen.md
ue03/emrano/kontext.md
ue03/emrano/zuordnung.md
ue03/en7-mj/anforderungen.md
ue03/en7-mj/kontext.md
ue03/en7-mj/zuordnung.md
ue03/ezen/anforderungen.md
ue03/ezen/kontext.md
ue03/ezen/zuordnung.md
ue03/fahm/anforderungen.md
ue03/fahm/kontext.md
ue03/fahm/zuordnung.md
ue03/flk/anforderungen.md
ue03/flk/kontext.md
ue03/flk/zuordnung.md
ue03/hfdr12/anforderungen.md
ue03/hfdr12/kontext.md
ue03/hfdr12/zuordnung.md
ue03/iaa/anforderungen.md
ue03/iaa/kontext.md
ue03/iaa/zuordnung.md
ue03/ilias04j/anforderungen.md
ue03/ilias04j/kontext.md
ue03/ilias04j/zuordnung.md
ue03/IY69/anforderungen.md
ue03/IY69/kontext.md
ue03/IY69/zuordnung.md
ue03/janp/anforderungen.md
ue03/janp/kontext.md
ue03/janp/zuordnung.md
ue03/javu/anforderungen.md
ue03/javu/kontext.md
ue03/javu/zuordnung.md
ue03/jemy/anforderungen.md
ue03/jemy/kontext.md
ue03/jemy/zuordnung.md
ue03/jsug/anforderungen.md
ue03/jsug/kontext.md
ue03/jsug/zuordnung.md
ue03/jvng/anforderungen.md
ue03/jvng/kontext.md
ue03/jvng/zuordnung.md
ue03/kraz/anforderungen.md
ue03/kraz/kontext.md
ue03/kraz/zuordnung.md
ue03/lkrs/anforderungen.md
ue03/lkrs/kontext.md
ue03/lkrs/zuordnung.md
ue03/lom/anforderungen.md
ue03/lom/kontext.md
ue03/lom/zuordnung.md
ue03/Lpr/anforderungen.md
ue03/Lpr/kontext.md
ue03/Lpr/zuordnung.md
ue03/masalabyte/anforderungen.md
ue03/masalabyte/kontext.md
ue03/masalabyte/zuordnung.md
ue03/maxbarrosschauer/anforderungen.md
ue03/maxbarrosschauer/kontext.md
ue03/maxbarrosschauer/zuordnung.md
ue03/mduc/anforderungen.md
ue03/mduc/kontext.md
ue03/mduc/zuordnung.md
ue03/meq/anforderungen.md
ue03/meq/kontext.md
ue03/meq/zuordnung.md
ue03/mjab/anforderungen.md
ue03/mjab/kontext.md
ue03/mjab/zuordnung.md
ue03/MK/anforderungen.md
ue03/MK/kontext.md
ue03/MK/zuordnung.md
ue03/mken/anforderungen.md
ue03/mken/kontext.md
ue03/mken/zuordnung.md
ue03/mkon/anforderungen.md
ue03/mkon/kontext.md
ue03/mkon/zuordnung.md
ue03/moh/anforderungen.md
ue03/moh/kontext.md
ue03/moh/zuordnung.md
ue03/mpal/anforderungen.md
ue03/mpal/kontext.md
ue03/mpal/zuordnung.md
ue03/mskk15/anforderungen.md
ue03/mskk15/kontext.md
ue03/mu/anforderungen.md
ue03/mu/kontext.md
ue03/mu/zuordnung.md
ue03/mw/anforderungen.md
ue03/mw/kontext.md
ue03/mw/zuordnung.md
ue03/my55/anforderungen.md
ue03/my55/kontext.md
ue03/my55/zuordnung.md
ue03/nicolino/anforderungen.md
ue03/nicolino/kontext.md
ue03/nicolino/zuordnung.md
ue03/nko/anforderungen.md
ue03/nko/kontext.md
ue03/nko/zuordnung.md
ue03/nly50/anforderungen.md
ue03/nly50/kontext.md
ue03/nly50/zuordnung.md
ue03/NN/anforderungen.md
ue03/NN/kontext.md
ue03/NN/zuordnung.md
ue03/nohl/anforderungen.md
ue03/nohl/kontext.md
ue03/nohl/zuordnung.md
ue03/NUAli/anforderungen.md
ue03/NUAli/kontext.md
ue03/NUAli/zuordnung.md
ue03/onzj/anforderungen.md
ue03/onzj/kontext.md
ue03/onzj/zuordnung.md
ue03/oubou/anforderungen.md
ue03/oubou/kontext.md
ue03/oubou/zuordnung.md
ue03/pdam/anforderungen.md
ue03/pdam/kontext.md
ue03/pdam/zuordnung.md
ue03/pgml/anforderungen.md
ue03/pgml/kontext.md
ue03/pgml/zuordnung.md
ue03/pz01/anforderungen.md
ue03/pz01/kontext.md
ue03/pz01/zuordnung.md
ue03/qho/anforderungen.md
ue03/qho/kontext.md
ue03/qho/zuordnung.md
ue03/README.md
ue03/real/anforderungen.md
ue03/real/kontext.md
ue03/real/zuordnung.md
ue03/sahmad/anforderungen.md
ue03/sahmad/kontext.md
ue03/sahmad/zuordnung.md
ue03/sahmed/anforderungen.md
ue03/sahmed/kontext.md
ue03/sahmed/zuordnung.md
ue03/sam/anforderungen.md
ue03/sam/kontext.md
ue03/sam/zuordnung.md
ue03/skrl78/anforderungen.md
ue03/skrl78/kontext.md
ue03/skrl78/zuordnung.md
ue03/snab/anforderungen.md
ue03/snab/kontext.md
ue03/snab/zuordnung.md
ue03/sngu/anforderungen.md
ue03/sngu/kontext.md
ue03/sngu/zuordnung.md
ue03/sraks/anforderungen.md
ue03/sraks/kontext.md
ue03/sraks/zuordnung.md
ue03/ssda78/anforderungen.md
ue03/ssda78/kontext.md
ue03/ssda78/zuordnung.md
ue03/sshj44/anforderungen.md
ue03/sshj44/kontext.md
ue03/sshj44/zuordnung.md
ue03/stmx/anforderungen.md
ue03/stmx/kontext.md
ue03/stmx/zuordnung.md
ue03/talh/anforderungen.md
ue03/talh/kontext.md
ue03/talh/zuordnung.md
ue03/TariqK2004/anforderungen.md
ue03/TariqK2004/kontext.md
ue03/TariqK2004/zuordnung.md
ue03/tcam/anforderungen.md
ue03/tcam/kontext.md
ue03/tcam/zuordnung.md
ue03/tiger/anforderungen.md
ue03/tiger/kontext.md
ue03/tiger/zuordnung.md
ue03/tnd/anforderungen.md
ue03/tnd/kontext.md
ue03/tnd/zuordnung.md
ue03/trry/anforderungen.md
ue03/trry/kontext.md
ue03/trry/zuordnung.md
ue03/tyfncc/anforderungen.md
ue03/tyfncc/kontext.md
ue03/tyfncc/zuordnung.md
ue03/uwar/anforderungen.md
ue03/uwar/kontext.md
ue03/uwar/zuordnung.md
ue03/val/anforderungen.md
ue03/val/kontext.md
ue03/val/zuordnung.md
ue03/vic26/anforderungen.md
ue03/vic26/kontext.md
ue03/vic26/zuordnung.md
ue03/virus/anforderungen.md
ue03/virus/kontext.md
ue03/virus/zuordnung.md
ue03/wnga/anforderungen.md
ue03/wnga/kontext.md
ue03/wnga/zuordnung.md
ue03/ygue/anforderungen.md
ue03/ygue/kontext.md
ue03/ygue/zuordnung.md
ue03/ykar/anforderungen.md
ue03/ykar/kontext.md
ue03/ykar/zuordnung.md
ue03/z-266/anforderungen.md
ue03/z-266/kontext.md
ue03/z-266/zuordnung.md
ue03/zc/anforderungen.md
ue03/zc/kontext.md
ue03/zc/zuordnung.md
ue03/zcbn/anforderungen.md
ue03/zcbn/kontext.md
ue03/zcbn/zuordnung.md
ue03/zcoel/anforderungen.md
ue03/zcoel/kontext.md
ue03/zcoel/zuordnung.md
ue03/zsh/anforderungen.md
ue03/zsh/kontext.md
ue03/zsh/zuordnung.md
ue04/_vorlage/einrichtung.md
ue04/mskk155/einrichtung.md
ue04/README.md


**Tool: shell**

**Input:**
```json
{
  "command": "find ue04/mskk155 -type f | sort | while read f; do echo \"--- $f\"; cat \"$f\"; done"
}
```

--- ue04/mskk155/einrichtung.md
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


**Tool: shell**

**Input:**
```json
{
  "command": "cat ue04/README.md; echo '--- ue01'; ls ue01; echo '--- ue04'; ls -la ue04"
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
--- ue01
README.md
steckbriefe
--- ue04
total 8
drwxr-xr-x@ 3 mariamsekkali  staff    96 Nov  5 16:46 _vorlage
drwxr-xr-x@ 5 mariamsekkali  staff   160 Nov  5 16:48 .
drwxr-xr-x@ 9 mariamsekkali  staff   288 Nov  5 16:46 ..
drwxr-xr-x@ 3 mariamsekkali  staff    96 Nov  5 16:48 mskk155
-rw-r--r--@ 1 mariamsekkali  staff  1994 Nov  5 16:46 README.md


---

## Assistant

_Thinking:_

The user's branch is ue04-mskk155, own dir ue04/mskk155. Existing ue03/mskk15 exists (older abbreviation maybe theirs?) and ue01/steckbriefe/mskk15.md. Need to determine which files come from the user. Branch name says mskk155. ue03/mskk15 — "Ältere Verzeichnisse können stattdessen ein früher gewähltes Kürzel tragen; sie gehören trotzdem der Person." But is mskk15 the same person as mskk155? Probably yes typo/different. We should be careful: "Ist unklar, welche Verzeichnisse ihr gehören, frage nach, statt es zu raten."

Let me check git log for ue03/mskk15 authorship and steckbrief content, and confirm branch remote. Also check whether sitzung.md exists (not yet). Let's inspect those files.

**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline -- ue03/mskk15 ue01/steckbriefe/mskk15.md | head -20; git log -1 --format='%an <%ae>%n%ad%n%s' -- ue03/mskk15; git log -1 --format='%an <%ae>%n%ad%n%s' -- ue01/steckbriefe/mskk15.md"
}
```

47056ae Aufgaben 1 und 3 bearbeiten (#305)
85b6c9c Steckbrief erstellen (#78)
mskk155 <mariam.sekkali@mnd.thm.de>
Mon Nov 2 14:32:03 2026 +0100
Aufgaben 1 und 3 bearbeiten (#305)
mskk155 <mariam.sekkali@mnd.thm.de>
Tue Oct 20 21:14:52 2026 +0200
Steckbrief erstellen (#78)


**Tool: read**

**Input:**
```json
{
  "path": "ue01/steckbriefe/mskk15.md"
}
```

Read file ue01/steckbriefe/mskk15.md, lines 1-14
1: # Steckbrief <mskk155>
2: 
3: ## Studiengang und Semester
4: Wirtschaftsinformatik, 3.Semester
5: …
6: 
7: ## Meine bisherige Erfahrung mit Softwareentwicklung
8: Keine erfahrungen in der Softwareentwicklung.Erste Grundlagen im Programmieren habe ich bereits in Java kennengelernt.
9: …
10: 
11: ## Das erwarte ich von der Veranstaltung
12: Die Grundlagen der Softwareentwichlung besser verstehen und lernen.
13: Umgang mit Git, GitHub ubd Visual Studio Code lernen.
14: …

**Tool: shell**

**Input:**
```json
{
  "command": "cat ue03/mskk15/kontext.md; echo '--- anforderungen'; cat ue03/mskk15/anforderungen.md; echo '--- status'; git status --porcelain=v1 -uall"
}
```

# Stakeholder und Systemkontext — Terminplaner für die THM



## Stakeholder



| Stakeholder | Worauf hat er Einfluss? |
| Studierender | Sie möchten freie Sprechstundentermine finden und buchen.|
| Lehrende | Sie legen ihre verfügbaren Sprechstundenzeiten fest und entscheiden, welche Termine angeboten werden. |
|Sekreteriat| 

Es unterstützt die Organisation von Terminen und pflegt gegebenenfalls Termindaten.|
|Fachbereichsleitung|Sie hat Interesse an einer guten Organisation der Sprechstunden und an einer effizienten Nutzung der Arbeitszeit.|
|IT-Abteilung der THM|Sie ist für den technischen Betrieb, die Wartung und die Sicherheit des Systems relevant.|
|Datenschutzbeauftragte der THM|Sie achtet darauf, dass personenbezogene Daten geschützt und Datenschutzvorgaben eingehalten werden.|
|Hochschulleitung|Sie hat Interesse an einer zuverlässigen und effizienten digitalen Verwaltung der Hochschule.|
## Systemkontext


| Aspekt | Art | Warum gehört er zum Kontext? |
|Studierende, die Sprechstundentermine buchen|Person|Sie benutzen den Terminplaner, sind aber nicht Teil des Systems selbst.|
| Lehrende, die Sprechstunden anbieten | Person | Sie stellen freie Termine bereit und verwalten ihre Verfügbarkeit.|
|Sekretariat der THM| Person|Es unterstützt die Terminorganisation außerhalb des eigentlichen Systems.|
|Hochschul-Login|System im betrieb| Es ermöglicht die Anmeldung der Benutzer mit ihrem Hochschulkont.|
|Buchung einer Sprechstunde|Prozess|Dabei sucht eine studierende Person einen freien Termin und bucht ihn.|

## Irrelevante Umgebung

   - Die Mensa der THM ist für den Terminplaner irrelevant, weil sie keinen Einfluss auf die Buchung von Sprechstundenterminen hat.
- Die Parkplatzbelegung der THM ist für den Terminplaner irrelevant, weil sie weder die Verfügbarkeit noch die Buchung von Sprechstunden bestimmt.

--- anforderungen
# Anforderungen — Terminplaner für die THM

| Nr.|	Anforderung |	Stakeholder| Art
|A01| Studierende können freie Sprechstundentermine bei einer Lehrperson buchen.| Studierende| FA |
|A02	| Lehrende können ihre verfügbaren Sprechstundenzeiten eintragen und ändern.| Lehrende|FA |
|A03	| Studierende können ihre gebuchten Termine einsehen.| Studierende| FA|
|A04	| Studierende können einen gebuchten Termin stornieren.| Studierende| FA|
|A05 |	Lehrende können eine Übersicht ihrer gebuchten Termine anzeigen lassen.| Lehrende|FA|
|A06	| Das System schützt personenbezogene Daten vor unberechtigtem Zugriff.| Datenschutzbeauftragte| QA|
|A07|	Eine Terminbuchung soll in höchstens drei Schritten möglich sein.|Studierende| QA| 
|A08	| Das System soll auch bei vielen gleichzeitigen Benutzern zuverlässig funktionieren.	|IT-Abteilung	| QA| 
|A09	| Die Anmeldung erfolgt ausschließlich über das Hochschulkonto der THM.| IT-Abteilung| RB| 
|A10	| Ein bereits gebuchter Termin kann nicht ein zweites Mal gebucht werden.| Lehrende| RB|


## Eine Anforderung, die niemand ausgesprochen hat

A10
Diese Anforderung wurde möglicherweise nicht ausdrücklich genannt, weil selbstverständlich sein sollte, dass jeder Termin nur einmal vergeben wird. Ohne diese Regel könnten mehrere Studierende denselben Termin buchen.
 genannt hat.

…
--- status
?? ue04/mskk155/einrichtung.md


**Tool: shell**

**Input:**
```json
{
  "command": "git remote -v; git branch -a"
}
```

origin	https://github.com/mskk155/thm_wk-1208_softwaretechnik-uebungen.git (fetch)
origin	https://github.com/mskk155/thm_wk-1208_softwaretechnik-uebungen.git (push)
upstream	https://github.com/carstenlucke/thm_wk-1208_softwaretechnik-uebungen.git (fetch)
upstream	https://github.com/carstenlucke/thm_wk-1208_softwaretechnik-uebungen.git (push)
  main
  steckbrief-mskk155
  ue02-mmskk155
  ue03-mmsk155
* ue04-mskk155
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/steckbrief-mskk155
  remotes/origin/ue02-mmskk155
  remotes/origin/ue03-mmsk155
  remotes/upstream/main
  remotes/upstream/steckbrief-clu


---

## Assistant

_Thinking:_

Confirmed: same author mskk155 <mariam.sekkali@mnd.thm.de>. So own files: ue01/steckbriefe/mskk15.md, ue03/mskk15/* (anforderungen.md, kontext.md; no zuordnung), ue04/mskk155/einrichtung.md (untracked, empty template). Wait, do ue02 own files exist? ue02 has no mskk15/mskk155 directory? Looking at list: ue02/... no mskk155 or mskk15. Branch ue02-mmskk155 exists but maybe no merged content. Let's check git log for author mskk155 across all files to identify any other own files.

**Tool: shell**

**Input:**
```json
{
  "command": "git log --all --author='mskk155' --name-only --format='%h %ad %s' --date=short | sed '/^$/d'"
}
```

3f97a10 2026-11-05 On ue04-mskk155: Sicherung vor Aufgabe 4
427c486 2026-11-05 index on ue04-mskk155: b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
56af870 2026-11-05 untracked files on ue04-mskk155: b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
ue02/_vorlage/notiz.md
ue02/_vorlage/spezifikation.md
ue03/README.md
ue03/_vorlage/anforderungen.md
ue03/_vorlage/kontext.md
ee5720f 2026-11-05 Anforderungen vervollständigt
ue03/mskk15/anforderungen.md
3004f71 2026-11-05 Eigene Anforderungen ergänzt
ue03/mskk15/anforderungen.md
d46266f 2026-11-05 Zuordnung Anforderungen oder Lösung
ue03/mskk15/zuordnung.md
47056ae 2026-11-02 Aufgaben 1 und 3 bearbeiten (#305)
ue03/mskk15/anforderungen.md
ue03/mskk15/kontext.md
57d79b1 2026-10-27 Aufgaben 1 und 3 bearbeiten
ue03/mmsk155/anforderungen.md
ue03/mmsk155/kontext.md
ue03/mmsk155/spezifikation.md
ac3346a 2026-10-26 Bearbeite Uebung 02
ue02/mmskk155/notiz.md
ue02/mmskk155/phasenplan.md
ue02/mmskk155/spezifikation.md
85b6c9c 2026-10-20 Steckbrief erstellen (#78)
ue01/steckbriefe/mskk15.md
d00319f 2026-10-19 Steckbrief erstellen
ue01/steckbriefe/mskk155


**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline --all -- ue02/mmskk155 ue02/mskk155 ue02/mskk15; git ls-tree -r --name-only ue02-mmskk155 -- ue02/ 2>/dev/null | grep -i mskk; git ls-tree -r --name-only ue03-msk155 -- ue03/ 2>/dev/null | grep -i mskk"
}
```

ac3346a Bearbeite Uebung 02
ue02/mmskk155/notiz.md
ue02/mmskk155/phasenplan.md
ue02/mmskk155/spezifikation.md

Exited with code 1

---

## Assistant

_Thinking:_

Interesting: own files include ue02/mmskk155 (older abbreviation with extra m), ue03/mmsk155 (another older abbreviation), ue03/mskk15, ue01/steckbriefe/mskk15.md, and maybe ue01/steckbriefe/mskk155 (from d00319f, but that path may have been renamed). All authored by mskk155 email. Need to determine what's in working tree vs branches. ue02/mmskk155 not present in current tree (list had no mmskk155). ue03/mmsk155 also not present. Possibly renamed via PR? Let's check git history for renames. Actually current branch is based on upstream main which includes commits from user's PRs merged: ue01/mskk15.md, ue03/mskk15. The other branches are unmerged local branches.

Question: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" They want overview and which files are theirs. Need to explain repository structure (ue01-ue04), plus own files on current branch and possibly unmerged branches. Let's identify own files in working tree via author. Only current merged: ue01/steckbriefe/mskk15.md, ue03/mskk15/anforderungen.md, ue03/mskk15/kontext.md, and untracked ue04/mskk155/einrichtung.md (template copy, not filled). ue02 own files are on branch ue02-mmskk155 but not merged? Wait local branch ue02-mmskk155 exists. Let's check its contents and whether a PR was merged under different path. ue02 list doesn't include mmskk155, and history for ue02 only shows the unmerged commit ac3346a? `git log --all --author` shows files. Let's see branches containing ac3346a and whether merged into main. Also ue03/mmsk155 branch.

Also check whether ue03/mskk15/zuordnung.md is on local branch but not main? The current working tree list showed ue03/mskk15 only anforderungen and kontext. So zuordnung commits d46266f, 3004f71, ee5720f are on ue03-msk155? Let's inspect.

Also there might be a stash. The `git log --all --author` first commits 3f97a10, 427c486, 56af870 are stash entries ("Sicherung vor Aufgabe 4", index..., untracked files...). Those include ue02/_vorlage etc. from stash. Not actual own files, but worth noting a stash exists.

Let me gather branch info, and status of files.

**Tool: shell**

**Input:**
```json
{
  "command": "for b in steckbrief-mskk155 ue02-mmskk155 ue03-msk155 ue04-mskk155; do echo \"### $b\"; git log --oneline -3 \"$b\"; git diff --stat main...\"$b\" 2>/dev/null; done"
}
```

### steckbrief-mskk155
d00319f Steckbrief erstellen
b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
43c75e2 Abschlussart ergänzt und Semester in neuer Zeile
 ue01/steckbriefe/mskk155 | 14 ++++++++++++++
 1 file changed, 14 insertions(+)
### ue02-mmskk155
ac3346a Bearbeite Uebung 02
b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
43c75e2 Abschlussart ergänzt und Semester in neuer Zeile
 ue02/mmskk155/notiz.md         | 26 +++++++++++++++++
 ue02/mmskk155/phasenplan.md    | 63 ++++++++++++++++++++++++++++++++++++++++++
 ue02/mmskk155/spezifikation.md | 47 +++++++++++++++++++++++++++++++
 3 files changed, 136 insertions(+)
### ue03-msk155
fatal: ambiguous argument 'ue03-msk155': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
### ue04-mskk155
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)


**Tool: shell**

**Input:**
```json
{
  "command": "echo '--- stash'; git stash list; echo '--- branches containing own commits'; for c in ac3346a d46266f 3004f71 ee5720f 85b6c9c 47056ae; do printf '%s: ' \"$c\"; git branch -a --contains \"$c\" | tr '\\n' ' '; echo; done"
}
```

--- stash
stash@{0}: On ue04-mskk155: Sicherung vor Aufgabe 4
--- branches containing own commits
ac3346a:   ue02-mmskk155   remotes/origin/ue02-mmskk155 
d46266f:   ue03-mmsk155   remotes/origin/ue03-mmsk155 
3004f71:   ue03-mmsk155   remotes/origin/ue03-mmsk155 
ee5720f:   ue03-mmsk155   remotes/origin/ue03-mmsk155 
85b6c9c:   main * ue04-mskk155   remotes/origin/HEAD -> origin/main   remotes/origin/main   remotes/upstream/main 
47056ae:   main * ue04-mskk155   remotes/origin/HEAD -> origin/main   remotes/origin/main 


**Tool: shell**

**Input:**
```json
{
  "command": "git ls-tree -r --name-only ue03-msk155 | grep -i 'ue03/msk'; echo '--- diff main ue03'; git diff --name-status main...ue03-msk155; echo '--- diff main ue02'; git diff --name-status main...ue02-mmskk155; echo '--- diff main steckbrief'; git diff --name-status main...steckbrief-mskk155"
}
```

fatal: Not a valid object name ue03-msk155
--- diff main ue03
fatal: ambiguous argument 'main...ue03-msk155': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
--- diff main ue02
A	ue02/mmskk155/notiz.md
A	ue02/mmskk155/phasenplan.md
A	ue02/mmskk155/spezifikation.md
--- diff main steckbrief
A	ue01/steckbriefe/mskk155


---

## Assistant

_Thinking:_

Branch name is ue03-msk155 (one k? "msk155"). `git branch -a` showed "ue03-mmsk155"? Let me re-read: output branch list: `ue03-mmsk155`? It displayed:

```
  ue02-mmskk155
  ue03-mmsk155
```

Actually first branch list output said "ue03-msk155"? It said `ue03-mmsk155`? Let me look: 
```
  ue02-mmskk155
  ue03-msk155
```
The string was "ue03-msk155" in my command loop? I used ue03-msk155 and it failed. Branch containing d46266f showed "ue03-msk155" twice? Wait output says "ue03-msk155" both local and remote. But command loop used "ue03-msk155"? Let me check exact characters. In output: `ue03-msk155:   ue03-msk155   remotes/origin/ue03-msk155` — hmm. My loop had `ue03-msk155`? The branch list earlier: `ue03-mmsk155`? Let me just list branches with quoting.

**Tool: shell**

**Input:**
```json
{
  "command": "git for-each-ref --format='%(refname:short)' refs/heads refs/remotes; echo '---'; for b in $(git for-each-ref --format='%(refname:short)' refs/heads); do printf '<%s>\\n' \"$b\"; done"
}
```

main
steckbrief-mskk155
ue02-mmskk155
ue03-mmsk155
ue04-mskk155
origin/HEAD
origin/main
origin/steckbrief-mskk155
origin/ue02-mmskk155
origin/ue03-mmsk155
upstream/main
upstream/steckbrief-clu
---
<main>
<steckbrief-mskk155>
<ue02-mmskk155>
<ue03-mmsk155>
<ue04-mskk155>


**Tool: shell**

**Input:**
```json
{
  "command": "git ls-tree -r --name-only $(git for-each-ref --format='%(refname:short)' refs/heads | grep ue03) | grep -i 'ue03/'"
}
```

ue03/mskk15/anforderungen.md
ue03/mskk15/kontext.md
ue03/mskk15/zuordnung.md


---

## Assistant

_Thinking:_

I typo'd missing k. Branch ue03-mmsk155 (two m's: mmsk155). Okay.

Let's inspect diff for ue03 branch and contents maybe own files. Also note ue01/steckbriefe/mskk155 vs mskk15.md. The branch steckbrief-mskk155 adds mskk155 but main has merged version mskk15.md via PR #78. How did that happen? d00319f created ue01/steckbriefe/mskk155 but merged commit 85b6c9c has mskk15.md. Maybe renamed during PR merge. Fine.

Need answer in German. Summarize repo structure: exercise dirs ue01-ue04 with many student subdirs; own identification by git author email mskk155.

Own files currently in main/working tree:
- ue01/steckbriefe/mskk15.md (Steckbrief; despite name mskk15, content header says mskk155; authored by mskk155)
- ue03/mskk15/anforderungen.md and kontext.md (committed on main via PR #305)
- ue04/mskk155/einrichtung.md (untracked, copy of template, currently only placeholders)

Own but not merged / on other branches:
- branch ue02-mmskk155: ue02/mmskk155/{notiz,phasenplan,spezifikation}.md — not on main
- branch ue03-mmsk155: ue03/mskk15/zuordnung.md plus newer edits to anforderungen.md — not on main (main has earlier version from PR #305). Wait the branch ue03-mmsk155 points to ee5720f with zuordnung and updates. The main has 47056ae version. So the branch has unmerged additional work. Let's confirm diff main...ue03-mmsk155.
- branch steckbrief-mskk155: ue01/steckbriefe/mskk155 (old path, superseded by mskk15.md on main).
- stash@{0} contains uncommitted changes incl. templates (ue02/_vorlage, ue03 README/vorlagen) — that's odd, likely agent work? Actually stash titled "Sicherung vor Aufgabe 4" includes these paths because maybe autostash on pull. It may include modifications to templates which shouldn't be committed. Do we mention? The user asked what's there and which files theirs. Mention a stash exists containing changes (possibly not theirs) is useful.

Wait, current branch ue04-mskk155 is at b5dbd3a (same as main) with untracked ue04/mskk155. Branch log showed b5dbd3a etc. So the branch has no commits yet; only untracked file. Good.

Let's get diff names for ue03 branch and stash names.

**Tool: shell**

**Input:**
```json
{
  "command": "git diff --name-status main...ue03-mmsk155; echo '--- contents zuordnung (branch)'; git show ue03-mmsk155:ue03/mskk15/zuordnung.md | head -40; echo '--- stash files'; git stash show --name-status stash@{0}"
}
```

A	ue03/mskk15/anforderungen.md
A	ue03/mskk15/kontext.md
A	ue03/mskk15/zuordnung.md
--- contents zuordnung (branch)
# Anforderung oder Lösung? — Terminplaner für die THM

GitHub-Benutzername: mskk155

## Funktionale Anforderung (FA)

- Studierende können einen freien Sprechstundentermin bei einer Lehrperson buchen.
- Ein bereits gebuchter Termin kann kein zweites Mal gebucht werden.
- Sagt eine Lehrperson eine Sprechstunde ab, erhalten alle, die gebucht haben, eine Nachricht.
- Jeder gebuchte Termin lässt sich als iCal-Datei herunterladen.
- Ein Sekretariat sieht alle Prüfungstermine seines Fachbereichs auf einen Blick.
- Über die API kann ein KI-Agent freie Termine abfragen und im Namen einer Person buchen.

## Qualitätsanforderung (QA)

- Eine Buchung ist für Studierende in höchstens drei Schritten abgeschlossen.
- Auch zu Beginn der Prüfungsanmeldung, wenn bis zu 2.000 Personen zugleich buchen, zeigt das System eine Seite in weniger als zwei Sekunden an.
- Die Buchungsseite ist mit einem Screenreader vollständig bedienbar.

## Randbedingung (RB)

- Die Anmeldung erfolgt ausschließlich über das Hochschulkonto.
- Die erste Ausbaustufe geht zum Sommersemester 2027 in Betrieb.
- Personenbezogene Daten werden nach den Vorgaben der EU-DSGVO verarbeitet.
- Das System wird im Rechenzentrum der THM betrieben.

## Keine Anforderung — Lösung (WIE)

- Die API nimmt Anfragen als REST-Aufrufe entgegen und antwortet in JSON.
- Vor jeder Buchung fragt die Komponente „Buchung“ bei der Komponente „Kalender“ an, ob der Termin noch frei ist.
- Termine werden in einer PostgreSQL-Datenbank gespeichert.

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue03-anforderung-oder-loesung: k01=fa k02=wie k03=rb k04=qa k05=fa k06=rb k07=wie k08=fa k09=rb k10=qa k11=wie k12=fa k13=qa k14=fa k15=rb k16=fa | unsicher: – -->
--- stash files


**Tool: shell**

**Input:**
```json
{
  "command": "git log --format='%h %an <%ae>' -1 main; git log --format='%h %an <%ae>' -1 ue02-mmskk155; git log --format='%h %an <%ae>' -1 ue03-mmsk155; git log --format='%h %an <%ae>' -1 steckbrief-mskk155"
}
```

b5dbd3a THM-Nos <nossair.belhaj@mnd.thm.de>
ac3346a mskk155 <Mariam.sekkali@mnd.thm.de>
ee5720f mskk155 <Mariam.sekkali@mnd.thm.de>
d00319f mskk155 <Mariam.sekkali@mnd.thm.de>


---

## Assistant

_Thinking:_

Interesting: `git diff --name-status main...ue03-mmsk155` says all three files added (A), meaning branch is not based on latest main? Actually three-dot diff compares merge base; if branch forked before PR #305, then all added. Let's check merge-base. Branch may contain files identical to main for two. `git diff main..ue03-mmsk155 --stat` would show only changed. Let's check.

Also stash show names empty? It might be a merge commit stash with nothing? `git stash show` default shows diff against first parent, but stash has index/untracked commits. Let's inspect `git stash show -p --include-untracked` or list tree. Not vital. But maybe mention stash contains a snapshot. Let's check quickly.

Also need clarify own files by author. The branch ue04-mskk155 has no own commits yet. ue04/mskk155/einrichtung.md untracked is a template copy, no content filled. It is "von dir" in the sense you created it, but it's an unchanged copy of template. Mention.

Let's determine whether ue03/mmsk155 branch is merged? Branch ue03-mmsk155 not in main; main's own files came from PR #305 (47056ae), which is a merge commit? `git log -1 47056ae` shown as "Aufgaben 1 und 3 bearbeiten (#305)" with author mskk155, likely squash merge. Branch ee5720f later has extra zuordnung and edits, unmerged.

Check diff main..ue03-mmsk155.

**Tool: shell**

**Input:**
```json
{
  "command": "git diff --stat main..ue03-mmsk155; echo '---'; git diff --name-status main..ue03-mmsk155; echo '--- merge-base'; git merge-base main ue03-mmsk155; git log --oneline -3 $(git merge-base main ue03-mmsk155)"
}
```

/notiz.md                     |  33 ------
 ue02/athr/phasenplan.md                |  63 -----------
 ue02/athr/spezifikation.md             |  36 ------
 ue02/avon507/notiz.md                  |  32 ------
 ue02/avon507/phasenplan.md             |  66 -----------
 ue02/avon507/spezifikation.md          |  18 ---
 ue02/ayue/notiz.md                     |  25 ----
 ue02/ayue/phasenplan.md                |  61 ----------
 ue02/ayue/spezifikation.md             |  42 -------
 ue02/bblj09/notiz.md                   |  27 -----
 ue02/bblj09/phasenplan.md              |  63 -----------
 ue02/bblj09/spezifikation.md           |  20 ----
 ue02/bima/notiz.md                     |  35 ------
 ue02/bima/phasenplan.md                |  67 -----------
 ue02/bima/spezifikation.md             |  26 -----
 ue02/datr03/notiz.md                   |  39 -------
 ue02/datr03/phasenplan.md              |  63 -----------
 ue02/datr03/spezifikation.md           |  48 --------
 ue02/div/notiz.md                      |  37 ------
 ue02/div/phasenplan.md                 |  65 -----------
 ue02/div/rollen.md                     |  34 ------
 ue02/div/spezifikation.md              |  28 -----
 ue02/dlm28/notiz.md                    |  25 ----
 ue02/dlm28/phasenplan.md               |  63 -----------
 ue02/dlm28/spezifikation.md            |  16 ---
 ue02/dmmh1710/notiz.md                 |  26 -----
 ue02/dmmh1710/phasenplan.md            |  63 -----------
 ue02/dmmh1710/spezifikation.md         |  16 ---
 ue02/dsc/notiz.md                      |  34 ------
 ue02/dsc/phasenplan.md                 |  64 -----------
 ue02/dsc/spezifikation.md              |  57 ----------
 ue02/dsch/notiz.md                     |  37 ------
 ue02/dsch/phasenplan.md                |  66 -----------
 ue02/dsch/spezifikation.md             |  35 ------
 ue02/dszp/notiz.md                     |  35 ------
 ue02/dszp/phasenplan.md                |  63 -----------
 ue02/dszp/spezifikation.md             |  27 -----
 ue02/emrano/notiz.md                   |  28 -----
 ue02/emrano/phasenplan.md              |  63 -----------
 ue02/emrano/spezifikation.md           |  58 ----------
 ue02/en7-mj/notiz.md                   |  26 -----
 ue02/en7-mj/phasenplan.md              |  64 -----------
 ue02/en7-mj/spezifikation.md           |  28 -----
 ue02/ezen/notiz.md                     |  27 -----
 ue02/ezen/phasenplan.md                |  63 -----------
 ue02/ezen/spezifikation.md             |  31 -----
 ue02/fahm/notiz.md                     |  30 -----
 ue02/fahm/phasenplan.md                |  63 -----------
 ue02/fahm/spezifikation.md             |  13 ---
 ue02/flk/notiz.md                      |  28 -----
 ue02/flk/phasenplan.md                 |  64 -----------
 ue02/flk/spezifikation.md              |  27 -----
 ue02/fortnitepro/notiz.md              |  37 ------
 ue02/fortnitepro/phasenplan.md         |  69 -----------
 ue02/fortnitepro/spezifikation.md      |  39 -------
 ue02/hams/notiz.md                     |  42 -------
 ue02/hams/phasenplan.md                |  63 -----------
 ue02/hams/spezifikation.md             |  57 ----------
 ue02/hfdr12/notiz.md                   |  33 ------
 ue02/hfdr12/phasenplan.md              |  63 -----------
 ue02/hfdr12/spezifikation.md           |  25 ----
 ue02/iaa/notiz.md                      |  37 ------
 ue02/iaa/phasenplan.md                 |  63 -----------
 ue02/iaa/spezifikation.md              |  28 -----
 ue02/iesp/notiz.md                     |  30 -----
 ue02/iesp/phasenplan.md                |  63 -----------
 ue02/iesp/spezifikation.md             |  32 ------
 ue02/ilias04j/notiz.md                 |  31 -----
 ue02/ilias04j/phasenplan.md            |  63 -----------
 ue02/ilias04j/spezifikation.md         |  29 -----
 ue02/ivlbs/notiz.md                    |  46 --------
 ue02/ivlbs/phasenplan.md               |  63 -----------
 ue02/ivlbs/spezifikation.md            |  30 -----
 ue02/janp/notiz.md                     |  27 -----
 ue02/janp/phasenplan.md                |  63 -----------
 ue02/janp/rollen.md                    |  34 ------
 ue02/janp/spezifikation.md             |  65 -----------
 ue02/javu11/notiz.md                   |  26 -----
 ue02/javu11/phasenplan.md              |  67 -----------
 ue02/javu11/rollen.md                  |  35 ------
 ue02/javu11/spezifikation.md           |  65 -----------
 ue02/jemy/notiz.md                     |  33 ------
 ue02/jemy/phasenplan.md                |  63 -----------
 ue02/jemy/rollen.md                    |  38 -------
 ue02/jemy/spezifikation.md             |  76 -------------
 ue02/jp26/notiz.md                     |  33 ------
 ue02/jp26/phasenplan.md                |  64 -----------
 ue02/jp26/spezifikation.md             |  30 -----
 ue02/jsug/notiz.md                     |  25 ----
 ue02/jsug/phasenplan.md                |  64 -----------
 ue02/jsug/spezifikation.md             |  43 -------
 ue02/jvng/notiz.md                     |  24 ----
 ue02/jvng/rollen.md                    |  35 ------
 ue02/jvng/spezifikation.md             |  22 ----
 ue02/kraz/notiz.md                     |  38 -------
 ue02/kraz/phasenplan.md                |  68 -----------
 ue02/kraz/spezifikation.md             | 100 ----------------
 ue02/lebr/notiz.md                     |  32 ------
 ue02/lebr/phasenplan.md                |  63 -----------
 ue02/lebr/spezifikation.md             |  35 ------
 ue02/lom/notiz.md                      |  37 ------
 ue02/lom/phasenplan.md                 |  63 -----------
 ue02/lom/spezifikation.md              |  44 --------
 ue02/mabl/notiz.md                     |  33 ------
 ue02/mabl/phasenplan.md                |  67 -----------
 ue02/mabl/spezifikation.md             |  47 --------
 ue02/masalabyte/notiz.md               |  26 -----
 ue02/masalabyte/phasenplan.md          |  46 --------
 ue02/masalabyte/spezifikation.md       |  23 ----
 ue02/maxbarrosschauer/notiz.md         |  35 ------
 ue02/maxbarrosschauer/phasenplan.md    |  63 -----------
 ue02/maxbarrosschauer/rollen.md        |  35 ------
 ue02/maxbarrosschauer/spezifikation.md |  79 -------------
 ue02/mbgrn04/notiz.md                  |  30 -----
 ue02/mbgrn04/phasenplan.md             |  63 -----------
 ue02/mbgrn04/spezifikation.md          |  16 ---
 ue02/mduc/notiz.md                     |  37 ------
 ue02/mduc/phasenplan.md                |  69 -----------
 ue02/mduc/spezifikation.md             |  81 -------------
 ue02/meq/notiz.md                      |  37 ------
 ue02/meq/phasenplan.md                 |  63 -----------
 ue02/meq/rollen.md                     |  34 ------
 ue02/meq/spezifikation.md              |  89 ---------------
 ue02/mf23/notiz.md                     |  25 ----
 ue02/mf23/phasenplan.md                |  75 ------------
 ue02/mf23/spezifikation.md             |  41 -------
 ue02/mjab/notiz.md                     |  33 ------
 ue02/mjab/phasenplan.md                |  66 -----------
 ue02/mjab/spezifikation.md             |  57 ----------
 ue02/mjas/notiz.md                     |  27 -----
 ue02/mjas/phasenplan.md                |  63 -----------
 ue02/mjas/spezifikation.md             |  88 ---------------
 ue02/mk/phasenplan.md                  |  63 -----------
 ue02/mkon/notiz.md                     |  29 -----
 ue02/mkon/phasenplan.md                |  63 -----------
 ue02/mkon/spezifikation.md             |  26 -----
 ue02/mpal/notiz.md                     |  25 ----
 ue02/mpal/phasenplan.md                |  63 -----------
 ue02/mpal/spezifikation.md             |  28 -----
 ue02/mu/notiz.md                       |  25 ----
 ue02/mu/phasenplan.md                  |  66 -----------
 ue02/mu/spezifikation.md               |  28 -----
 ue02/mw/notiz.md                       |  38 -------
 ue02/mw/phasenplan.md                  |  64 -----------
 ue02/mw/spezifikation.md               |  35 ------
 ue02/my55/notiz.md                     |  29 -----
 ue02/my55/phasenplan.md                |  63 -----------
 ue02/my55/spezifikation.md             |  25 ----
 ue02/ngh/notiz.md                      |  35 ------
 ue02/ngh/phasenplan.md                 |  63 -----------
 ue02/ngh/spezifikation.md              |  70 ------------
 ue02/nicolino/notiz.md                 |  27 -----
 ue02/nicolino/phasenplan.md            |  63 -----------
 ue02/nicolino/spezifikation.md         |  61 ----------
 ue02/nko/notiz.md                      |  24 ----
 ue02/nko/phasenplan.md                 |  63 -----------
 ue02/nko/spezifikation.md              |  29 -----
 ue02/nly50/notiz.md                    |  37 ------
 ue02/nly50/phasenplan.md               |  64 -----------
 ue02/nly50/spezifikation.md            |  19 ----
 ue02/nohl/notiz.md                     |  37 ------
 ue02/nohl/phasenplan.md                |  64 -----------
 ue02/nohl/spezifikation.md             |  30 -----
 ue02/oubou/notiz.md                    |  37 ------
 ue02/oubou/phasenplan.md               |  64 -----------
 ue02/oubou/spezifikation.md            |  18 ---
 ue02/pdam/notiz.md                     |  28 -----
 ue02/pdam/phasenplan.md                |  68 -----------
 ue02/pdam/spezifikation.md             |  33 ------
 ue02/pgml/notiz.md                     |  34 ------
 ue02/pgml/phasenplan.md                |  63 -----------
 ue02/pgml/spezifikation.md             |  31 -----
 ue02/pz01/notiz.md                     |  35 ------
 ue02/pz01/phasenplan.md                |  65 -----------
 ue02/pz01/spezifikation.md             |  44 --------
 ue02/qdb/notiz.md                      |  38 -------
 ue02/qdb/phasenplan.md                 |  63 -----------
 ue02/qdb/rollen.md                     |  34 ------
 ue02/qdb/spezifikation.md              |  44 --------
 ue02/qho/notiz.md                      |  26 -----
 ue02/qho/phasenplan.md                 |  63 -----------
 ue02/qho/spezifikation.md              |  20 ----
 ue02/real/notiz.md                     |  22 ----
 ue02/real/phasenplan.md                |  63 -----------
 ue02/real/spezifikation.md             |  31 -----
 ue02/renn/notiz.md                     |  26 -----
 ue02/renn/phasenplan.md                |  64 -----------
 ue02/renn/spezifikation.md             |  33 ------
 ue02/sahmad/notiz.md                   |  28 -----
 ue02/sahmad/phasenplan.md              |  63 -----------
 ue02/sahmad/spezifikation.md           |  44 --------
 ue02/sahmed/notiz.md                   |  35 ------
 ue02/sahmed/phasenplan.md              |  63 -----------
 ue02/sahmed/rollen.md                  |  35 ------
 ue02/sahmed/spezifikation.md           |  79 -------------
 ue02/sam/notiz.md                      |  35 ------
 ue02/sam/phasenplan.md                 |  63 -----------
 ue02/sam/spezifikation.md              |  28 -----
 ue02/skrl78/notiz.md                   |  25 ----
 ue02/skrl78/phasenplan.md              |  66 -----------
 ue02/skrl78/rollen.md                  |  34 ------
 ue02/skrl78/spezifikation.md           |  23 ----
 ue02/skt435/notiz.md                   |  28 -----
 ue02/skt435/spezifikation.md           |  15 ---
 ue02/snab/notiz.md                     |  29 -----
 ue02/snab/phasenplan.md                |  64 -----------
 ue02/snab/spezifikation.md             |  31 -----
 ue02/sngu/notiz.md                     |  36 ------
 ue02/sngu/phasenplan.md                |  63 -----------
 ue02/sngu/spezifikation.md             |  51 ---------
 ue02/ssda78/notiz.md                   |  37 ------
 ue02/ssda78/spezifikation.md           |  16 ---
 ue02/sshj44/notiz.md                   |  25 ----
 ue02/sshj44/phasenplan.md              |  63 -----------
 ue02/sshj44/spezifikation.md           | 123 --------------------
 ue02/ssng61/notiz.md                   |  26 -----
 ue02/ssng61/spezifikation.md           |  15 ---
 ue02/stmx/notiz.md                     |  27 -----
 ue02/stmx/phasenplan.md                |  64 -----------
 ue02/stmx/spezifikation.md             |  30 -----
 ue02/talh/notiz.md                     |  27 -----
 ue02/talh/phasenplan.md                |  63 -----------
 ue02/talh/rollen.md                    |  34 ------
 ue02/talh/spezifikation.md             |  18 ---
 ue02/tcam/notiz.md                     |  37 ------
 ue02/tcam/phasenplan.md                |  63 -----------
 ue02/tcam/spezifikation.md             | 105 -----------------
 ue02/thm-nos/notiz.md                  |  29 -----
 ue02/thm-nos/phasenplan.md             |  64 -----------
 ue02/thm-nos/spezifikation.md          |  18 ---
 ue02/thng/notiz.md                     |  41 -------
 ue02/thng/phasenplan.md                |  63 -----------
 ue02/thng/spezifikation.md             |  68 -----------
 ue02/tiger/notiz.md                    |  24 ----
 ue02/tiger/phasenplan.md               |  63 -----------
 ue02/tiger/spezifikation.md            |  60 ----------
 ue02/tnd/notiz.md                      |  29 -----
 ue02/tnd/phasenplan.md                 |  63 -----------
 ue02/tnd/spezifikation.md              |  27 -----
 ue02/tngan/notiz.md                    |  23 ----
 ue02/tngan/phasenplan.md               |  63 -----------
 ue02/tngan/spezifikation.md            |  16 ---
 ue02/trry/notiz.md                     |  25 ----
 ue02/trry/phasenplan.md                |  63 -----------
 ue02/trry/rollen.md                    |  32 ------
 ue02/trry/spezifikation.md             |  29 -----
 ue02/ttpr21/notiz.md                   |  25 ----
 ue02/ttpr21/phasenplan.md              |  65 -----------
 ue02/ttpr21/spezifikation.md           |  52 ---------
 ue02/tyfncc/notiz.md                   |  25 ----
 ue02/tyfncc/phasenplan.md              |  63 -----------
 ue02/tyfncc/rollen.md                  |  34 ------
 ue02/tyfncc/spezifikation.md           |  52 ---------
 ue02/uwar/notiz.md                     |  37 ------
 ue02/uwar/phasenplan.md                |  66 -----------
 ue02/uwar/spezifikation.md             | 134 ----------------------
 ue02/vic26/notiz.md                    |  25 ----
 ue02/vic26/phasenplan.md               |  62 ----------
 ue02/vic26/spezifikation.md            |  33 ------
 ue02/virus/notiz.md                    |  36 ------
 ue02/virus/phasenplan.md               |  65 -----------
 ue02/virus/spezifikation.md            |  65 -----------
 ue02/wnga/notiz.md                     |  37 ------
 ue02/wnga/phasenplan.md                |  63 -----------
 ue02/wnga/rollen.md                    |  34 ------
 ue02/wnga/spezifikation.md             |  24 ----
 ue02/ygue/notiz.md                     |  20 ----
 ue02/ygue/phasenplan.md                |  64 -----------
 ue02/ygue/spezifikation.md             |  22 ----
 ue02/ysbi82/notiz.md                   |  59 ----------
 ue02/ysbi82/spezifikation.md           |  48 --------
 ue02/zcbn/notiz.md                     |  32 ------
 ue02/zcbn/phasenplan.md                |  63 -----------
 ue02/zcbn/spezifikation.md             |  24 ----
 ue02/zcoel/notiz.md                    |  27 -----
 ue02/zcoel/phasenplan.md               |  63 -----------
 ue02/zcoel/spezifikation.md            |  31 -----
 ue02/zsh/notiz.md                      |  29 -----
 ue02/zsh/phasenplan.md                 |  66 -----------
 ue02/zsh/spezifikation.md              |  16 ---
 ue03/IY69/anforderungen.md             |  25 ----
 ue03/IY69/kontext.md                   |  33 ------
 ue03/IY69/zuordnung.md                 |  37 ------
 ue03/Lpr/anforderungen.md              |  16 ---
 ue03/Lpr/kontext.md                    |  25 ----
 ue03/Lpr/zuordnung.md                  |  35 ------
 ue03/MK/anforderungen.md               |  24 ----
 ue03/MK/kontext.md                     |  40 -------
 ue03/MK/zuordnung.md                   |  37 ------
 ue03/NN/anforderungen.md               |  18 ---
 ue03/NN/kontext.md                     |  30 -----
 ue03/NN/zuordnung.md                   |  37 ------
 ue03/NUAli/anforderungen.md            |  24 ----
 ue03/NUAli/kontext.md                  |  40 -------
 ue03/NUAli/zuordnung.md                |  37 ------
 ue03/README.md                         |  30 -----
 ue03/TariqK2004/anforderungen.md       |  15 ---
 ue03/TariqK2004/kontext.md             |  20 ----
 ue03/TariqK2004/zuordnung.md           |  37 ------
 ue03/_vorlage/anforderungen.md         |  19 ----
 ue03/_vorlage/kontext.md               |  31 -----
 ue03/aayd/anforderungen.md             |  17 ---
 ue03/aayd/kontext.md                   |  28 -----
 ue03/aayd/zuordnung.md                 |  39 -------
 ue03/af/anforderungen.md               |  17 ---
 ue03/af/kontext.md                     |  30 -----
 ue03/af/zuordnung.md                   |  40 -------
 ue03/agbr/anforderungen.md             |  17 ---
 ue03/agbr/kontext.md                   |  32 ------
 ue03/ahyi/anforderungen.md             |  28 -----
 ue03/ahyi/kontext.md                   |  43 -------
 ue03/ahyi/zuordnung.md                 |  37 ------
 ue03/akyf/anforderungen.md             |  19 ----
 ue03/akyf/kontext.md                   |  32 ------
 ue03/akyf/zuordnung.md                 |  35 ------
 ue03/anas23088/anforderungen.md        |  18 ---
 ue03/anas23088/kontext.md              |  27 -----
 ue03/anas23088/zuordnung.md            |  37 ------
 ue03/anddun/anforderungen.md           |  27 -----
 ue03/anddun/kontext.md                 |  46 --------
 ue03/anddun/zuordnung.md               |  37 ------
 ue03/andel0/anforderungen.md           |  20 ----
 ue03/andel0/kontext.md                 |  30 -----
 ue03/andel0/zuordnung.md               |  37 ------
 ue03/anpa/anforderungen.md             |  18 ---
 ue03/anpa/kontext.md                   |  31 -----
 ue03/anpa/zuordnung.md                 |  35 ------
 ue03/anushka/anforderungen.md          |  22 ----
 ue03/anushka/kontext.md                |  33 ------
 ue03/anushka/zuordnung.md              |  37 ------
 ue03/avon507/anforderungen.md          |  19 ----
 ue03/avon507/kontext.md                |  28 -----
 ue03/avon507/zuordnung.md              |  40 -------
 ue03/ayue/anforderungen.md             |  20 ----
 ue03/ayue/kontext.md                   |  37 ------
 ue03/ayue/zuordnung.md                 |  37 ------
 ue03/azm96/anforderungen.md            |  23 ----
 ue03/azm96/kontext.md                  |  28 -----
 ue03/azm96/zuordnung.md                |  37 ------
 ue03/bblj09/anforderungen.md           |  19 ----
 ue03/bblj09/kontext.md                 |  37 ------
 ue03/bblj09/zuordnung.md               |  37 ------
 ue03/bogh233/anforderungen.md          |  19 ----
 ue03/bogh233/kontext.md                |  28 -----
 ue03/bogh233/zuordnung.md              |  37 ------
 ue03/cms/anforderungen.md              |  21 ----
 ue03/cms/kontext.md                    |  36 ------
 ue03/cms/zuordnung.md                  |  38 -------
 ue03/davn68/anforderungen.md           |  16 ---
 ue03/davn68/kontext.md                 |  33 ------
 ue03/davn68/zuordnung.md               |  37 ------
 ue03/dlm28/anforderungen.md            |  24 ----
 ue03/dlm28/kontext.md                  |  29 -----
 ue03/dlm28/zuordnung.md                |  37 ------
 ue03/dmmh1710/anforderungen.md         |  24 ----
 ue03/dmmh1710/kontext.md               |  27 -----
 ue03/dmmh1710/zuordnung.md             |  37 ------
 ue03/dsch/anforderungen.md             |  16 ---
 ue03/dsch/kontext.md                   |  28 -----
 ue03/dsch/zuordnung.md                 |  38 -------
 ue03/ecib/anforderungen.md             |  19 ----
 ue03/ecib/kontext.md                   |  31 -----
 ue03/ecib/zuordnung.md                 |  37 ------
 ue03/emrano/anforderungen.md           |  19 ----
 ue03/emrano/kontext.md                 |  29 -----
 ue03/emrano/zuordnung.md               |  37 ------
 ue03/en7-mj/anforderungen.md           |  19 ----
 ue03/en7-mj/kontext.md                 |  27 -----
 ue03/en7-mj/zuordnung.md               |  37 ------
 ue03/ezen/anforderungen.md             |  20 ----
 ue03/ezen/kontext.md                   |  31 -----
 ue03/ezen/zuordnung.md                 |  38 -------
 ue03/fahm/anforderungen.md             |  18 ---
 ue03/fahm/kontext.md                   |  29 -----
 ue03/fahm/zuordnung.md                 |  37 ------
 ue03/flk/anforderungen.md              |  24 ----
 ue03/flk/kontext.md                    |  34 ------
 ue03/flk/zuordnung.md                  |  37 ------
 ue03/hfdr12/anforderungen.md           |  17 ---
 ue03/hfdr12/kontext.md                 |  39 -------
 ue03/hfdr12/zuordnung.md               |  35 ------
 ue03/iaa/anforderungen.md              |  17 ---
 ue03/iaa/kontext.md                    |  24 ----
 ue03/iaa/zuordnung.md                  |  30 -----
 ue03/ilias04j/anforderungen.md         |  18 ---
 ue03/ilias04j/kontext.md               |  30 -----
 ue03/ilias04j/zuordnung.md             |  37 ------
 ue03/janp/anforderungen.md             |  17 ---
 ue03/janp/kontext.md                   |  29 -----
 ue03/janp/zuordnung.md                 |  37 ------
 ue03/javu/anforderungen.md             |  25 ----
 ue03/javu/kontext.md                   |  30 -----
 ue03/javu/zuordnung.md                 |  37 ------
 ue03/jemy/anforderungen.md             |  27 -----
 ue03/jemy/kontext.md                   |  39 -------
 ue03/jemy/zuordnung.md                 |  37 ------
 ue03/jsug/anforderungen.md             |  21 ----
 ue03/jsug/kontext.md                   |  28 -----
 ue03/jsug/zuordnung.md                 |  37 ------
 ue03/jvng/anforderungen.md             |  23 ----
 ue03/jvng/kontext.md                   |  43 -------
 ue03/jvng/zuordnung.md                 |  37 ------
 ue03/kraz/anforderungen.md             |  19 ----
 ue03/kraz/kontext.md                   |  32 ------
 ue03/kraz/zuordnung.md                 |  41 -------
 ue03/lkrs/anforderungen.md             |  25 ----
 ue03/lkrs/kontext.md                   |  42 -------
 ue03/lkrs/zuordnung.md                 |  37 ------
 ue03/lom/anforderungen.md              |  18 ---
 ue03/lom/kontext.md                    |  37 ------
 ue03/lom/zuordnung.md                  |  37 ------
 ue03/masalabyte/anforderungen.md       |  19 ----
 ue03/masalabyte/kontext.md             |  27 -----
 ue03/masalabyte/zuordnung.md           |  37 ------
 ue03/maxbarrosschauer/anforderungen.md |  22 ----
 ue03/maxbarrosschauer/kontext.md       |  33 ------
 ue03/maxbarrosschauer/zuordnung.md     |  37 ------
 ue03/mduc/anforderungen.md             |  16 ---
 ue03/mduc/kontext.md                   |  27 -----
 ue03/mduc/zuordnung.md                 |  40 -------
 ue03/meq/anforderungen.md              |  18 ---
 ue03/meq/kontext.md                    |  32 ------
 ue03/meq/zuordnung.md                  |  37 ------
 ue03/mjab/anforderungen.md             |  16 ---
 ue03/mjab/kontext.md                   |  32 ------
 ue03/mjab/zuordnung.md                 |  38 -------
 ue03/mken/anforderungen.md             |  19 ----
 ue03/mken/kontext.md                   |  37 ------
 ue03/mken/zuordnung.md                 |   0
 ue03/mkon/anforderungen.md             |  22 ----
 ue03/mkon/kontext.md                   |  31 -----
 ue03/mkon/zuordnung.md                 |  38 -------
 ue03/moh/anforderungen.md              |  20 ----
 ue03/moh/kontext.md                    |  41 -------
 ue03/moh/zuordnung.md                  |  37 ------
 ue03/mpal/anforderungen.md             |  16 ---
 ue03/mpal/kontext.md                   |  28 -----
 ue03/mpal/zuordnung.md                 |  37 ------
 ue03/mskk15/anforderungen.md           |  13 ++-
 ue03/{agbr => mskk15}/zuordnung.md     |   6 +-
 ue03/mu/anforderungen.md               |  22 ----
 ue03/mu/kontext.md                     |  27 -----
 ue03/mu/zuordnung.md                   |  39 -------
 ue03/mw/anforderungen.md               |  19 ----
 ue03/mw/kontext.md                     |  31 -----
 ue03/mw/zuordnung.md                   |  37 ------
 ue03/my55/anforderungen.md             |  19 ----
 ue03/my55/kontext.md                   |  36 ------
 ue03/my55/zuordnung.md                 |  37 ------
 ue03/nicolino/anforderungen.md         |  18 ---
 ue03/nicolino/kontext.md               |  32 ------
 ue03/nicolino/zuordnung.md             |  37 ------
 ue03/nko/anforderungen.md              |  18 ---
 ue03/nko/kontext.md                    |  30 -----
 ue03/nko/zuordnung.md                  |  37 ------
 ue03/nly50/anforderungen.md            |  22 ----
 ue03/nly50/kontext.md                  |  38 -------
 ue03/nly50/zuordnung.md                |  39 -------
 ue03/nohl/anforderungen.md             |  16 ---
 ue03/nohl/kontext.md                   |  27 -----
 ue03/nohl/zuordnung.md                 |  38 -------
 ue03/onzj/anforderungen.md             |  17 ---
 ue03/onzj/kontext.md                   |  28 -----
 ue03/onzj/zuordnung.md                 |  36 ------
 ue03/oubou/anforderungen.md            |  16 ---
 ue03/oubou/kontext.md                  |  27 -----
 ue03/oubou/zuordnung.md                |  37 ------
 ue03/pdam/anforderungen.md             |  18 ---
 ue03/pdam/kontext.md                   |  27 -----
 ue03/pdam/zuordnung.md                 |  38 -------
 ue03/pgml/anforderungen.md             |  17 ---
 ue03/pgml/kontext.md                   |  37 ------
 ue03/pgml/zuordnung.md                 |  37 ------
 ue03/pz01/anforderungen.md             |  20 ----
 ue03/pz01/kontext.md                   |  29 -----
 ue03/pz01/zuordnung.md                 |  39 -------
 ue03/qho/anforderungen.md              |  22 ----
 ue03/qho/kontext.md                    |  33 ------
 ue03/qho/zuordnung.md                  |  36 ------
 ue03/real/anforderungen.md             |  21 ----
 ue03/real/kontext.md                   |  27 -----
 ue03/real/zuordnung.md                 |  35 ------
 ue03/sahmad/anforderungen.md           |  18 ---
 ue03/sahmad/kontext.md                 |  31 -----
 ue03/sahmad/zuordnung.md               |  37 ------
 ue03/sahmed/anforderungen.md           |  22 ----
 ue03/sahmed/kontext.md                 |  33 ------
 ue03/sahmed/zuordnung.md               |  37 ------
 ue03/sam/anforderungen.md              |  18 ---
 ue03/sam/kontext.md                    |  24 ----
 ue03/sam/zuordnung.md                  |  37 ------
 ue03/skrl78/anforderungen.md           |  18 ---
 ue03/skrl78/kontext.md                 |  25 ----
 ue03/skrl78/zuordnung.md               |  39 -------
 ue03/snab/anforderungen.md             |  19 ----
 ue03/snab/kontext.md                   |  35 ------
 ue03/snab/zuordnung.md                 |  37 ------
 ue03/sngu/anforderungen.md             |  17 ---
 ue03/sngu/kontext.md                   |  27 -----
 ue03/sngu/zuordnung.md                 |  37 ------
 ue03/sraks/anforderungen.md            |  15 ---
 ue03/sraks/kontext.md                  |  25 ----
 ue03/sraks/zuordnung.md                |  37 ------
 ue03/ssda78/anforderungen.md           |  19 ----
 ue03/ssda78/kontext.md                 |  30 -----
 ue03/ssda78/zuordnung.md               |  74 ------------
 ue03/sshj44/anforderungen.md           |  17 ---
 ue03/sshj44/kontext.md                 |  27 -----
 ue03/sshj44/zuordnung.md               |  37 ------
 ue03/stmx/anforderungen.md             |  17 ---
 ue03/stmx/kontext.md                   |  34 ------
 ue03/stmx/zuordnung.md                 |  38 -------
 ue03/talh/anforderungen.md             |  23 ----
 ue03/talh/kontext.md                   |  31 -----
 ue03/talh/zuordnung.md                 |  37 ------
 ue03/tcam/anforderungen.md             |  20 ----
 ue03/tcam/kontext.md                   |  28 -----
 ue03/tcam/zuordnung.md                 |  37 ------
 ue03/tiger/anforderungen.md            |  17 ---
 ue03/tiger/kontext.md                  |  32 ------
 ue03/tiger/zuordnung.md                |  37 ------
 ue03/tnd/anforderungen.md              |  16 ---
 ue03/tnd/kontext.md                    |  29 -----
 ue03/tnd/zuordnung.md                  |  38 -------
 ue03/trry/anforderungen.md             |  20 ----
 ue03/trry/kontext.md                   |  33 ------
 ue03/trry/zuordnung.md                 |  37 ------
 ue03/tyfncc/anforderungen.md           |  21 ----
 ue03/tyfncc/kontext.md                 |  28 -----
 ue03/tyfncc/zuordnung.md               |  39 -------
 ue03/uwar/anforderungen.md             |  19 ----
 ue03/uwar/kontext.md                   |  31 -----
 ue03/uwar/zuordnung.md                 |  40 -------
 ue03/val/anforderungen.md              |  40 -------
 ue03/val/kontext.md                    |  70 ------------
 ue03/val/zuordnung.md                  |  37 ------
 ue03/vic26/anforderungen.md            |  17 ---
 ue03/vic26/kontext.md                  |  26 -----
 ue03/vic26/zuordnung.md                |  37 ------
 ue03/virus/anforderungen.md            |  18 ---
 ue03/virus/kontext.md                  |  30 -----
 ue03/virus/zuordnung.md                |  37 ------
 ue03/wnga/anforderungen.md             |  25 ----
 ue03/wnga/kontext.md                   |  35 ------
 ue03/wnga/zuordnung.md                 |  37 ------
 ue03/ygue/anforderungen.md             |  15 ---
 ue03/ygue/kontext.md                   |  24 ----
 ue03/ygue/zuordnung.md                 |  39 -------
 ue03/ykar/anforderungen.md             |  21 ----
 ue03/ykar/kontext.md                   |  39 -------
 ue03/ykar/zuordnung.md                 |  37 ------
 ue03/z-266/anforderungen.md            |  19 ----
 ue03/z-266/kontext.md                  |  31 -----
 ue03/z-266/zuordnung.md                |  37 ------
 ue03/zc/anforderungen.md               |  30 -----
 ue03/zc/kontext.md                     |  31 -----
 ue03/zc/zuordnung.md                   |  37 ------
 ue03/zcbn/anforderungen.md             |  19 ----
 ue03/zcbn/kontext.md                   |  29 -----
 ue03/zcbn/zuordnung.md                 |  37 ------
 ue03/zcoel/anforderungen.md            |  17 ---
 ue03/zcoel/kontext.md                  |  27 -----
 ue03/zcoel/zuordnung.md                |  37 ------
 ue03/zsh/anforderungen.md              |  21 ----
 ue03/zsh/kontext.md                    |  33 ------
 ue03/zsh/zuordnung.md                  |  37 ------
 ue04/README.md                         |  40 -------
 ue04/_vorlage/einrichtung.md           |  55 ---------
 780 files changed, 32 insertions(+), 25678 deletions(-)
---
D	AGENTS.md
M	README.md
M	ue01/README.md
D	ue01/steckbriefe/AF.md
D	ue01/steckbriefe/AR.md
D	ue01/steckbriefe/Agub.md
D	ue01/steckbriefe/Anas23088.md
D	ue01/steckbriefe/Aza.md
D	ue01/steckbriefe/Bblj09.md
D	ue01/steckbriefe/Fahm.md
D	ue01/steckbriefe/HussainButt7.md
D	ue01/steckbriefe/IY69.md
D	ue01/steckbriefe/MK.md
D	ue01/steckbriefe/NN.md
D	ue01/steckbriefe/NUAli.md
D	ue01/steckbriefe/Smu.md
D	ue01/steckbriefe/TariqK2004.md
D	ue01/steckbriefe/Tiger.md
D	ue01/steckbriefe/Z-266.md
D	ue01/steckbriefe/ZahraGit12.md
M	ue01/steckbriefe/_beispiel.md
M	ue01/steckbriefe/_vorlage.md
D	ue01/steckbriefe/aalg.md
D	ue01/steckbriefe/aayd.md
D	ue01/steckbriefe/adni.md
D	ue01/steckbriefe/agbr.md
D	ue01/steckbriefe/ahyi.md
D	ue01/steckbriefe/akyf.md
D	ue01/steckbriefe/ale563.md
D	ue01/steckbriefe/anddun.md
D	ue01/steckbriefe/andel0.md
D	ue01/steckbriefe/anpa.md
D	ue01/steckbriefe/anushka.md
D	ue01/steckbriefe/asi.md
D	ue01/steckbriefe/asng24.md
D	ue01/steckbriefe/athr.md
D	ue01/steckbriefe/avon507.md
D	ue01/steckbriefe/azm96.md
D	ue01/steckbriefe/bima.md
D	ue01/steckbriefe/bunter95.md
D	ue01/steckbriefe/cms.md
D	ue01/steckbriefe/datr03.md
D	ue01/steckbriefe/davn68.md
D	ue01/steckbriefe/dhfn1611.md
D	ue01/steckbriefe/div.md
D	ue01/steckbriefe/dlm28.md
D	ue01/steckbriefe/dmal2004.md
D	ue01/steckbriefe/dmmh1710.md
D	ue01/steckbriefe/dsc.md
D	ue01/steckbriefe/dsch.md
D	ue01/steckbriefe/dszp.md
D	ue01/steckbriefe/ecib.md
D	ue01/steckbriefe/ekes.md
D	ue01/steckbriefe/emalj.md
D	ue01/steckbriefe/emrano.md
D	ue01/steckbriefe/en7-mj.md
D	ue01/steckbriefe/ezen.md
D	ue01/steckbriefe/flk.md
D	ue01/steckbriefe/fortnitepro.md
D	ue01/steckbriefe/fpz.md
D	ue01/steckbriefe/hams.md
D	ue01/steckbriefe/hfdr12.md
D	ue01/steckbriefe/hjri.md
D	ue01/steckbriefe/iaa.md
D	ue01/steckbriefe/iesp.md
D	ue01/steckbriefe/ilias04j.md
D	ue01/steckbriefe/ivlbs.md
D	ue01/steckbriefe/janp.md
D	ue01/steckbriefe/jat01.md
D	ue01/steckbriefe/javu.md
D	ue01/steckbriefe/jemy.md
D	ue01/steckbriefe/jk04.md
D	ue01/steckbriefe/jp26.md
D	ue01/steckbriefe/jsug.md
D	ue01/steckbriefe/jvng.md
D	ue01/steckbriefe/kraz.md
D	ue01/steckbriefe/lebr.md
D	ue01/steckbriefe/lkrs.md
D	ue01/steckbriefe/lom.md
D	ue01/steckbriefe/lpr2.md
D	ue01/steckbriefe/lswl60.md
D	ue01/steckbriefe/mabl.md
D	ue01/steckbriefe/masalabyte.md
D	ue01/steckbriefe/maxbarrosschauer.md
D	ue01/steckbriefe/mbgrn04.md
D	ue01/steckbriefe/mduc.md
D	ue01/steckbriefe/meq.md
D	ue01/steckbriefe/mf23.md
D	ue01/steckbriefe/mjab.md
D	ue01/steckbriefe/mjas.md
D	ue01/steckbriefe/mken.md
D	ue01/steckbriefe/mkon.md
D	ue01/steckbriefe/mks24.md
D	ue01/steckbriefe/mnag.md
D	ue01/steckbriefe/mosm.md
D	ue01/steckbriefe/mpal.md
D	ue01/steckbriefe/mskk15.md
D	ue01/steckbriefe/mu.md
D	ue01/steckbriefe/mw.md
D	ue01/steckbriefe/my55.md
D	ue01/steckbriefe/nblh.md
D	ue01/steckbriefe/ngh.md
D	ue01/steckbriefe/nicolino.md
D	ue01/steckbriefe/nko.md
D	ue01/steckbriefe/nly50.md
D	ue01/steckbriefe/nohl.md
D	ue01/steckbriefe/onzj.md
D	ue01/steckbriefe/oubou.md
D	ue01/steckbriefe/pdam.md
D	ue01/steckbriefe/peng.md
D	ue01/steckbriefe/pgml.md
D	ue01/steckbriefe/pz01.md
D	ue01/steckbriefe/qdb.md
D	ue01/steckbriefe/qho.md
D	ue01/steckbriefe/real.md
D	ue01/steckbriefe/renn.md
D	ue01/steckbriefe/sahmad.md
D	ue01/steckbriefe/sahmed.md
D	ue01/steckbriefe/sam.md
D	ue01/steckbriefe/sazy1.md
D	ue01/steckbriefe/sd99.md
D	ue01/steckbriefe/shiva.md
D	ue01/steckbriefe/skrl78.md
D	ue01/steckbriefe/skt435.md
D	ue01/steckbriefe/slr63.md
D	ue01/steckbriefe/snab.md
D	ue01/steckbriefe/sngu.md
D	ue01/steckbriefe/sshj44.md
D	ue01/steckbriefe/ssng61.md
D	ue01/steckbriefe/stmx.md
D	ue01/steckbriefe/tcam.md
D	ue01/steckbriefe/thng.md
D	ue01/steckbriefe/tnd.md
D	ue01/steckbriefe/tngan.md
D	ue01/steckbriefe/trry.md
D	ue01/steckbriefe/ttpr21.md
D	ue01/steckbriefe/tyfncc.md
D	ue01/steckbriefe/uk.md
D	ue01/steckbriefe/uwar.md
D	ue01/steckbriefe/val.md
D	ue01/steckbriefe/vic26.md
D	ue01/steckbriefe/virus.md
D	ue01/steckbriefe/vkab.md
D	ue01/steckbriefe/wnga.md
D	ue01/steckbriefe/yamekk.md
D	ue01/steckbriefe/ygue.md
D	ue01/steckbriefe/ykar.md
D	ue01/steckbriefe/yoibr42.md
D	ue01/steckbriefe/ysbi82.md
D	ue01/steckbriefe/zc.md
D	ue01/steckbriefe/zcbn.md
D	ue01/steckbriefe/zcoel.md
D	ue01/steckbriefe/zomj.md
D	ue02/Agub/notiz.md
D	ue02/Agub/phasenplan.md
D	ue02/Agub/rollen.md
D	ue02/Agub/spezifikation.md
D	ue02/IY69/notiz.md
D	ue02/IY69/phasenplan.md
D	ue02/IY69/spezifikation.md
D	ue02/Lpr/notiz.md
D	ue02/Lpr/phasenplan.md
D	ue02/Lpr/spezifikation.md
D	ue02/NN/notiz.md
D	ue02/NN/phasenplan.md
D	ue02/NN/spezifikation.md
D	ue02/NUAli/notiz.md
D	ue02/NUAli/phasenplan.md
D	ue02/NUAli/spezifikation.md
D	ue02/README.md
D	ue02/TariqK2004/notiz.md
D	ue02/TariqK2004/phasenplan.md
D	ue02/TariqK2004/spezifikation.md
D	ue02/_vorlage/notiz.md
D	ue02/_vorlage/spezifikation.md
D	ue02/_zugabe/rollen.md
D	ue02/aayd/notiz.md
D	ue02/aayd/phasenplan.md
D	ue02/aayd/spezifikation.md
D	ue02/abdu113/notiz.md
D	ue02/abdu113/phasenplan.md
D	ue02/abdu113/spezifikation.md
D	ue02/af/notiz.md
D	ue02/af/phasenplan.md
D	ue02/af/spezifikation.md
D	ue02/agbr/notiz.md
D	ue02/agbr/phasenplan.md
D	ue02/agbr/spezifikation.md
D	ue02/ahyi/notiz.md
D	ue02/ahyi/phasenplan.md
D	ue02/ahyi/spezifikation.md
D	ue02/akyf/notiz.md
D	ue02/akyf/phasenplan.md
D	ue02/akyf/spezifikation.md
D	ue02/anas23088/notiz.md
D	ue02/anas23088/phasenplan.md
D	ue02/anas23088/rollen.md
D	ue02/anas23088/spezifikation.md
D	ue02/anddun/notiz.md
D	ue02/anddun/phasenplan.md
D	ue02/anddun/spezifikation.md
D	ue02/andel0/notiz.md
D	ue02/andel0/phasenplan.md
D	ue02/andel0/spezifikation.md
D	ue02/anpa/notiz.md
D	ue02/anpa/phasenplan.md
D	ue02/anpa/rollen.md
D	ue02/anpa/spezifikation.md
D	ue02/anushka/notiz.md
D	ue02/anushka/phasenplan.md
D	ue02/anushka/rollen.md
D	ue02/anushka/spezifikation.md
D	ue02/athr/notiz.md
D	ue02/athr/phasenplan.md
D	ue02/athr/spezifikation.md
D	ue02/avon507/notiz.md
D	ue02/avon507/phasenplan.md
D	ue02/avon507/spezifikation.md
D	ue02/ayue/notiz.md
D	ue02/ayue/phasenplan.md
D	ue02/ayue/spezifikation.md
D	ue02/bblj09/notiz.md
D	ue02/bblj09/phasenplan.md
D	ue02/bblj09/spezifikation.md
D	ue02/bima/notiz.md
D	ue02/bima/phasenplan.md
D	ue02/bima/spezifikation.md
D	ue02/datr03/notiz.md
D	ue02/datr03/phasenplan.md
D	ue02/datr03/spezifikation.md
D	ue02/div/notiz.md
D	ue02/div/phasenplan.md
D	ue02/div/rollen.md
D	ue02/div/spezifikation.md
D	ue02/dlm28/notiz.md
D	ue02/dlm28/phasenplan.md
D	ue02/dlm28/spezifikation.md
D	ue02/dmmh1710/notiz.md
D	ue02/dmmh1710/phasenplan.md
D	ue02/dmmh1710/spezifikation.md
D	ue02/dsc/notiz.md
D	ue02/dsc/phasenplan.md
D	ue02/dsc/spezifikation.md
D	ue02/dsch/notiz.md
D	ue02/dsch/phasenplan.md
D	ue02/dsch/spezifikation.md
D	ue02/dszp/notiz.md
D	ue02/dszp/phasenplan.md
D	ue02/dszp/spezifikation.md
D	ue02/emrano/notiz.md
D	ue02/emrano/phasenplan.md
D	ue02/emrano/spezifikation.md
D	ue02/en7-mj/notiz.md
D	ue02/en7-mj/phasenplan.md
D	ue02/en7-mj/spezifikation.md
D	ue02/ezen/notiz.md
D	ue02/ezen/phasenplan.md
D	ue02/ezen/spezifikation.md
D	ue02/fahm/notiz.md
D	ue02/fahm/phasenplan.md
D	ue02/fahm/spezifikation.md
D	ue02/flk/notiz.md
D	ue02/flk/phasenplan.md
D	ue02/flk/spezifikation.md
D	ue02/fortnitepro/notiz.md
D	ue02/fortnitepro/phasenplan.md
D	ue02/fortnitepro/spezifikation.md
D	ue02/hams/notiz.md
D	ue02/hams/phasenplan.md
D	ue02/hams/spezifikation.md
D	ue02/hfdr12/notiz.md
D	ue02/hfdr12/phasenplan.md
D	ue02/hfdr12/spezifikation.md
D	ue02/iaa/notiz.md
D	ue02/iaa/phasenplan.md
D	ue02/iaa/spezifikation.md
D	ue02/iesp/notiz.md
D	ue02/iesp/phasenplan.md
D	ue02/iesp/spezifikation.md
D	ue02/ilias04j/notiz.md
D	ue02/ilias04j/phasenplan.md
D	ue02/ilias04j/spezifikation.md
D	ue02/ivlbs/notiz.md
D	ue02/ivlbs/phasenplan.md
D	ue02/ivlbs/spezifikation.md
D	ue02/janp/notiz.md
D	ue02/janp/phasenplan.md
D	ue02/janp/rollen.md
D	ue02/janp/spezifikation.md
D	ue02/javu11/notiz.md
D	ue02/javu11/phasenplan.md
D	ue02/javu11/rollen.md
D	ue02/javu11/spezifikation.md
D	ue02/jemy/notiz.md
D	ue02/jemy/phasenplan.md
D	ue02/jemy/rollen.md
D	ue02/jemy/spezifikation.md
D	ue02/jp26/notiz.md
D	ue02/jp26/phasenplan.md
D	ue02/jp26/spezifikation.md
D	ue02/jsug/notiz.md
D	ue02/jsug/phasenplan.md
D	ue02/jsug/spezifikation.md
D	ue02/jvng/notiz.md
D	ue02/jvng/rollen.md
D	ue02/jvng/spezifikation.md
D	ue02/kraz/notiz.md
D	ue02/kraz/phasenplan.md
D	ue02/kraz/spezifikation.md
D	ue02/lebr/notiz.md
D	ue02/lebr/phasenplan.md
D	ue02/lebr/spezifikation.md
D	ue02/lom/notiz.md
D	ue02/lom/phasenplan.md
D	ue02/lom/spezifikation.md
D	ue02/mabl/notiz.md
D	ue02/mabl/phasenplan.md
D	ue02/mabl/spezifikation.md
D	ue02/masalabyte/notiz.md
D	ue02/masalabyte/phasenplan.md
D	ue02/masalabyte/spezifikation.md
D	ue02/maxbarrosschauer/notiz.md
D	ue02/maxbarrosschauer/phasenplan.md
D	ue02/maxbarrosschauer/rollen.md
D	ue02/maxbarrosschauer/spezifikation.md
D	ue02/mbgrn04/notiz.md
D	ue02/mbgrn04/phasenplan.md
D	ue02/mbgrn04/spezifikation.md
D	ue02/mduc/notiz.md
D	ue02/mduc/phasenplan.md
D	ue02/mduc/spezifikation.md
D	ue02/meq/notiz.md
D	ue02/meq/phasenplan.md
D	ue02/meq/rollen.md
D	ue02/meq/spezifikation.md
D	ue02/mf23/notiz.md
D	ue02/mf23/phasenplan.md
D	ue02/mf23/spezifikation.md
D	ue02/mjab/notiz.md
D	ue02/mjab/phasenplan.md
D	ue02/mjab/spezifikation.md
D	ue02/mjas/notiz.md
D	ue02/mjas/phasenplan.md
D	ue02/mjas/spezifikation.md
D	ue02/mk/phasenplan.md
D	ue02/mkon/notiz.md
D	ue02/mkon/phasenplan.md
D	ue02/mkon/spezifikation.md
D	ue02/mpal/notiz.md
D	ue02/mpal/phasenplan.md
D	ue02/mpal/spezifikation.md
D	ue02/mu/notiz.md
D	ue02/mu/phasenplan.md
D	ue02/mu/spezifikation.md
D	ue02/mw/notiz.md
D	ue02/mw/phasenplan.md
D	ue02/mw/spezifikation.md
D	ue02/my55/notiz.md
D	ue02/my55/phasenplan.md
D	ue02/my55/spezifikation.md
D	ue02/ngh/notiz.md
D	ue02/ngh/phasenplan.md
D	ue02/ngh/spezifikation.md
D	ue02/nicolino/notiz.md
D	ue02/nicolino/phasenplan.md
D	ue02/nicolino/spezifikation.md
D	ue02/nko/notiz.md
D	ue02/nko/phasenplan.md
D	ue02/nko/spezifikation.md
D	ue02/nly50/notiz.md
D	ue02/nly50/phasenplan.md
D	ue02/nly50/spezifikation.md
D	ue02/nohl/notiz.md
D	ue02/nohl/phasenplan.md
D	ue02/nohl/spezifikation.md
D	ue02/oubou/notiz.md
D	ue02/oubou/phasenplan.md
D	ue02/oubou/spezifikation.md
D	ue02/pdam/notiz.md
D	ue02/pdam/phasenplan.md
D	ue02/pdam/spezifikation.md
D	ue02/pgml/notiz.md
D	ue02/pgml/phasenplan.md
D	ue02/pgml/spezifikation.md
D	ue02/pz01/notiz.md
D	ue02/pz01/phasenplan.md
D	ue02/pz01/spezifikation.md
D	ue02/qdb/notiz.md
D	ue02/qdb/phasenplan.md
D	ue02/qdb/rollen.md
D	ue02/qdb/spezifikation.md
D	ue02/qho/notiz.md
D	ue02/qho/phasenplan.md
D	ue02/qho/spezifikation.md
D	ue02/real/notiz.md
D	ue02/real/phasenplan.md
D	ue02/real/spezifikation.md
D	ue02/renn/notiz.md
D	ue02/renn/phasenplan.md
D	ue02/renn/spezifikation.md
D	ue02/sahmad/notiz.md
D	ue02/sahmad/phasenplan.md
D	ue02/sahmad/spezifikation.md
D	ue02/sahmed/notiz.md
D	ue02/sahmed/phasenplan.md
D	ue02/sahmed/rollen.md
D	ue02/sahmed/spezifikation.md
D	ue02/sam/notiz.md
D	ue02/sam/phasenplan.md
D	ue02/sam/spezifikation.md
D	ue02/skrl78/notiz.md
D	ue02/skrl78/phasenplan.md
D	ue02/skrl78/rollen.md
D	ue02/skrl78/spezifikation.md
D	ue02/skt435/notiz.md
D	ue02/skt435/spezifikation.md
D	ue02/snab/notiz.md
D	ue02/snab/phasenplan.md
D	ue02/snab/spezifikation.md
D	ue02/sngu/notiz.md
D	ue02/sngu/phasenplan.md
D	ue02/sngu/spezifikation.md
D	ue02/ssda78/notiz.md
D	ue02/ssda78/spezifikation.md
D	ue02/sshj44/notiz.md
D	ue02/sshj44/phasenplan.md
D	ue02/sshj44/spezifikation.md
D	ue02/ssng61/notiz.md
D	ue02/ssng61/spezifikation.md
D	ue02/stmx/notiz.md
D	ue02/stmx/phasenplan.md
D	ue02/stmx/spezifikation.md
D	ue02/talh/notiz.md
D	ue02/talh/phasenplan.md
D	ue02/talh/rollen.md
D	ue02/talh/spezifikation.md
D	ue02/tcam/notiz.md
D	ue02/tcam/phasenplan.md
D	ue02/tcam/spezifikation.md
D	ue02/thm-nos/notiz.md
D	ue02/thm-nos/phasenplan.md
D	ue02/thm-nos/spezifikation.md
D	ue02/thng/notiz.md
D	ue02/thng/phasenplan.md
D	ue02/thng/spezifikation.md
D	ue02/tiger/notiz.md
D	ue02/tiger/phasenplan.md
D	ue02/tiger/spezifikation.md
D	ue02/tnd/notiz.md
D	ue02/tnd/phasenplan.md
D	ue02/tnd/spezifikation.md
D	ue02/tngan/notiz.md
D	ue02/tngan/phasenplan.md
D	ue02/tngan/spezifikation.md
D	ue02/trry/notiz.md
D	ue02/trry/phasenplan.md
D	ue02/trry/rollen.md
D	ue02/trry/spezifikation.md
D	ue02/ttpr21/notiz.md
D	ue02/ttpr21/phasenplan.md
D	ue02/ttpr21/spezifikation.md
D	ue02/tyfncc/notiz.md
D	ue02/tyfncc/phasenplan.md
D	ue02/tyfncc/rollen.md
D	ue02/tyfncc/spezifikation.md
D	ue02/uwar/notiz.md
D	ue02/uwar/phasenplan.md
D	ue02/uwar/spezifikation.md
D	ue02/vic26/notiz.md
D	ue02/vic26/phasenplan.md
D	ue02/vic26/spezifikation.md
D	ue02/virus/notiz.md
D	ue02/virus/phasenplan.md
D	ue02/virus/spezifikation.md
D	ue02/wnga/notiz.md
D	ue02/wnga/phasenplan.md
D	ue02/wnga/rollen.md
D	ue02/wnga/spezifikation.md
D	ue02/ygue/notiz.md
D	ue02/ygue/phasenplan.md
D	ue02/ygue/spezifikation.md
D	ue02/ysbi82/notiz.md
D	ue02/ysbi82/spezifikation.md
D	ue02/zcbn/notiz.md
D	ue02/zcbn/phasenplan.md
D	ue02/zcbn/spezifikation.md
D	ue02/zcoel/notiz.md
D	ue02/zcoel/phasenplan.md
D	ue02/zcoel/spezifikation.md
D	ue02/zsh/notiz.md
D	ue02/zsh/phasenplan.md
D	ue02/zsh/spezifikation.md
D	ue03/IY69/anforderungen.md
D	ue03/IY69/kontext.md
D	ue03/IY69/zuordnung.md
D	ue03/Lpr/anforderungen.md
D	ue03/Lpr/kontext.md
D	ue03/Lpr/zuordnung.md
D	ue03/MK/anforderungen.md
D	ue03/MK/kontext.md
D	ue03/MK/zuordnung.md
D	ue03/NN/anforderungen.md
D	ue03/NN/kontext.md
D	ue03/NN/zuordnung.md
D	ue03/NUAli/anforderungen.md
D	ue03/NUAli/kontext.md
D	ue03/NUAli/zuordnung.md
D	ue03/README.md
D	ue03/TariqK2004/anforderungen.md
D	ue03/TariqK2004/kontext.md
D	ue03/TariqK2004/zuordnung.md
D	ue03/_vorlage/anforderungen.md
D	ue03/_vorlage/kontext.md
D	ue03/aayd/anforderungen.md
D	ue03/aayd/kontext.md
D	ue03/aayd/zuordnung.md
D	ue03/af/anforderungen.md
D	ue03/af/kontext.md
D	ue03/af/zuordnung.md
D	ue03/agbr/anforderungen.md
D	ue03/agbr/kontext.md
D	ue03/ahyi/anforderungen.md
D	ue03/ahyi/kontext.md
D	ue03/ahyi/zuordnung.md
D	ue03/akyf/anforderungen.md
D	ue03/akyf/kontext.md
D	ue03/akyf/zuordnung.md
D	ue03/anas23088/anforderungen.md
D	ue03/anas23088/kontext.md
D	ue03/anas23088/zuordnung.md
D	ue03/anddun/anforderungen.md
D	ue03/anddun/kontext.md
D	ue03/anddun/zuordnung.md
D	ue03/andel0/anforderungen.md
D	ue03/andel0/kontext.md
D	ue03/andel0/zuordnung.md
D	ue03/anpa/anforderungen.md
D	ue03/anpa/kontext.md
D	ue03/anpa/zuordnung.md
D	ue03/anushka/anforderungen.md
D	ue03/anushka/kontext.md
D	ue03/anushka/zuordnung.md
D	ue03/avon507/anforderungen.md
D	ue03/avon507/kontext.md
D	ue03/avon507/zuordnung.md
D	ue03/ayue/anforderungen.md
D	ue03/ayue/kontext.md
D	ue03/ayue/zuordnung.md
D	ue03/azm96/anforderungen.md
D	ue03/azm96/kontext.md
D	ue03/azm96/zuordnung.md
D	ue03/bblj09/anforderungen.md
D	ue03/bblj09/kontext.md
D	ue03/bblj09/zuordnung.md
D	ue03/bogh233/anforderungen.md
D	ue03/bogh233/kontext.md
D	ue03/bogh233/zuordnung.md
D	ue03/cms/anforderungen.md
D	ue03/cms/kontext.md
D	ue03/cms/zuordnung.md
D	ue03/davn68/anforderungen.md
D	ue03/davn68/kontext.md
D	ue03/davn68/zuordnung.md
D	ue03/dlm28/anforderungen.md
D	ue03/dlm28/kontext.md
D	ue03/dlm28/zuordnung.md
D	ue03/dmmh1710/anforderungen.md
D	ue03/dmmh1710/kontext.md
D	ue03/dmmh1710/zuordnung.md
D	ue03/dsch/anforderungen.md
D	ue03/dsch/kontext.md
D	ue03/dsch/zuordnung.md
D	ue03/ecib/anforderungen.md
D	ue03/ecib/kontext.md
D	ue03/ecib/zuordnung.md
D	ue03/emrano/anforderungen.md
D	ue03/emrano/kontext.md
D	ue03/emrano/zuordnung.md
D	ue03/en7-mj/anforderungen.md
D	ue03/en7-mj/kontext.md
D	ue03/en7-mj/zuordnung.md
D	ue03/ezen/anforderungen.md
D	ue03/ezen/kontext.md
D	ue03/ezen/zuordnung.md
D	ue03/fahm/anforderungen.md
D	ue03/fahm/kontext.md
D	ue03/fahm/zuordnung.md
D	ue03/flk/anforderungen.md
D	ue03/flk/kontext.md
D	ue03/flk/zuordnung.md
D	ue03/hfdr12/anforderungen.md
D	ue03/hfdr12/kontext.md
D	ue03/hfdr12/zuordnung.md
D	ue03/iaa/anforderungen.md
D	ue03/iaa/kontext.md
D	ue03/iaa/zuordnung.md
D	ue03/ilias04j/anforderungen.md
D	ue03/ilias04j/kontext.md
D	ue03/ilias04j/zuordnung.md
D	ue03/janp/anforderungen.md
D	ue03/janp/kontext.md
D	ue03/janp/zuordnung.md
D	ue03/javu/anforderungen.md
D	ue03/javu/kontext.md
D	ue03/javu/zuordnung.md
D	ue03/jemy/anforderungen.md
D	ue03/jemy/kontext.md
D	ue03/jemy/zuordnung.md
D	ue03/jsug/anforderungen.md
D	ue03/jsug/kontext.md
D	ue03/jsug/zuordnung.md
D	ue03/jvng/anforderungen.md
D	ue03/jvng/kontext.md
D	ue03/jvng/zuordnung.md
D	ue03/kraz/anforderungen.md
D	ue03/kraz/kontext.md
D	ue03/kraz/zuordnung.md
D	ue03/lkrs/anforderungen.md
D	ue03/lkrs/kontext.md
D	ue03/lkrs/zuordnung.md
D	ue03/lom/anforderungen.md
D	ue03/lom/kontext.md
D	ue03/lom/zuordnung.md
D	ue03/masalabyte/anforderungen.md
D	ue03/masalabyte/kontext.md
D	ue03/masalabyte/zuordnung.md
D	ue03/maxbarrosschauer/anforderungen.md
D	ue03/maxbarrosschauer/kontext.md
D	ue03/maxbarrosschauer/zuordnung.md
D	ue03/mduc/anforderungen.md
D	ue03/mduc/kontext.md
D	ue03/mduc/zuordnung.md
D	ue03/meq/anforderungen.md
D	ue03/meq/kontext.md
D	ue03/meq/zuordnung.md
D	ue03/mjab/anforderungen.md
D	ue03/mjab/kontext.md
D	ue03/mjab/zuordnung.md
D	ue03/mken/anforderungen.md
D	ue03/mken/kontext.md
D	ue03/mken/zuordnung.md
D	ue03/mkon/anforderungen.md
D	ue03/mkon/kontext.md
D	ue03/mkon/zuordnung.md
D	ue03/moh/anforderungen.md
D	ue03/moh/kontext.md
D	ue03/moh/zuordnung.md
D	ue03/mpal/anforderungen.md
D	ue03/mpal/kontext.md
D	ue03/mpal/zuordnung.md
M	ue03/mskk15/anforderungen.md
R098	ue03/agbr/zuordnung.md	ue03/mskk15/zuordnung.md
D	ue03/mu/anforderungen.md
D	ue03/mu/kontext.md
D	ue03/mu/zuordnung.md
D	ue03/mw/anforderungen.md
D	ue03/mw/kontext.md
D	ue03/mw/zuordnung.md
D	ue03/my55/anforderungen.md
D	ue03/my55/kontext.md
D	ue03/my55/zuordnung.md
D	ue03/nicolino/anforderungen.md
D	ue03/nicolino/kontext.md
D	ue03/nicolino/zuordnung.md
D	ue03/nko/anforderungen.md
D	ue03/nko/kontext.md
D	ue03/nko/zuordnung.md
D	ue03/nly50/anforderungen.md
D	ue03/nly50/kontext.md
D	ue03/nly50/zuordnung.md
D	ue03/nohl/anforderungen.md
D	ue03/nohl/kontext.md
D	ue03/nohl/zuordnung.md
D	ue03/onzj/anforderungen.md
D	ue03/onzj/kontext.md
D	ue03/onzj/zuordnung.md
D	ue03/oubou/anforderungen.md
D	ue03/oubou/kontext.md
D	ue03/oubou/zuordnung.md
D	ue03/pdam/anforderungen.md
D	ue03/pdam/kontext.md
D	ue03/pdam/zuordnung.md
D	ue03/pgml/anforderungen.md
D	ue03/pgml/kontext.md
D	ue03/pgml/zuordnung.md
D	ue03/pz01/anforderungen.md
D	ue03/pz01/kontext.md
D	ue03/pz01/zuordnung.md
D	ue03/qho/anforderungen.md
D	ue03/qho/kontext.md
D	ue03/qho/zuordnung.md
D	ue03/real/anforderungen.md
D	ue03/real/kontext.md
D	ue03/real/zuordnung.md
D	ue03/sahmad/anforderungen.md
D	ue03/sahmad/kontext.md
D	ue03/sahmad/zuordnung.md
D	ue03/sahmed/anforderungen.md
D	ue03/sahmed/kontext.md
D	ue03/sahmed/zuordnung.md
D	ue03/sam/anforderungen.md
D	ue03/sam/kontext.md
D	ue03/sam/zuordnung.md
D	ue03/skrl78/anforderungen.md
D	ue03/skrl78/kontext.md
D	ue03/skrl78/zuordnung.md
D	ue03/snab/anforderungen.md
D	ue03/snab/kontext.md
D	ue03/snab/zuordnung.md
D	ue03/sngu/anforderungen.md
D	ue03/sngu/kontext.md
D	ue03/sngu/zuordnung.md
D	ue03/sraks/anforderungen.md
D	ue03/sraks/kontext.md
D	ue03/sraks/zuordnung.md
D	ue03/ssda78/anforderungen.md
D	ue03/ssda78/kontext.md
D	ue03/ssda78/zuordnung.md
D	ue03/sshj44/anforderungen.md
D	ue03/sshj44/kontext.md
D	ue03/sshj44/zuordnung.md
D	ue03/stmx/anforderungen.md
D	ue03/stmx/kontext.md
D	ue03/stmx/zuordnung.md
D	ue03/talh/anforderungen.md
D	ue03/talh/kontext.md
D	ue03/talh/zuordnung.md
D	ue03/tcam/anforderungen.md
D	ue03/tcam/kontext.md
D	ue03/tcam/zuordnung.md
D	ue03/tiger/anforderungen.md
D	ue03/tiger/kontext.md
D	ue03/tiger/zuordnung.md
D	ue03/tnd/anforderungen.md
D	ue03/tnd/kontext.md
D	ue03/tnd/zuordnung.md
D	ue03/trry/anforderungen.md
D	ue03/trry/kontext.md
D	ue03/trry/zuordnung.md
D	ue03/tyfncc/anforderungen.md
D	ue03/tyfncc/kontext.md
D	ue03/tyfncc/zuordnung.md
D	ue03/uwar/anforderungen.md
D	ue03/uwar/kontext.md
D	ue03/uwar/zuordnung.md
D	ue03/val/anforderungen.md
D	ue03/val/kontext.md
D	ue03/val/zuordnung.md
D	ue03/vic26/anforderungen.md
D	ue03/vic26/kontext.md
D	ue03/vic26/zuordnung.md
D	ue03/virus/anforderungen.md
D	ue03/virus/kontext.md
D	ue03/virus/zuordnung.md
D	ue03/wnga/anforderungen.md
D	ue03/wnga/kontext.md
D	ue03/wnga/zuordnung.md
D	ue03/ygue/anforderungen.md
D	ue03/ygue/kontext.md
D	ue03/ygue/zuordnung.md
D	ue03/ykar/anforderungen.md
D	ue03/ykar/kontext.md
D	ue03/ykar/zuordnung.md
D	ue03/z-266/anforderungen.md
D	ue03/z-266/kontext.md
D	ue03/z-266/zuordnung.md
D	ue03/zc/anforderungen.md
D	ue03/zc/kontext.md
D	ue03/zc/zuordnung.md
D	ue03/zcbn/anforderungen.md
D	ue03/zcbn/kontext.md
D	ue03/zcbn/zuordnung.md
D	ue03/zcoel/anforderungen.md
D	ue03/zcoel/kontext.md
D	ue03/zcoel/zuordnung.md
D	ue03/zsh/anforderungen.md
D	ue03/zsh/kontext.md
D	ue03/zsh/zuordnung.md
D	ue04/README.md
D	ue04/_vorlage/einrichtung.md
--- merge-base
b2fa46875fb3dfeb54edda7c04dab6c499d0586b
b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
43c75e2 Abschlussart ergänzt und Semester in neuer Zeile
cc126fd Steckbrief von Lorenz ergänzt


[showing lines 213-1567 of 1567; full output saved to /Users/mariamsekkali/.local/share/opencode/shell/47c7872faf7c2f56de6aa4f37c7b7877521c2937/sh_1ac6a93b9001h5tPiVlT3rU0l3.out]

**Tool: shell**

**Input:**
```json
{
  "command": "git stash show --include-untracked --name-status stash@{0}; echo '--- tree of stash untracked'; git ls-tree -r --name-only stash@{0}^3 2>/dev/null | head -20"
}
```

A	ue02/_vorlage/notiz.md
A	ue02/_vorlage/spezifikation.md
A	ue03/README.md
A	ue03/_vorlage/anforderungen.md
A	ue03/_vorlage/kontext.md
--- tree of stash untracked
ue02/_vorlage/notiz.md
ue02/_vorlage/spezifikation.md
ue03/README.md
ue03/_vorlage/anforderungen.md
ue03/_vorlage/kontext.md


---

## Assistant

_Thinking:_

Oops, I used `git diff main..ue03-mmsk155` with two dots, which compares tips directly and shows huge deletions because branch is old. That explains. The branch is based on b2fa468, old main from Oct. So all ue02/ue03 dirs missing on branch (not deleted; just older base). Important not to misreport. The only own files on that branch are ue03/mskk15/* plus modifications. Since branch is behind main, diff shows all other merged files as deleted. Fine.

Key finding: user's branch ue03-mmsk155 is old base, with own files added/modified. Unmerged extra work: ue03/mskk15/zuordnung.md and updated anforderungen.md.

The stash adds only template files (ue02/_vorlage, ue03 README, _vorlage). That is a stash from autostash/pull that includes files from upstream? Actually stash "Sicherung vor Aufgabe 4" saved untracked files that were templates? It appears the user's local repo had older state? Not crucial. But mention: there is a stash with copies of templates/README — not own content, don't commit.

Wait, stash untracked files are additions of ue02/_vorlage/notiz.md etc. That's weird because in current main those files exist. A stash created on old base. Probably not important.

Now answer user. They asked in German. We should describe:

Repository: exercise repo for Softwaretechnik THM with four exercise folders:
- ue01: Steckbriefe (student profiles)
- ue02: project model case (notiz, phasenplan, spezifikation per person)
- ue03: requirements (anforderungen, kontext, zuordnung)
- ue04: coding agent setup (einrichtung.md, sitzung.md)
Plus README and AGENTS.md. Many student dirs; only own dirs are relevant.

Your identification: branch ue04-mskk155, GitHub username mskk155 (confirm from remote URL and commits). Files written by you (author mskk155):
1. Currently in main/working tree (committed/merged):
   - ue01/steckbriefe/mskk15.md — note filename has old abbreviation mskk15, but content "Steckbrief <mskk155>" and commit author mskk155.
   - ue03/mskk15/anforderungen.md
   - ue03/mskk15/kontext.md
   These came via PRs #78 and #305.
2. New/untracked on current branch:
   - ue04/mskk155/einrichtung.md — copy of _vorlage, still only placeholders, not yet filled; no sitzung.md.
3. On other branches, not merged:
   - ue02-mmskk155: ue02/mmskk155/{notiz,phasenplan,spezifikation}.md (old abbreviation)
   - ue03-mmsk155: ue03/mskk15/zuordnung.md and newer version of anforderungen.md (unmerged; branch is based on older main)
   - steckbrief-mskk155: ue01/steckbriefe/mskk155 (superseded/renamed to mskk15.md on main)
Note: branch ue03-mmsk155 is based on old main (b2fa468), so don't interpret missing files as deletions.

Also note stash exists containing only template/README files (ue02/_vorlage, ue03/README, ue03/_vorlage) — not your content; don't include.

Potential ambiguity: Are ue02/mmskk155 and ue03/mskk15 really theirs? Evidence: all commits author mskk155 same email; branch names; directory names close. AGENTS says if unclear ask. But evidence is strong (commit author). We can state "nach Prüfung der Commit-Autoren" and mention older abbreviations. No need to ask unless user wants certainty. But maybe question tool? The instruction says ask if unclear. It's clear enough from commit author email matching remote mskk155. We can note the assumption.

Also mention there is no ue02 directory for mskk155 on main, because that work is only on branch. Wait—did PR for ue02 get merged? Maybe under mmskk155? Not in current tree. So not merged.

Need be concise. Use Markdown. No changes made. Also note current branch is not main, so AGENTS rule satisfied; nothing changed anyway.

Let's craft German answer. Include counts maybe "über 1.000 Dateien" not needed. We can say "sehr viele Studierendenverzeichnisse".

Also important: ue01/steckbriefe/mskk15.md content has placeholders "…" leftover; ue03 has "Sekreteriat" typo etc. Not asked to review. Maybe don't critique.

Let's give table of own files with status.

Also mention "sitzung.md fehlt noch" for ue04. And that einrichtung.md is still template. That's directly relevant.

Should I mention the stash? Yes, brief note under "Sonstiges".

Let's make final answer in German with file paths.

Ich habe die Verzeichnisse und die Commit-Autoren geprüft. Du arbeitest auf dem Branch `ue04-mskk155`; dein GitHub-Benutzername ist laut Remote-URL und Commits **`mskk155`**.

## Was im Repository liegt

Es ist das Übungsrepository der THM für Softwaretechnik. Es enthält vier Übungsverzeichnisse mit den Abgaben vieler Studierender:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | Steckbriefe pro Person (`steckbriefe/<name>.md`) |
| `ue02/` | Projektmodell am Fall, pro Person `notiz.md`, `phasenplan.md`, `spezifikation.md` |
| `ue03/` | Anforderungen, pro Person `anforderungen.md`, `kontext.md`, `zuordnung.md` |
| `ue04/` | Coding Agent, pro Person `einrichtung.md` und `sitzung.md` |

Dazu kommen die Regeln in `README.md` und `AGENTS.md` sowie die Vorlagen in den `_vorlage`-Verzeichnissen.

## Dateien, die von dir stammen

Nach Prüfung der Commit-Autoren (`mskk155 <…@mnd.thm.de>`) gehören dir diese Dateien:

**Bereits in `main` enthalten (über Pull Requests zusammengeführt):**

- `ue01/steckbriefe/mskk15.md` – dein Steckbrief. Der Dateiname trägt noch das ältere Kürzel `mskk15`, im Inhalt steht aber `# Steckbrief <mskk155>`.
- `ue03/mskk15/anforderungen.md`
- `ue03/mskk15/kontext.md`

**Neu und noch nicht committet (auf deinem aktuellen Branch):**

- `ue04/mskk155/einrichtung.md` – eine Kopie der Vorlage. Sie enthält noch die Platzhalter „…“; ausgefüllt ist sie noch nicht. `ue04/mskk155/sitzung.md` fehlt bisher.

**Auf anderen, nicht zusammengeführten Branches:**

- Branch `ue02-mmskk155`: `ue02/mmskk155/notiz.md`, `phasenplan.md`, `spezifikation.md` (ältere Schreibweise mit zwei „m“) – diese Übung ist nicht in `main`.
- Branch `ue03-mmsk155`: `ue03/mskk15/zuordnung.md` und eine neuere Fassung von `anforderungen.md` – ebenfalls noch nicht in `main`. Achtung: Der Branch basiert auf einem älteren `main`-Stand (`b2fa468`), daher wirkt ein Vergleich mit dem heutigen `main` so, als fehlten viele fremde Dateien. Das ist nur der alte Stand, keine Löschung.
- Branch `steckbrief-mskk155`: `ue01/steckbriefe/mskk155` – offenbar die frühere Fassung, die in `main` als `mskk15.md` gelandet ist.

**Sonstiges:** Es gibt einen Stash `Sicherung vor Aufgabe 4`. Darin liegen nur Kopien von Vorlagen (`ue02/_vorlage/…`, `ue03/README.md`, `ue03/_vorlage/…`), also keine eigenen Inhalte. Den solltest du nicht mit einreichen.

Kurz gesagt: Deine bisher eingereichten Inhalte sind der Steckbrief und die Übung-3-Dateien unter `ue03/mskk15/`; an Übung 4 hast du bisher nur die unveränderte Vorlage als `ue04/mskk155/einrichtung.md` kopiert. Geändert habe ich nichts.

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

The user repeats the same question. Maybe they want re-check because date changed / files may have changed. We should re-run inspection to see if anything changed since yesterday. The working tree may now have sitzung.md or filled einrichtung.md. Let's check status and files.

Ich prüfe den aktuellen Stand erneut.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current; echo '--- status'; git status --short -uall; echo '--- log'; git log --oneline -3"
}
```

ue04-mskk155
--- status
?? ue04/mskk155/einrichtung.md
--- log
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)


**Tool: shell**

**Input:**
```json
{
  "command": "find ue04/mskk155 -type f -maxdepth 1 -print -exec sh -c 'echo \"--- $1\"; cat \"$1\"' _ {} \\; 2>/dev/null"
}
```

ue04/mskk155/einrichtung.md
--- ue04/mskk155/einrichtung.md
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


**Tool: shell**

**Input:**
```json
{
  "command": "git log --all --author='mskk155' --name-only --format='%h %ad %s' --date=short | sed '/^$/d'; echo '--- stash'; git stash list"
}
```

3f97a10 2026-11-05 On ue04-mskk155: Sicherung vor Aufgabe 4
427c486 2026-11-05 index on ue04-mskk155: b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
56af870 2026-11-05 untracked files on ue04-mskk155: b2fa468 Merge pull request #13 from LorenzPrz/steckbrief-Lpr
ue02/_vorlage/notiz.md
ue02/_vorlage/spezifikation.md
ue03/README.md
ue03/_vorlage/anforderungen.md
ue03/_vorlage/kontext.md
ee5720f 2026-11-05 Anforderungen vervollständigt
ue03/mskk15/anforderungen.md
3004f71 2026-11-05 Eigene Anforderungen ergänzt
ue03/mskk15/anforderungen.md
d46266f 2026-11-05 Zuordnung Anforderungen oder Lösung
ue03/mskk15/zuordnung.md
47056ae 2026-11-02 Aufgaben 1 und 3 bearbeiten (#305)
ue03/mskk15/anforderungen.md
ue03/mskk15/kontext.md
57d79b1 2026-10-27 Aufgaben 1 und 3 bearbeiten
ue03/mmsk155/anforderungen.md
ue03/mmsk155/kontext.md
ue03/mmsk155/spezifikation.md
ac3346a 2026-10-26 Bearbeite Uebung 02
ue02/mmskk155/notiz.md
ue02/mmskk155/phasenplan.md
ue02/mmskk155/spezifikation.md
85b6c9c 2026-10-20 Steckbrief erstellen (#78)
ue01/steckbriefe/mskk15.md
d00319f 2026-10-19 Steckbrief erstellen
ue01/steckbriefe/mskk155
--- stash
stash@{0}: On ue04-mskk155: Sicherung vor Aufgabe 4


---

## Assistant

_Thinking:_

Nothing changed. Should answer again, perhaps concise, maybe note it's unchanged since yesterday. The user may have wanted the same answer; perhaps they expected a fresh check. We can say "Der Stand ist unverändert." and provide the same summary, maybe more compact. Also maybe they ask because another agent? We should provide full answer to be useful.

We could verify own files and branch state again, but already have data. Branch ue03-mmsk155 still exists. Let's quickly confirm no branch changes since yesterday? The log shows same. Fine.

Answer in German. Don't include personal email. Mention user identity mskk155. Keep same content, maybe slightly refined.

Important: "welche Dateien stammen von mir?" We can group.

Let's answer compactly but completely.

Der Stand ist unverändert gegenüber meiner letzten Prüfung.

## Repository-Inhalt

Das Repository gehört zur Softwaretechnik-Übung der THM. Es enthält die Abgaben vieler Studierender in vier Übungsverzeichnissen:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | Steckbriefe (`ue01/steckbriefe/<name>.md`) |
| `ue02/` | Projektmodell am Fall: `notiz.md`, `phasenplan.md`, `spezifikation.md` |
| `ue03/` | Anforderungen: `anforderungen.md`, `kontext.md`, `zuordnung.md` |
| `ue04/` | Coding Agent: `einrichtung.md` und `sitzung.md` |

Dazu kommen `README.md`, `AGENTS.md` und die Vorlagen in den `_vorlage`-Verzeichnissen. Dein Branch ist `ue04-mskk155`, dein Benutzername **`mskk155`**.

## Deine Dateien

**Bereits in `main` (über Pull Requests zusammengeführt):**

- `ue01/steckbriefe/mskk15.md` – dein Steckbrief; der Dateiname trägt noch das ältere Kürzel `mskk15`, der Inhalt lautet `# Steckbrief <mskk155>`.
- `ue03/mskk15/anforderungen.md`
- `ue03/mskk15/kontext.md`

**Auf dem aktuellen Branch, aber noch nicht committet:**

- `ue04/mskk155/einrichtung.md` – unveränderte Kopie der Vorlage, alle Angaben sind noch „…“. Eine `sitzung.md` fehlt bisher.

**Auf anderen Branches, nicht in `main`:**

- `ue02-mmskk155`: `ue02/mmskk155/notiz.md`, `phasenplan.md`, `spezifikation.md` (ältere Schreibweise mit zwei „m“).
- `ue03-mmsk155`: `ue03/mskk15/zuordnung.md` und eine neuere Fassung von `anforderungen.md`. Der Branch beruht auf einem älteren `main`-Stand; fehlende fremde Dateien im Vergleich sind daher kein Löschen.
- `steckbrief-mskk155`: `ue01/steckbriefe/mskk155` – die frühere Fassung, die in `main` als `mskk15.md` liegt.

**Hinweis:** Der Stash `Sicherung vor Aufgabe 4` enthält nur Kopien von Vorlagen und `README`-Dateien, keine eigenen Inhalte. Er gehört nicht in die Abgabe.

Geändert habe ich nichts.
