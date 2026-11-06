# Repository-Dateien und eigene Beiträge

**Session ID:** ses_e4d4e5d84ffes9otSob9mQS0wc
**Created:** 11/6/2026, 10:09:08 PM
**Updated:** 11/6/2026, 10:09:45 PM

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

ue04-pokerbuddie


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
.git\
ue01\
ue02\
ue03\
ue04\
AGENTS.md
README.md

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

**Tool: shell**

**Input:**
```json
{
  "command": "git status --short"
}
```

?? ue04/pokerbuddie/


**Tool: glob**

**Input:**
```json
{
  "pattern": "**/AGENTS.md"
}
```

C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\AGENTS.md

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

C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage\einrichtung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue04\README.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue04\pokerbuddie\einrichtung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\README.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\_zugabe\rollen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\_vorlage.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\_beispiel.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zomj.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zcoel.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zcbn.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zc.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ZahraGit12.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Z-266.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ysbi82.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\yoibr42.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ykar.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ygue.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\yamekk.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\wnga.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\vkab.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\virus.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\vic26.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\val.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\uwar.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\uk.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tyfncc.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ttpr21.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\trry.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tngan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tnd.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Tiger.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\thng.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tcam.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\TariqK2004.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\stmx.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ssng61.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sshj44.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sngu.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\snab.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Smu.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\slr63.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\skt435.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\skrl78.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\shiva.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sd99.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sazy1.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sam.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sahmed.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sahmad.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\renn.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\real.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\qho.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\qdb.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\pz01.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\pgml.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\peng.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\pdam.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\oubou.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\onzj.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\NUAli.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nohl.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\NN.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nly50.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nko.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nicolino.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ngh.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nblh.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\my55.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mw.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mu.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mskk15.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mpal.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mosm.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mnag.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mks24.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mkon.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mken.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\MK.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mjas.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mjab.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mf23.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\meq.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mduc.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mbgrn04.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\maxbarrosschauer.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\masalabyte.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mabl.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lswl60.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lpr2.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Lpr.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lom.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lkrs.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lebr.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\kraz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jvng.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jsug.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jp26.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jk04.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jemy.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\javu.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jat01.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\janp.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\IY69.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ivlbs.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ilias04j.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\iesp.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\iaa.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\HussainButt7.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\hjri.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\hfdr12.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\hams.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\fpz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\fortnitepro.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\flk.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Fahm.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ezen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\en7-mj.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\emrano.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\emalj.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ekes.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ecib.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dszp.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dsch.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dsc.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dmmh1710.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dmal2004.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dlm28.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\div.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dhfn1611.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\davn68.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\datr03.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\cms.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\bunter95.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\bima.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Bblj09.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\azm96.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Aza.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\avon507.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\athr.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\asng24.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\asi.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\AR.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\anushka.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\anpa.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\andel0.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\anddun.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Anas23088.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ale563.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\akyf.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ahyi.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Agub.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\agbr.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\AF.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\adni.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\aayd.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\aalg.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mk\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\zuordnung.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\kontext.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\anforderungen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\div\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\div\rollen.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\div\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\div\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\akyf\spezifikation.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\akyf\phasenplan.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\akyf\notiz.md
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\zuordnung.md

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
  "pattern": "pokerbuddie",
  "caseSensitive": false,
  "limit": 40
}
```

Found 1 matches
C:\Users\pokerbuddie\OneDrive\Desktop\Schule\thm_wk-1208_softwaretechnik-uebungen\ue02\pz01\spezifikation.md:
  Line 4: Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @PokerBuddie


**Tool: glob**

**Input:**
```json
{
  "pattern": "**/*poker*",
  "limit": 50
}
```

No files found

**Tool: read**

**Input:**
```json
{
  "path": "ue04/pokerbuddie",
  "limit": 30
}
```

Read directory ue04/pokerbuddie, entries 1-1
einrichtung.md

---

## Assistant

_Thinking:_



**Tool: read**

**Input:**
```json
{
  "path": "ue02/pz01"
}
```

Read directory ue02/pz01, entries 1-3
notiz.md
phasenplan.md
spezifikation.md

**Tool: read**

**Input:**
```json
{
  "path": "ue03/pz01"
}
```

Read directory ue03/pz01, entries 1-3
anforderungen.md
kontext.md
zuordnung.md

**Tool: read**

**Input:**
```json
{
  "path": "ue01/steckbriefe/pz01.md"
}
```

Read file ue01/steckbriefe/pz01.md, lines 1-13
1: # Steckbrief pz01
2: 
3: ## Studiengang und Semester
4: 
5: Ich studiere Wirtschaftsinformatik an der THM in Friedberg und befinde mich im 3. Semester.
6: 
7: ## Meine bisherige Erfahrung mit Softwareentwicklung
8: 
9: Ich habe bisher erste Grundlagen der Programmierung im Studium kennengelernt. Meine praktischen Erfahrungen mit Softwareentwicklung sind noch begrenzt, aber ich möchte meine Kenntnisse weiter ausbauen.
10: 
11: ## Das erwarte ich von der Veranstaltung
12: 
13: Ich erwarte von der Veranstaltung, dass ich die Grundlagen der Softwareentwicklung besser verstehe und lerne, wie Softwareprojekte geplant und umgesetzt werden. Besonders möchte ich praktische Erfahrungen sammeln und den Umgang mit Git und GitHub verbessern.

**Tool: read**

**Input:**
```json
{
  "path": "ue02/pz01/spezifikation.md",
  "limit": 15
}
```

Read file ue02/pz01/spezifikation.md, lines 1-15
1: 
2: # Spezifikation des Terminplaners – Gliederung und Beispiele
3: 
4: Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @PokerBuddie
5: 
6: ## 1. Ziel und Zweck
7: 
8: ### Beispiel
9: Der Terminplaner soll Studierenden ermöglichen, Sprechstunden und Prüfungstermine online zu buchen, ohne dafür E-Mails schreiben zu müssen.
10: 
11: ## 2. Benutzergruppen und Rollen
12: 
13: ### Beispiel
14: Studierende können freie Termine buchen und absagen. Lehrende können ihre verfügbaren Sprechstunden verwalten. Sekretariate erhalten eine Übersicht über die Termine.
15: 
[Output truncated. Continue reading with offset: 16]

---

## Assistant

## Was liegt im Repository?

Das Repository enthält Abgaben zu den **Softwaretechnik-Übungen der THM**:

| Ordner | Inhalt |
|---|---|
| `ue01/` | Git und GitHub: Steckbriefe |
| `ue02/` | Projektmodell: Gesprächsnotiz, Phasenplan und Spezifikation |
| `ue03/` | Anforderungen an einen Terminplaner |
| `ue04/` | Einrichtung eines Coding Agents und Sitzungsdokumentation |

Dazu kommen Aufgabenbeschreibungen (`README.md`), Vorlagen (`_vorlage/`), Zusatzmaterial (`_zugabe/`) und Agentenregeln (`AGENTS.md`).

## Welche Dateien sind deine?

Dein aktueller Branch heißt **`ue04-pokerbuddie`**. Dazu passt:

- `ue04/pokerbuddie/einrichtung.md` — vorhanden, aber noch **nicht von Git erfasst**.

Außerdem nennt `ue02/pz01/spezifikation.md` ausdrücklich **`@PokerBuddie`** als Mitwirkenden. Das deutet auf dein früheres Kürzel **`pz01`** hin. Unter diesem Kürzel liegen:

- `ue01/steckbriefe/pz01.md`
- `ue02/pz01/notiz.md`
- `ue02/pz01/phasenplan.md`
- `ue02/pz01/spezifikation.md`
- `ue03/pz01/anforderungen.md`
- `ue03/pz01/kontext.md`
- `ue03/pz01/zuordnung.md`

**War `pz01` dein früheres Kürzel?** Dann lassen sich auch diese Dateien dir zuordnen.

Für Übung 4 fehlt aktuell noch `ue04/pokerbuddie/sitzung.md`. Ich habe nichts verändert.
