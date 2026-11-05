# Repository-Inhalte und eigene Dateien

**Session ID:** ses_e52a5ecb9ffefvIm9rHJeBsZhx
**Created:** 11/5/2026, 9:15:24 PM
**Updated:** 11/5/2026, 9:15:58 PM

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

**Tool: read**

**Input:**
```json
{
  "path": ".",
  "limit": 100
}
```

Read directory ., entries 1-7
.git/
ue01/
ue02/
ue03/
ue04/
AGENTS.md
README.md

**Tool: read**

**Input:**
```json
{
  "path": "README.md",
  "limit": 250
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

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current"
}
```

ue04-zehracoban990-bit


**Tool: shell**

**Input:**
```json
{
  "command": "git status --short"
}
```

?? ue04/zehracoban990-bit/


**Tool: glob**

**Input:**
```json
{
  "pattern": "**/AGENTS.md",
  "limit": 100
}
```

/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/AGENTS.md

---

## Assistant

**Tool: glob**

**Input:**
```json
{
  "pattern": "ue*/**/*",
  "limit": 250
}
```

/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dlm28/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dlm28/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dlm28/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dsc/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dsc/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dsc/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/meq/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/meq/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/meq/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/meq/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/virus/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/virus/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/virus/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/vic26/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/vic26/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/vic26/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dmmh1710/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dmmh1710/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dmmh1710/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tnd/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tnd/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tnd/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/akyf/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/akyf/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/akyf/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ttpr21/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ttpr21/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ttpr21/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/my55/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/my55/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/my55/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcoel/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcoel/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcoel/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anushka/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anushka/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anushka/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anushka/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ygue/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ygue/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ygue/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/qho/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/qho/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/qho/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ysbi82/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ysbi82/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/pgml/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/pgml/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/pgml/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tcam/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/maxbarrosschauer/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/maxbarrosschauer/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/maxbarrosschauer/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tcam/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/maxbarrosschauer/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tcam/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mbgrn04/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mbgrn04/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mbgrn04/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmad/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmad/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmad/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/agbr/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/agbr/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/agbr/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mjas/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mjas/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mjas/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/skt435/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/skt435/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ssda78/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/_vorlage/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Agub/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Agub/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Agub/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Agub/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ssda78/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/_vorlage/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/thm-nos/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/thm-nos/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/thm-nos/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/README.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/renn/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/renn/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/renn/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/skrl78/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/skrl78/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/skrl78/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/skrl78/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/aayd/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/aayd/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/aayd/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/kraz/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/kraz/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/kraz/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/trry/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/trry/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/trry/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Lpr/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/trry/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Lpr/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/Lpr/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/_zugabe/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/IY69/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/IY69/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/IY69/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nly50/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nly50/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nly50/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/andel0/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/andel0/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/andel0/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/uwar/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dszp/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dszp/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/uwar/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/dszp/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/uwar/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/snab/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/snab/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/snab/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/NUAli/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/NUAli/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/NUAli/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/hfdr12/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/hfdr12/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/hfdr12/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/jp26/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue04/zehracoban990-bit/einrichtung.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/jp26/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/jp26/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tiger/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tiger/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tiger/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue04/README.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/lebr/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/iaa/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/lebr/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/iaa/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/lebr/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/iaa/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sngu/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sngu/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sngu/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/janp/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/janp/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/janp/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/janp/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/talh/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/talh/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/talh/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/talh/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nicolino/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nicolino/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nicolino/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue04/_vorlage/einrichtung.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/bblj09/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mabl/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/bblj09/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mabl/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/bblj09/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/masalabyte/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mabl/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/masalabyte/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/masalabyte/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/abdu113/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/abdu113/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/abdu113/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mw/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mw/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mw/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/jvng/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/athr/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/jvng/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/jvng/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/athr/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/athr/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anddun/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anddun/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anddun/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anpa/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anpa/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anpa/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anpa/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/fortnitepro/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/fortnitepro/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/fortnitepro/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ayue/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ayue/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ayue/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nko/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zsh/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/af/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmed/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmed/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmed/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/sahmed/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nko/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nko/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/af/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/af/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zsh/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zsh/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mjab/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mjab/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mjab/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mu/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mu/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mu/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anas23088/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anas23088/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anas23088/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/anas23088/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/avon507/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/fahm/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tyfncc/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tyfncc/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tyfncc/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/tyfncc/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/avon507/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/avon507/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/bima/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/wnga/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/wnga/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/wnga/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/wnga/rollen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/bima/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/bima/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/fahm/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/fahm/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/mk/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/stmx/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/stmx/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/stmx/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/oubou/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/oubou/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/oubou/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/flk/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/flk/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/flk/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue03/dlm28/anforderungen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue03/dlm28/kontext.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue03/dlm28/zuordnung.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/datr03/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/datr03/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/datr03/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ilias04j/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ilias04j/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/ilias04j/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/nohl/phasenplan.md

