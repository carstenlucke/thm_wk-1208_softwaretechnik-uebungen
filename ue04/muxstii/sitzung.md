# Repository-Inhalt und meq-Dateien

**Session ID:** ses_e5d4ead22fferMuKyhEDFhN10V
**Created:** 11/3/2026, 7:34:52 PM
**Updated:** 11/3/2026, 7:35:18 PM

---

## User

Was liegt in diesem Repository? Welche Dateien stammen von mir? Mein Kürzel ist meq. Ändere keine Dateien.

---

## Assistant

_Thinking:_

Let me explore the repository.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current && git status --short | head -30"
}
```

ue04-meq
?? ue04/meq/


**Tool: shell**

**Input:**
```json
{
  "command": "ls -la"
}
```

total 36
drwxrwxr-x   7 user user 4096 Nov  3 19:31 .
drwxr-x---  22 user user 4096 Nov  3 19:23 ..
drwxrwxr-x   7 user user 4096 Nov  3 19:32 .git
-rw-rw-r--   1 user user 2172 Nov  3 19:31 AGENTS.md
-rw-rw-r--   1 user user 3212 Nov  3 19:31 README.md
drwxrwxr-x   3 user user 4096 Nov  3 19:31 ue01
drwxrwxr-x 112 user user 4096 Nov  3 19:31 ue02
drwxrwxr-x  98 user user 4096 Nov  3 19:31 ue03
drwxrwxr-x   4 user user 4096 Nov  3 19:33 ue04


---

## Assistant

**Tool: shell**

**Input:**
```json
{
  "command": "cat README.md"
}
```

# Softwaretechnik — Übungsrepository

Dieses Repository gehört zu den Übungen der Veranstaltung **Softwaretechnik**
(THM, Campus Friedberg, Fachbereich MND). Hier reichen Sie ein, was in den
Übungen entsteht — auf dem Weg, auf dem in Softwareprojekten gearbeitet wird:
über einen eigenen Fork, einen Branch und einen Pull Request.

## Aufbau

Jede Übung hat ein eigenes Verzeichnis mit einer eigenen `README.md`, die
sagt, was dort einzureichen ist.

| Verzeichnis | Übung |
|---|---|
| [`ue01/`](ue01/) | Erste Schritte mit Git und GitHub |
| [`ue02/`](ue02/) | Das Projektmodell am Fall |
| [`ue03/`](ue03/) | Anforderungen an den Terminplaner |
| [`ue04/`](ue04/) | Einen Coding Agent einrichten |

## So reichen Sie etwas ein

1. Legen Sie einmalig einen **Fork** dieses Repositorys an und **klonen** Sie
   ihn auf Ihren Rechner.
2. Legen Sie für jedes Vorhaben einen eigenen **Branch** an.
3. Halten Sie Ihre Änderungen als **Commits** fest und übertragen Sie sie per
   **Push** in Ihren Fork.
4. Stellen Sie einen **Pull Request** an dieses Repository.

Den Weg Schritt für Schritt beschreibt das
[Übungsblatt zur Übung 1](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/).

## Vor jeder weiteren Übung

Dieses Repository wächst mit jeder Übung. Bringen Sie vorher Ihren Fork und
Ihren Rechner auf den neuen Stand:

1. Klicken Sie auf der Startseite Ihres Forks auf **Sync fork → Update
   branch**.
2. Holen Sie den neuen Stand aus dem Fork auf Ihren Rechner:

   ```console
   $ git switch main
   $ git pull
   ```

Den Branch für die neue Übung zweigen Sie erst danach ab.

## Spielregeln

- **Ihr GitHub-Benutzername als Kennung.** Ihre Datei- und Verzeichnisnamen
  sowie Ihre Branches tragen Ihren GitHub-Benutzernamen, und zwar in
  Kleinbuchstaben: Aus `MMustermann` wird `mmustermann`. Anders als ein
  selbst gewähltes Kürzel ist er eindeutig, und er steht ohnehin an jedem
  Pull Request. Ihren Benutzernamen sehen Sie auf GitHub, wenn Sie oben
  rechts auf Ihr Profilbild klicken.
- **Öffentlich ist mehr als der Benutzername.** In jedem Commit stehen Name
  und E-Mail-Adresse aus Ihrer Git-Einrichtung. Wie Sie Ihre Adresse
  verbergen, steht in
  [Aufgabe 0 des Übungsblatts](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/#aufgabe-0--einrichten).
  Schreiben Sie auch in Ihre Dateien nichts, was nicht jeder lesen darf —
  keine Matrikelnummer, keine Anschrift.
- **Nur eigene Dateien.** Sie ändern ausschließlich, was Sie selbst angelegt
  haben; Vorlagen und die Dateien anderer bleiben unberührt. So kommen sich
  die Pull Requests nicht in die Quere.
- **Nicht auf `main` arbeiten.** `main` Ihres Forks folgt allein dem Stand
  dieses Repositorys; nur so lässt er sich später abgleichen.
- **Ein Anliegen je Pull Request**, mit einem Titel, der sagt, was sich
  ändert.
- **Aussagekräftige Commit-Nachrichten**, etwa `Steckbrief für mmustermann anlegen`.

Arbeiten Sie mit einem KI-Agenten, gelten die Spielregeln auch für ihn. Die
Datei [`AGENTS.md`](AGENTS.md) fasst sie für Agenten zusammen; opencode und
andere Coding Agents lesen sie, wenn sie in diesem Repository gestartet
werden.


**Tool: shell**

**Input:**
```json
{
  "command": "find . -path ./.git -prune -o -type d -print | sort | head -80"
}
```

.
./ue01
./ue01/steckbriefe
./ue02
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


---

## Assistant

_Thinking:_

Let me look at the whole structure and the meq directories, plus git history for authorship.

**Tool: shell**

**Input:**
```json
{
  "command": "find . -path ./.git -prune -o -type d -print | sort | tail -60"
}
```

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
./ue03/_vorlage
./ue03/wnga
./ue03/ygue
./ue03/ykar
./ue03/z-266
./ue03/zc
./ue03/zcbn
./ue03/zcoel
./ue03/zsh
./ue04
./ue04/meq
./ue04/_vorlage


**Tool: shell**

**Input:**
```json
{
  "command": "find ue01 ue02/meq ue03 ue04 -maxdepth 3 -not -path '*/.git*' | grep -E 'meq|^ue01|^ue04' | sort"
}
```

ue01
ue01/README.md
ue01/steckbriefe
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
ue01/steckbriefe/_beispiel.md
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
ue01/steckbriefe/dsch.md
ue01/steckbriefe/dsc.md
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
ue01/steckbriefe/lpr2.md
ue01/steckbriefe/Lpr.md
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
ue01/steckbriefe/mken.md
ue01/steckbriefe/MK.md
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
ue01/steckbriefe/_vorlage.md
ue01/steckbriefe/wnga.md
ue01/steckbriefe/yamekk.md
ue01/steckbriefe/ygue.md
ue01/steckbriefe/ykar.md
ue01/steckbriefe/yoibr42.md
ue01/steckbriefe/ysbi82.md
ue01/steckbriefe/Z-266.md
ue01/steckbriefe/ZahraGit12.md
ue01/steckbriefe/zcbn.md
ue01/steckbriefe/zc.md
ue01/steckbriefe/zcoel.md
ue01/steckbriefe/zomj.md
ue02/meq
ue02/meq/notiz.md
ue02/meq/phasenplan.md
ue02/meq/rollen.md
ue02/meq/spezifikation.md
ue03/meq
ue03/meq/anforderungen.md
ue03/meq/kontext.md
ue03/meq/zuordnung.md
ue04
ue04/meq
ue04/meq/einrichtung.md
ue04/README.md
ue04/_vorlage
ue04/_vorlage/einrichtung.md


---

## Assistant

_Thinking:_

Now let me check git history for the meq files — authored by whom. Note repository clone likely contains all commits from upstream. Let me check git log for those paths and author of commits. Also list all files under ue04/meq and contents. Let me also check what's in each exercise folder README and the ue04/meq/einrichtung.md (untracked).

**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline -- ue01/steckbriefe/meq.md ue02/meq ue03/meq ue04/meq | cat"
}
```

