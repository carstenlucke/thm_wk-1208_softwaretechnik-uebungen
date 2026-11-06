# Repository-Dateien und eigene Beiträge

**Session ID:** ses_e4fe13cdeffeL8VXgV14PP8DuW
**Created:** 11/6/2026, 10:09:28 AM
**Updated:** 11/6/2026, 10:09:42 AM

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

ue04-shalinkoirala


---

## Assistant

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
  "command": "git status --short && git branch --show-current && find . -maxdepth 2 -type d -not -path './.git*' | sort",
  "workdir": "."
}
```

?? ue04/shalinkoirala/
ue04-shalinkoirala
.
./ue01
./ue01/steckbriefe
./ue02
./ue02/_vorlage
./ue02/_zugabe
./ue02/aayd
./ue02/abdu113
./ue02/af
./ue02/agbr
./ue02/Agub
./ue02/ahyi
./ue02/akyf
./ue02/anas23088
./ue02/anddun
./ue02/andel0
./ue02/anpa
./ue02/anushka
./ue02/athr
./ue02/avon507
./ue02/ayue
./ue02/bblj09
./ue02/bima
./ue02/datr03
./ue02/div
./ue02/dlm28
./ue02/dmmh1710
./ue02/dsc
./ue02/dsch
./ue02/dszp
./ue02/emrano
./ue02/en7-mj
./ue02/ezen
./ue02/fahm
./ue02/flk
./ue02/fortnitepro
./ue02/hams
./ue02/hfdr12
./ue02/iaa
./ue02/iesp
./ue02/ilias04j
./ue02/ivlbs
./ue02/IY69
./ue02/janp
./ue02/javu11
./ue02/jemy
./ue02/jp26
./ue02/jsug
./ue02/jvng
./ue02/kraz
./ue02/lebr
./ue02/lom
./ue02/Lpr
./ue02/mabl
./ue02/masalabyte
./ue02/maxbarrosschauer
./ue02/mbgrn04
./ue02/mduc
./ue02/meq
./ue02/mf23
./ue02/mjab
./ue02/mjas
./ue02/mk
./ue02/mkon
./ue02/mpal
./ue02/mu
./ue02/mw
./ue02/my55
./ue02/ngh
./ue02/nicolino
./ue02/nko
./ue02/nly50
./ue02/NN
./ue02/nohl
./ue02/NUAli
./ue02/oubou
./ue02/pdam
./ue02/pgml
./ue02/pz01
./ue02/qdb
./ue02/qho
./ue02/real
./ue02/renn
./ue02/sahmad
./ue02/sahmed
./ue02/sam
./ue02/skrl78
./ue02/skt435
./ue02/snab
./ue02/sngu
./ue02/ssda78
./ue02/sshj44
./ue02/ssng61
./ue02/stmx
./ue02/talh
./ue02/TariqK2004
./ue02/tcam
./ue02/thm-nos
./ue02/thng
./ue02/tiger
./ue02/tnd
./ue02/tngan
./ue02/trry
./ue02/ttpr21
./ue02/tyfncc
./ue02/uwar
./ue02/vic26
./ue02/virus
./ue02/wnga
./ue02/ygue
./ue02/ysbi82
./ue02/zcbn
./ue02/zcoel
./ue02/zsh
./ue03
./ue03/_vorlage
./ue03/aayd
./ue03/af
./ue03/agbr
./ue03/ahyi
./ue03/akyf
./ue03/anas23088
./ue03/anddun
./ue03/andel0
./ue03/anpa
./ue03/anushka
./ue03/avon507
./ue03/ayue
./ue03/azm96
./ue03/bblj09
./ue03/bogh233
./ue03/cms
./ue03/davn68
./ue03/dlm28
./ue03/dmmh1710
./ue03/dsch
./ue03/ecib
./ue03/emrano
./ue03/en7-mj
./ue03/ezen
./ue03/fahm
./ue03/flk
./ue03/hfdr12
./ue03/iaa
./ue03/ilias04j
./ue03/IY69
./ue03/janp
./ue03/javu
./ue03/jemy
./ue03/jsug
./ue03/jvng
./ue03/kraz
./ue03/lkrs
./ue03/lom
./ue03/Lpr
./ue03/masalabyte
./ue03/maxbarrosschauer
./ue03/mduc
./ue03/meq
./ue03/mjab
./ue03/MK
./ue03/mken
./ue03/mkon
./ue03/moh
./ue03/mpal
./ue03/mskk15
./ue03/mu
./ue03/mw
./ue03/my55
./ue03/nicolino
./ue03/nko
./ue03/nly50
./ue03/NN
./ue03/nohl
./ue03/NUAli
./ue03/onzj
./ue03/oubou
./ue03/pdam
./ue03/pgml
./ue03/pz01
./ue03/qho
./ue03/real
./ue03/sahmad
./ue03/sahmed
./ue03/sam
./ue03/skrl78
./ue03/snab
./ue03/sngu
./ue03/sraks
./ue03/ssda78
./ue03/sshj44
./ue03/stmx
./ue03/talh
./ue03/TariqK2004
./ue03/tcam
./ue03/tiger
./ue03/tnd
./ue03/trry
./ue03/tyfncc
./ue03/uwar
./ue03/val
./ue03/vic26
./ue03/virus
./ue03/wnga
./ue03/ygue
./ue03/ykar
./ue03/z-266
./ue03/zc
./ue03/zcbn
./ue03/zcoel
./ue03/zsh
./ue04
./ue04/_vorlage
./ue04/shalinkoirala


**Tool: shell**

**Input:**
```json
{
  "command": "find ue04 -maxdepth 2 -type f | sort",
  "workdir": "."
}
```

ue04/_vorlage/einrichtung.md
ue04/README.md
ue04/shalinkoirala/einrichtung.md


---

## Assistant

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

Das Repository enthält die Übungen der Veranstaltung Softwaretechnik. Laut Haupt-README gibt es vier Bereiche:

- `ue01/` – Erste Schritte mit Git und GitHub
- `ue02/` – Projektmodell am Fall
- `ue03/` – Anforderungen an den Terminplaner
- `ue04/` – Coding Agent einrichten

Dein Benutzername ist `shalinkoirala` (aus dem Branch `ue04-shalinkoirala`). Dein persönliches Verzeichnis ist **`ue04/shalinkoirala/`**. Darin liegt derzeit:

- `ue04/shalinkoirala/einrichtung.md`

Die Übungsanleitung sieht außerdem eine `sitzung.md` vor; die ist in deinem Verzeichnis aktuell nicht vorhanden. Momentan ist auch `ue04/shalinkoirala/` als nicht versionierte Änderung markiert.