(Results are truncated: showing first 250 results. Consider using a more specific path or pattern.)

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

**Tool: grep**

**Input:**
```json
{
  "pattern": "zehracoban990-bit",
  "limit": 60
}
```

Found 1 matches
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcbn/spezifikation.md:
  Line 3: Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @zehracoban990-bit


**Tool: glob**

**Input:**
```json
{
  "pattern": "**/*zehracoban*",
  "limit": 30
}
```

No files found

**Tool: read**

**Input:**
```json
{
  "path": "ue04/zehracoban990-bit/",
  "limit": 30
}
```

Read directory ue04/zehracoban990-bit/, entries 1-1
einrichtung.md

**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files --others --exclude-standard ue04/zehracoban990-bit/"
}
```

ue04/zehracoban990-bit/einrichtung.md


---

## Assistant

**Tool: glob**

**Input:**
```json
{
  "pattern": "ue*/zcbn/*",
  "limit": 30
}
```

/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcbn/phasenplan.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcbn/notiz.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue02/zcbn/spezifikation.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue03/zcbn/anforderungen.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue03/zcbn/kontext.md
/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue03/zcbn/zuordnung.md

**Tool: glob**

**Input:**
```json
{
  "pattern": "ue01/**/*zcbn*",
  "limit": 20
}
```

/Users/zehra/Desktop/thm_wk-1208_softwaretechnik-uebungen/ue01/steckbriefe/zcbn.md

**Tool: read**

**Input:**
```json
{
  "path": "ue02/zcbn/spezifikation.md",
  "limit": 25
}
```

Read file ue02/zcbn/spezifikation.md, lines 1-24
1: # Spezifikation des Terminplaners — Gliederung und Beispiele
2: 
3: Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @zehracoban990-bit
4: 
5: 
6: 
7: ## Ziel und Zielgruppe
8: 
9: Der Terminplaner soll Studierenden ermöglichen, Termine online zu buchen, zu verwalten und zu stornieren.
10: Lehrende können ihre verfügbaren Termine anbieten.
11: 
12: ## Kernfunktionen
13: 
14: Nutzer können einen freien Zeitraum auswählen, einen Termin buchen und eine Bestätigung erhalten.
15: Bereits gebuchte Termine können geändert oder storniert werden.
16: 
17: ## Regeln und Einschränkungen
18: 
19: Doppelbuchungen sollen verhindert werden.
20: Eine Stornierung ist beispielsweise nur bis 24 Stunden vor Terminbeginn möglich.
21: 
22: ## Datenverwaltung
23: 
24: Für jeden Termin werden Informationen wie Termin-ID, Titel, Startzeit, Endzeit und zugehöriger Nutzer gespeichert.

---

## Assistant

## Was liegt im Repository?

Das Repository enthält Abgaben zu den **Softwaretechnik-Übungen der THM**:

| Ordner | Inhalt |
|---|---|
| `ue01/` | Git/GitHub kennenlernen, persönliche Steckbriefe |
| `ue02/` | Projektmodell: Gesprächsnotiz, Phasenplan und Spezifikation |
| `ue03/` | Stakeholder, Systemkontext und Anforderungen an einen Terminplaner |
| `ue04/` | Coding Agent einrichten und Sitzung dokumentieren |

Dazu kommen Aufgabenbeschreibungen (`README.md`), Vorlagen und Abgaben anderer Studierender. `AGENTS.md` enthält Regeln für KI-Agenten.

## Welche Dateien sind deine?

Dein aktueller Branch heißt `ue04-zehracoban990-bit`. In `ue02/zcbn/spezifikation.md` steht außerdem ausdrücklich `@zehracoban990-bit`. Damit lässt sich das ältere Kürzel **`zcbn`** deinem Benutzernamen zuordnen:

- `ue01/steckbriefe/zcbn.md`
- `ue02/zcbn/notiz.md`
- `ue02/zcbn/phasenplan.md`
- `ue02/zcbn/spezifikation.md`
- `ue03/zcbn/anforderungen.md`
- `ue03/zcbn/kontext.md`
- `ue03/zcbn/zuordnung.md`
- `ue04/zehracoban990-bit/einrichtung.md`

Die letzte Datei ist **noch nicht in Git aufgenommen**. Die für Übung 4 vorgesehene `sitzung.md` liegt noch nicht vor.

Ich habe nichts verändert.