ce179ec Übung 3: Ergebnisse von meq (#306)
5b6f0ec Übung 2: Ergebnisse von meq (#171)
e1892ff Steckbrief meq (#2)


**Tool: shell**

**Input:**
```json
{
  "command": "git log --format='%h %an <%ae> %ad %s' --date=short -- ue02/meq ue03/meq ue01/steckbriefe/meq.md | cat"
}
```

ce179ec muxstii <E-Mail entfernt> 2026-11-02 Übung 3: Ergebnisse von meq (#306)
5b6f0ec muxstii <E-Mail entfernt> 2026-10-26 Übung 2: Ergebnisse von meq (#171)
e1892ff muxstii <E-Mail entfernt> 2026-10-20 Steckbrief meq (#2)


**Tool: shell**

**Input:**
```json
{
  "command": "wc -l ue01/steckbriefe/meq.md ue02/meq/*.md ue03/meq/*.md ue04/meq/*.md 2>/dev/null; echo ---; cat ue04/README.md; echo ---; cat ue04/meq/einrichtung.md"
}
```

   17 ue01/steckbriefe/meq.md
   36 ue02/meq/notiz.md
   63 ue02/meq/phasenplan.md
   33 ue02/meq/rollen.md
   89 ue02/meq/spezifikation.md
   18 ue03/meq/anforderungen.md
   31 ue03/meq/kontext.md
   37 ue03/meq/zuordnung.md
   55 ue04/meq/einrichtung.md
  379 total
---
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
---
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

The user asks: what's in this repository? Which files are mine? My abbreviation is meq. Don't change files.

Interesting: the user mentions "Kürzel" meq, while AGENTS.md says usernames in lowercase. But ue04 requires GitHub username in lowercase. The branch is ue04-meq which suggests username meq. Git author is muxstii / muxstii. Hmm, AGENTS.md says ask when unclear which directories belong to person. For ue02 and ue03, meq exists. For ue01/steckbriefe/meq.md exists. So files are consistent with meq being the identifier. But note there's no ue04/meq/sitzung.md — and ue04/meq directory is untracked, containing einrichtung.md which appears to still be the template (unfilled). Actually let me check whether it's a copy of template exactly.

Let me check git status and diff for the untracked dir, and also check whether ue04/meq/einrichtung.md equals ue04/_vorlage/einrichtung.md.

Also need to give overview of repository contents: four exercise dirs, templates, number of participants etc. Let's gather stats.

**Tool: shell**

**Input:**
```json
{
  "command": "diff ue04/_vorlage/einrichtung.md ue04/meq/einrichtung.md > /dev/null && echo \"identisch mit Vorlage\" || echo \"weicht ab\"; ls -la ue04/meq"
}
```

identisch mit Vorlage
total 12
drwxrwxr-x 2 user user 4096 Nov  3 19:33 .
drwxrwxr-x 4 user user 4096 Nov  3 19:33 ..
-rw-rw-r-- 1 user user 1946 Nov  3 19:33 einrichtung.md


**Tool: shell**

**Input:**
```json
{
  "command": "echo \"ue01 Steckbriefe: $(ls ue01/steckbriefe/*.md | wc -l)\"; echo \"ue02 Verzeichnisse: $(find ue02 -mindepth 1 -maxdepth 1 -type d | wc -l)\"; echo \"ue03 Verzeichnisse: $(find ue03 -mindepth 1 -maxdepth 1 -type d | wc -l)\"; echo \"ue04 Verzeichnisse: $(find ue04 -mindepth 1 -maxdepth 1 -type d | wc -l)\"; echo ---; ls ue02/meq ue03/meq; echo ---; git log --oneline -6 | cat"
}
```

ue01 Steckbriefe: 151
ue02 Verzeichnisse: 110
ue03 Verzeichnisse: 96
ue04 Verzeichnisse: 2
---
ue02/meq:
notiz.md
phasenplan.md
rollen.md
spezifikation.md

ue03/meq:
anforderungen.md
kontext.md
zuordnung.md
---
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)
8cfd580 Übung 2: Formatierung der Gesprächsnotiz korrigiert (#286)


---

## Assistant

_Thinking:_

Let me read the user's files briefly to summarize content, and each ue README titles maybe. Let me also check git authorship of ue01/steckbriefe/meq.md — done. Also check whether the local branch contains only these. Let me quickly read the files for content summaries.

**Tool: shell**

**Input:**
```json
{
  "command": "for f in ue01/steckbriefe/meq.md ue02/meq/notiz.md ue02/meq/rollen.md ue02/meq/phasenplan.md ue02/meq/spezifikation.md ue03/meq/kontext.md ue03/meq/anforderungen.md ue03/meq/zuordnung.md; do echo \"### $f\"; head -12 \"$f\"; echo; done"
}
```

### ue01/steckbriefe/meq.md
# Steckbrief <meq>

## Studiengang und Semester

Organisations- und IT-Sicherheit im 3. Semester

…

## Meine bisherige Erfahrung mit Softwareentwicklung

Ich interessiere mich besonders für Cybersecurity, insbesondere SOC und Cloud Security. Ich beschäftige mich mit den Grundlagen und möchte mein technisches Wissen Schritt für Schritt erweitern. Praktische Erfahrungen in der Softwareentwicklung möchte ich im Rahmen der Veranstaltung sammeln.
…

### ue02/meq/notiz.md
# Gesprächsnotiz: Terminplaner für die THM

## Worum es geht

Die THM möchte eine Software zur Planung und Vereinbarung von Terminen. Lehrende bieten Sprechstunden und Prüfungstermine an, Studierende buchen sie, Sekretariate behalten den Überblick.

Die Software soll sich über das Hochschulkonto bedienen lassen. Zunächst soll sie Termine als iCal-Datei zum Herunterladen anbieten, später vielleicht direkt in die Kalender der Beteiligten eintragen.

Außerdem soll sie eine API bekommen, über die KI-Agenten sie steuern können.

Die THM sagte dazu wörtlich:


### ue02/meq/rollen.md
# Rollen — Terminplaner für die THM

Mitgearbeitet haben @muxstii

## Der Kunde

| Bereich | Wer ist das an der THM? | Woran machen Sie es fest? |
|---|---|---|
| Fachbereich (eigentlicher Auftraggeber) | Die Hochschulleitung (Vizepräsidium für Studium und Lehre) stellvertretend für Lehrende, Studierende und Sekretariate | Deren Ziel, die Terminvereinbarung zu vereinfachen, soll das Projekt erreichen. Die Hochschulleitung stellt das Budget und trifft die grundsätzlichen Entscheidungen, die Endanwender sitzen in den Fachbereichen. |
| IT-Bereich | Das Hochschulrechenzentrum (HRZ) der THM | Es betreibt das System später und stellt die Systembasis bereit, z.B. die Anmeldung über das Hochschulkonto und die Server. Was das System leisten soll, bestimmt es nicht. |

## Das Projektteam

### ue02/meq/phasenplan.md
# Phasenplan — Terminplaner für die THM

Kürzel: meq

## Studie

**Ergebnis der Phase:** Projektvorschlag mit Ist-Analyse, bewerteten Lösungsalternativen und Aufwandsschätzung als Entscheidungsgrundlage für die THM

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Aufwand schätzen und einen Meilensteinplan vorschlagen


### ue02/meq/spezifikation.md
# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben  @muxstii


## 1. Ziel des Systems

Der Terminplaner soll den Studierenden und Lehrenden der THM helfen, Termine einfacher zu planen und zu buchen.
Lehrende können Termine anbieten und Studierende können diese online buchen.

## 2. Benutzer des Systems


### ue03/meq/kontext.md
# Stakeholder und Systemkontext — Terminplaner für die THM

## Stakeholder

| Stakeholder | Worauf hat er Einfluss? |
|---|---|
| Lehrende | Welche Sprechstunden und Prüfungstermine angeboten werden und wie sich das Anlegen und Verwalten von Terminen anfühlen muss. |
| Studierende | Wie das Suchen, Buchen und Stornieren von Terminen abläuft und ob das System überhaupt angenommen wird. |
| Sekretariate | Welche Übersichten über Termine und Buchungen ihres Bereichs nötig sind. |
| Hochschulleitung (Auftraggeber) | Budget, Umfang und Zeitplan des Projekts sowie die grundsätzlichen Entscheidungen. |
| Rechenzentrum der THM | Betrieb, Systembasis und die Anbindung an das Hochschulkonto. |
| Datenschutzbeauftragte der THM | Welche personenbezogenen Daten gespeichert, wie lange sie aufbewahrt und wer sie sehen darf. |

### ue03/meq/anforderungen.md
# Anforderungen — Terminplaner für die THM

| Nr. | Anforderung | Stakeholder | Art |
|---|---|---|---|
| A01 | Studierende können nach einer Lehrperson suchen. | Studierende | FA |
| A02 | Lehrpersonen können einstellen, wie lange ihre Sprechstunden dauern. | Lehrpersonen | FA |
| A03 | Studierende können einen gebuchten Termin verschieben. | Studierende | FA |
| A04 | Studierende können nach freien Terminen an einem bestimmten Tag suchen. | Studierende | FA |
| A05 | Der Terminplaner soll einfach zu bedienen sein. | Studierende | QA |
| A06 | Man soll den Terminplaner auch auf dem Handy gut benutzen können. | Studierende | QA |
| A07 | Für die Anmeldung braucht man ein Hochschulkonto der THM. | Studierende | RB |
| A08 | Der Terminplaner soll bis zum Sommersemester 2027 fertig sein. | THM | RB |

### ue03/meq/zuordnung.md
# Anforderung oder Lösung? — Terminplaner für die THM

Kürzel: meq

## Funktionale Anforderung (FA)

- Studierende können einen freien Sprechstundentermin bei einer Lehrperson buchen.
- Ein bereits gebuchter Termin kann kein zweites Mal gebucht werden.
- Sagt eine Lehrperson eine Sprechstunde ab, erhalten alle, die gebucht haben, eine Nachricht.
- Jeder gebuchte Termin lässt sich als iCal-Datei herunterladen.
- Ein Sekretariat sieht alle Prüfungstermine seines Fachbereichs auf einen Blick.
- Über die API kann ein KI-Agent freie Termine abfragen und im Namen einer Person buchen.



---

## Assistant

_Thinking:_

Now compose answer in German. No file changes. Explain repo structure, the four exercises, which files are theirs (based on commits by the same author and path name meq), plus ue04 status: untracked directory containing an untouched copy of the template, missing sitzung.md, and note the branch is ue04-meq (not main), so fine.

Also mention per AGENTS.md: ue04 requires GitHub username lowercased; "meq" is treated as their identifier per branch and dirs, but note their GitHub account appears as @muxstii in the files. Hmm — that's a point worth flagging: README says GitHub username in lowercase must be used, and the files under ue02 contain @muxstii. The branch is ue04-meq. The user says "Mein Kürzel ist meq" — but the rules say username, not chosen abbreviation. Potential mismatch: ue04 requires `ue04/<benutzername>/` and branch `ue04-<benutzername>`; if the GitHub username is muxstii, then ue04/meq may be wrong. But AGENTS.md says older directories may carry an earlier chosen abbreviation and still belong to the person. For ue04 though, README explicitly says GitHub username. That's a useful observation but since user asked "which files are mine" and said abbreviation is meq, I should mention the conflict gently and ask? Plan mode—just inform. Also mention that I shouldn't decide. Let me verify the ue02/ue03 commit files exactly, to list all files authored. Let me get file lists per commit to be accurate.

**Tool: shell**

**Input:**
```json
{
  "command": "for c in e1892ff 5b6f0ec ce179ec; do echo \"## $c\"; git show --stat --format='%s' --name-only $c | sed '/^$/d'; done"
}
```

## e1892ff
Steckbrief meq (#2)
ue01/steckbriefe/meq.md
## 5b6f0ec
Übung 2: Ergebnisse von meq (#171)
ue02/meq/notiz.md
ue02/meq/phasenplan.md
ue02/meq/rollen.md
ue02/meq/spezifikation.md
## ce179ec
Übung 3: Ergebnisse von meq (#306)
ue03/meq/anforderungen.md
ue03/meq/kontext.md
ue03/meq/zuordnung.md


**Tool: shell**

**Input:**
```json
{
  "command": "git log --format='%h %s' --author='muxstii' | head -20; echo ---; git config user.name; git config user.email; echo ---; ls ue04/meq"
}
```

ce179ec Übung 3: Ergebnisse von meq (#306)
5b6f0ec Übung 2: Ergebnisse von meq (#171)
e1892ff Steckbrief meq (#2)
---
muxstii
[E-Mail entfernt]
---
einrichtung.md


---

## Assistant

Ich habe nur gelesen, nichts geändert.

## Was im Repository liegt

Ein Übungsrepository zur Veranstaltung **Softwaretechnik** (THM Friedberg). Aufbau:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | Erste Schritte mit Git/GitHub; `steckbriefe/` mit 151 Steckbriefen plus `_vorlage.md` und `_beispiel.md` |
| `ue02/` | Projektmodell am Fall „Terminplaner der THM“; 110 Personenverzeichnisse plus `_vorlage/` |
| `ue03/` | Anforderungen an den Terminplaner; 96 Personenverzeichnisse plus `_vorlage/` |
| `ue04/` | Einen Coding Agent einrichten; `_vorlage/` und bisher erst 2 Personenverzeichnisse |
| `README.md`, `AGENTS.md` | Spielregeln für Menschen bzw. KI-Agenten (eigene Dateien, nicht auf `main`, keine persönlichen Daten, Push/PR nur auf Bitte) |

Aktueller Branch: `ue04-meq`. In `ue02` und `ue03` liegen die Ergebnisse vieler Kommilitonen; das Repo wächst pro Übung.

## Deine Dateien

Belegt über die Commits von `muxstii` (GitHub: `@muxstii`) und die Namenskennung `meq`:

**Bereits committet (aus früheren Übungen, aus deinem Fork übernommen):**
- `ue01/steckbriefe/meq.md` — Steckbrief (Studiengang Organisations- und IT-Sicherheit, Interesse an Cybersecurity/SOC/Cloud Security)
- `ue02/meq/notiz.md` — Gesprächsnotiz zum Terminplaner
- `ue02/meq/rollen.md` — Kunde und Projektteam
- `ue02/meq/phasenplan.md` — Phasenplan (Kürzel `meq`)
- `ue02/meq/spezifikation.md` — Gliederung der Spezifikation
- `ue03/meq/kontext.md` — Stakeholder und Systemkontext
- `ue03/meq/anforderungen.md` — Anforderungstabelle A01–A08
- `ue03/meq/zuordnung.md` — Einordnung FA/QA/RB

**Noch unversioniert (Stand jetzt):**
- `ue04/meq/einrichtung.md` — eine **unveränderte Kopie** von `ue04/_vorlage/einrichtung.md`; alle „…“ sind noch Platzhalter. `git status` zeigt `?? ue04/meq/`.

Für Übung 4 fehlen also noch das Ausfüllen von `einrichtung.md` und die Datei `sitzung.md` (Agenten-Export).

## Ein Hinweis zur Kennung

Laut `README.md` und `ue04/README.md` muss für Übung 4 der **GitHub-Benutzername in Kleinbuchstaben** verwendet werden (Verzeichnis `ue04/<benutzername>/`, Branch `ue04-<benutzername>`). Dein GitHub-Konto erscheint in den Dateien als `@muxstii`, Branch und Verzeichnis tragen aber `meq`. Für `ue02`/`ue03` ist das laut `AGENTS.md` unproblematisch (ältere Kürzel bleiben gültig), für `ue04` könnte es beanstandet werden. Das solltest du vor dem Einreichen selbst entscheiden — sag Bescheid, wenn ich das genauer prüfen soll.
