# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e54d4e273ffeaO9CapYP5TyxUM
**Created:** 5.11.2026, 11:04:52
**Updated:** 5.11.2026, 11:05:27

---

## User

was liegt in diesem repository, und welche dateien stammen von mir 

---

## Assistant

_Thinking:_

Let me explore the repository.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current; git status --short; git log --oneline -5"
}
```

ue04-bblj09
?? ue04/bblj09/
b5dbd3a Ü2: Ergebnisse von thm-nos (#400)
122ab21 Ergebnisse der Phasen ergänzen (#396)
fcf17f4 Übung 2: Ergebnisse von pz01 (#330)
babf65e Ue02 real (#322)
bf88cc9 Übung 2 ivlbs (#311)


**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\bblj09\\Documents\\thm_wk-1208_softwaretechnik-uebungen"
}
```

Read directory C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen, entries 1-7
.git\
ue01\
ue02\
ue03\
ue04\
AGENTS.md
README.md

---

## Assistant

_Thinking:_

Branch ue04-bblj09 → username bblj09. Let's look deeper.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Recurse -File -Path ue04\\bblj09 | Select-Object FullName, Length; git status --porcelain -uall"
}
```


?? ue04/bblj09/einrichtung.md
FullName                                                                                   Length
--------                                                                                   ------
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue04\bblj09\einrichtung.md   2053




**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\bblj09\\Documents\\thm_wk-1208_softwaretechnik-uebungen\\README.md"
}
```

Read file C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\README.md, lines 1-74
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

Let's look at the overall structure: ue01, ue02, ue03, ue04 contents. And read ue04/bblj09/einrichtung.md and ue04/README.md.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Directory | ForEach-Object { \"== $($_.Name) ==\"; Get-ChildItem -Directory $_.FullName | Select-Object -ExpandProperty Name }"
}
```

== ue01 ==
steckbriefe
== ue02 ==
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
_vorlage
_zugabe
== ue03 ==
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
_vorlage
== ue04 ==
bblj09
_vorlage


**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\bblj09\\Documents\\thm_wk-1208_softwaretechnik-uebungen\\ue04\\bblj09\\einrichtung.md"
}
```

Read file C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue04\bblj09\einrichtung.md, lines 1-55
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
12: | Läuft der Agent? | ja |
13: | Werkzeug | opencode |
14: | Version | 2.2.5 |
15: | Betriebssystem | Windows |
16: | Modellzugang | OpenCode Zen (kostenlos) |
17: | Modell | DeepSeek V4.1 Flash Free |
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

**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\bblj09\\Documents\\thm_wk-1208_softwaretechnik-uebungen\\ue04\\README.md"
}
```

Read file C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue04\README.md, lines 1-40
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

Now, which files "stammen von mir" — user is bblj09 (branch ue04-bblj09). There is ue02/bblj09, ue03/bblj09, ue04/bblj09. Let's list those. Also check git log for commits by author maybe. Let's inspect files in those dirs and git history for them.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Recurse -File -Path ue02\\bblj09, ue03\\bblj09 | Select-Object FullName, Length; git log --oneline --author-date-order -- ue02/bblj09 ue03/bblj09 ue04/bblj09; git config user.name; git config user.email"
}
```


2d536eb Übung 3 - Anforderung -  bblj09 (#372)
0db1ea0 Ue02 bblj09 (#227)
bblj09
[E-mail entfernt]
FullName                                                                                     Length
--------                                                                                     ------
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\notiz.md           1408
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\phasenplan.md      3733
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\spezifikation.md    855
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\anforderungen.md   1574
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\kontext.md         2719
C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\zuordnung.md       1825




**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Directory ue01\\steckbriefe | Select-Object -ExpandProperty Name | Select-String -Pattern \"bblj09\" -SimpleMatch; Get-ChildItem ue01\\steckbriefe -Filter \"*bblj09*\" -Recurse"
}
```



    Verzeichnis: C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
-a----        25.10.2026     22:38            441 Bblj09.md                                                            




---

## Assistant

_Thinking:_

Let me check the ue01 steckbrief to confirm ownership details, and maybe list commit subjects. Also check whether there are other dirs possibly belonging to the person under alternate initials? AGENTS says older dirs might use a chosen abbreviation; but no indication. bblj09 in ue02, ue03, ue04, ue01 steckbrief Bblj09.md.

Let me read files briefly to summarize content.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-Content ue01\\steckbriefe\\Bblj09.md; \"== ue02 notiz ==\"; Get-Content ue02\\bblj09\\notiz.md; \"== ue02 spez ==\"; Get-Content ue02\\bblj09\\spezifikation.md"
}
```

# Steckbrief Bblj09

## Studiengang und Semester
Wirtschaftsinformatik (Bachelor), 5.Semester


## Meine bisherige Erfahrung mit Softwareentwicklung
Ich habe im Studium erste Erfahrungen mit Java gesammelt. Dabei habe ich kleinere Programme und �obungsaufgaben bearbeitet.


## Das erwarte ich von der Veranstaltung
Ich m��chte lernen, wie man Softwareprojekte strukturiert plant und gemeinsam mit Git und Github bearbeitet
�?�
== ue02 notiz ==


# Gespr��chsnotiz: Terminplaner fǬr die THM
## Worum es geht
Die THM m��chte eine Software zur Planung und Vereinbarung von Terminen. Lehrende bieten Sprechstunden und PrǬfungstermine an, Studierende buchen sie, Sekretariate behalten den �oberblick.
Die Software soll sich Ǭber das Hochschulkonto bedienen lassen. Zun��chst soll sie Termine als iCal-Datei zum Herunterladen anbieten, sp��ter vielleicht direkt in die Kalender der Beteiligten eintragen.
Au�Yerdem soll sie eine API bekommen, Ǭber die KI-Agenten sie steuern k��nnen.
Die THM sagte dazu w��rtlich:
> Wir wollen nicht noch ein Werkzeug, das am Ende keiner benutzt.

**Wichtig: Noch ist nichts beauftragt, wir sollen zuerst einen Vorschlag machen.**
## Was heute benutzt wird
- E-Mail
- Listen an der BǬrotǬr
- Werkzeuge im Netz, n��mlich
  - [DFN-Terminplaner](https://terminplaner6.dfn.de/de)
  - [Doodle](https://doodle.com/de/)
## N��chste Schritte
1. Diese Notiz mit der THM abstimmen.
2. Einen Phasenplan vorlegen, Datei `phasenplan.md`.
3. Die Rollen kl��ren, Datei `rollen.md`.
## Offene Punkte
| Punkt | Wer kl��rt | Bis wann |
| --- | --- | --- |
| Wer nimmt fǬr die THM an den Gespr��chen teil? | Die THM | bis zum n��chsten Gespr��ch. |
| Bis wann soll die Software eingefǬhrt sein? | Die THM | bis zum n��chsten Gespr��ch. |
| Wer aus unserer Firma leitet das Projekt? | Wir | in dieser Woche. |
== ue02 spez ==
# Spezifikation des Terminplaners �?" Gliederung und Beispiele

Mitgearbeitet: bblj09

<!-- Je Abschnitt Ihrer Gliederung eine �oberschrift (## fǬr Abschnitte, ###
     fǬr Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten wǬrden.
     Die beiden �oberschriften unten sind lediglich Platzhalter. -->

## 1. Benutzergruppen und Funktionen

Lehrende bieten Sprechstunden und PrǬfungstermine an, Studierende buchen sie und Sekretariate behalten den �oberblick.
Beispiel: Studierende w��hlen einen freien Sprechstundentermin aus und buchen ihn.

## 2. Angaben zu einem Termin

FǬr einen Termin mǬssen die ben��tigten Angaben festgelegt werden.
Beispiel: Ein Sprechstundentermin k��nnte Datum, Uhrzeit, Raum und den Namen der Lehrperson enthalten.




**Tool: shell**

**Input:**
```json
{
  "command": "\"== ue02 phasenplan ==\"; Get-Content ue02\\bblj09\\phasenplan.md; \"== ue03 anforderungen ==\"; Get-Content ue03\\bblj09\\anforderungen.md"
}
```

== ue02 phasenplan ==
# Phasenplan �?" Terminplaner fǬr die THM

KǬrzel: bblj09

## Studie

**Ergebnis der Phase:** Bewertete L��sungsalternativen und begrǬndeter Projektvorschlag mit Aufwandssch��tzung und grobem Meilensteinplan.

- Eigenentwicklung, Anpassung einer Open-Source-L��sung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und PrǬfungstermine bisher vereinbart werden und wo es hakt
- Aufwand sch��tzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Abgestimmte Beschreibung der fachlichen Anforderungen, Abl��ufe und Daten sowie der sp��teren Abnahmekriterien.

- Mit Lehrenden und Sekretariaten Schritt fǬr Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorg��nge ein KI-Agent Ǭber die API ausl��sen darf �?" z.B. freie Termine abfragen und buchen, aber keine PrǬfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin geh��ren und wie Termine, Personen und R��ume zusammenh��ngen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Testf��lle formulieren, an denen sich sp��ter zeigt, ob das System leistet, was vereinbart wurde

## Systemkonstruktion

**Ergebnis der Phase:** Technischer Entwurf mit Komponenten, Schnittstellen, Technologieauswahl und Aufbauplan.

- Das System in Komponenten zerlegen �?" z.B. Terminverwaltung, Benachrichtigung, Anmeldung �?" und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework ausw��hlen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Mit einem technischen Prototyp prǬfen, ob die Anmeldung Ǭber das Hochschulkonto funktioniert
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** Programmierte und einzeln getestete Komponenten.

- Die Komponente �?zBenachrichtigung�?o programmieren
- Die fertige Komponente �?zTerminverwaltung�?o fǬr sich testen, ehe sie mit anderen zusammenkommt

## Integration & EinfǬhrung

**Ergebnis der Phase:** ZusammengefǬhrtes, geprǬftes, vom Auftraggeber abgenommenes und eingefǬhrtes System.

- Die THM installiert das System in ihrer eigenen Umgebung und prǬft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenfǬhren und ihr Zusammenspiel gegen Testf��lle prǬfen
- Das System als Ganzes unter FederfǬhrung des Qualit��tsbeauftragten gegen die Testf��lle prǬfen
- Mit einem KI-Agenten prǬfen, ob sich ein Sprechstundentermin vollst��ndig Ǭber die API buchen l��sst
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Im Betrieb betreutes, korrigiertes und bedarfsgerecht weiterentwickeltes

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline fǬr Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste fǬr ausgebuchte Termine nachrǬsten, die sich die Lehrenden nach einem Semester wǬnschen

## Bei welchen Karten waren Sie unsicher �?" und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: �?" -->
== ue03 anforderungen ==
# Anforderungen �?" Terminplaner fǬr die THM

| Nr. | Anforderung | Stakeholder | Art |
|---|---|---|---|
| A01 | Lehrende k��nnen Sprechstunden mit Datum, Uhrzeit und Dauer anbieten. | Lehrende | FA |
| A02 | Lehrende k��nnen PrǬfungstermine anlegen und fǬr Buchungen freigeben. | Lehrende | FA |
| A03 | Studierende k��nnen eine eigene Buchung stornieren. | Studierende | FA |
| A04 | Sekretariate k��nnen alle Termine ihres Fachbereichs nach Datum und Lehrperson filtern. | Sekretariate | FA |
| A05 | Das System erm��glicht den Export gebuchter Termine als iCal-Datei. | Studierende | FA |
| A06 | Neue Nutzende k��nnen ihren ersten Termin ohne Anleitung innerhalb von 5 Minuten buchen. | Studierende | QA |
| A07 | Die TerminǬbersicht l��dt bei normaler Last in unter 3 Sekunden. | Studierende | QA |
| A08 | Das System ist au�Yer in angekǬndigten Wartungsfenstern jederzeit erreichbar. | Lehrende | QA |
| A09 | Der Zugriff ist nur fǬr Angeh��rige der THM mit gǬltigem Hochschulkonto m��glich. | Verantwortliche der THM | RB |
| A10 | Die Nutzung durch KI-Agenten l��uft Ǭber eine dokumentierte Schnittstelle, die die THM freigibt. | Hochschul-IT | RB |
| A11 | Personenbezogene Daten werden nach den Vorgaben der DSGVO verarbeitet. | Datenschutzverantwortliche der THM | RB |

## Eine Anforderung, die niemand ausgesprochen hat

A11: Im Gespr��ch ging es um Termine, Hochschulkonto und KI-Schnittstelle, aber niemand nannte den Datenschutz. Er gilt trotzdem, denn Termindaten verknǬpfen Namen von Personen mit Sprechzeiten und PrǬfungen.


---

## Assistant

_Thinking:_

Also ue03 kontext.md, zuordnung.md. Let's peek quickly and count. Also check git status for sitzung.md missing. And verify the files in ue04 folder untracked; the einrichtung.md says sitzung.md should exist but doesn't. Note that in answer maybe.

Let me read remaining two files quickly.

**Tool: shell**

**Input:**
```json
{
  "command": "\"== kontext ==\"; Get-Content ue03\\bblj09\\kontext.md; \"== zuordnung ==\"; Get-Content ue03\\bblj09\\zuordnung.md"
}
```

== kontext ==
# Stakeholder und Systemkontext �?" Terminplaner fǬr die THM

## Stakeholder

| Stakeholder | Worauf hat er Einfluss? |
|---|---|
| Lehrende | Sie bestimmen, welche Angaben und Abl��ufe sie zum Anbieten von Sprechstunden und PrǬfungsterminen ben��tigen. |
| Studierende | Sie beeinflussen die Anforderungen an das Finden und Buchen von Terminen sowie an eine verst��ndliche Bedienung. |
| Sekretariate | Sie bestimmen, welche �obersichten sie zur organisatorischen Betreuung der Termine ben��tigen. |
| Verantwortliche der THM | Sie kl��ren Projektziele, EinfǬhrungstermin und Umfang eines m��glichen Auftrags; ihre konkreten Vertreter sind noch offen. |
| Hochschul-IT (angenommen) | Sie beeinflusst die technischen und betrieblichen Vorgaben sowie die Anbindung an das Hochschulkonto. |
| Datenschutzverantwortliche der THM (angenommen) | Sie beeinflussen die Vorgaben zum Umgang mit personenbezogenen Termin- und Kontodaten. |

## Systemkontext

Das betrachtete System ist die neue Terminplaner-Software.
Personen, externe Systeme und organisatorische Abl��ufe,
mit denen sie zusammenwirkt, liegen au�Yerhalb ihrer Systemgrenze.

| Aspekt | Art | Warum geh��rt er zum Kontext? |
|---|---|---|
| Lehrende | Person | Sie stellen Sprechstunden und PrǬfungstermine im Terminplaner bereit. |
| Studierende | Person | Sie w��hlen angebotene Termine aus und buchen diese. |
| Sekretariate | Person | Sie nutzen den Terminplaner, um den �oberblick Ǭber Termine zu behalten. |
| Hochschulkonto bzw. zugeh��riger Anmeldedienst | System im Betrieb | Die Software soll Ǭber das Hochschulkonto nutzbar sein; die genaue Anbindung ist noch zu kl��ren. |
| Kalenderprogramme der Beteiligten | System im Betrieb | Sie sollen die heruntergeladenen iCal-Dateien Ǭbernehmen k��nnen; eine direkte Eintragung ist erst eine m��gliche sp��tere Erweiterung. |
| Heruntergeladene iCal-Datei | Dokument | Sie Ǭbertr��gt Termininformationen aus dem Terminplaner an die Kalenderprogramme. |
| Externe KI-Agenten | System im Betrieb | Sie sollen den Terminplaner Ǭber dessen API steuern k��nnen; die Agenten selbst geh��ren nicht zum Terminplaner. |
| Vereinbarung von Sprechstunden und PrǬfungsterminen | Prozess | Diesen organisatorischen Ablauf soll die neue Software unterstǬtzen. |

## Irrelevante Umgebung

- Mensaspeisepl��ne: FǬr die beschriebenen Funktionen zur Terminplanung ist keine Wechselwirkung mit Speisepl��nen erkennbar.
- Bibliotheksausleihe: Das Ausleihen und ZurǬckgeben von Medien geh��rt nicht zum beschriebenen Zweck des Terminplaners.

Diese Abgrenzung gilt fǬr den aktuell beschriebenen Umfang.
Falls weitere Anforderungen hinzukommen, muss sie erneut geprǬft werden.
== zuordnung ==
# Anforderung oder L��sung? �?" Terminplaner fǬr die THM

KǬrzel: bblj09

## Funktionale Anforderung (FA)

- Studierende k��nnen einen freien Sprechstundentermin bei einer Lehrperson buchen.
- Ein bereits gebuchter Termin kann kein zweites Mal gebucht werden.
- Sagt eine Lehrperson eine Sprechstunde ab, erhalten alle, die gebucht haben, eine Nachricht.
- Jeder gebuchte Termin l��sst sich als iCal-Datei herunterladen.
- Ein Sekretariat sieht alle PrǬfungstermine seines Fachbereichs auf einen Blick.
- �ober die API kann ein KI-Agent freie Termine abfragen und im Namen einer Person buchen.

## Qualit��tsanforderung (QA)

- Eine Buchung ist fǬr Studierende in h��chstens drei Schritten abgeschlossen.
- Auch zu Beginn der PrǬfungsanmeldung, wenn bis zu 2.000 Personen zugleich buchen, zeigt das System eine Seite in weniger als zwei Sekunden an.
- Die Buchungsseite ist mit einem Screenreader vollst��ndig bedienbar.

## Randbedingung (RB)

- Die Anmeldung erfolgt ausschlie�Ylich Ǭber das Hochschulkonto.
- Die erste Ausbaustufe geht zum Sommersemester 2027 in Betrieb.
- Personenbezogene Daten werden nach den Vorgaben der EU-DSGVO verarbeitet.
- Das System wird im Rechenzentrum der THM betrieben.

## Keine Anforderung �?" L��sung (WIE)

- Die API nimmt Anfragen als REST-Aufrufe entgegen und antwortet in JSON.
- Vor jeder Buchung fragt die Komponente �?zBuchung�?o bei der Komponente �?zKalender�?o an, ob der Termin noch frei ist.
- Termine werden in einer PostgreSQL-Datenbank gespeichert.

## Bei welchen Karten waren Sie unsicher �?" und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue03-anforderung-oder-loesung: k01=fa k02=wie k03=rb k04=qa k05=fa k06=rb k07=wie k08=fa k09=rb k10=qa k11=wie k12=fa k13=qa k14=fa k15=rb k16=fa | unsicher: �?" -->


**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files | Measure-Object -Line; git ls-files | Where-Object { $_ -match \"bblj09|Bblj09\" }; git log --oneline -3 --format=\"%h %an %s\" -- ue04/bblj09"
}
```


Lines Words Characters Property
----- ----- ---------- --------
  782                          
ue01/steckbriefe/Bblj09.md
ue02/bblj09/notiz.md
ue02/bblj09/phasenplan.md
ue02/bblj09/spezifikation.md
ue03/bblj09/anforderungen.md
ue03/bblj09/kontext.md
ue03/bblj09/zuordnung.md




---

## Assistant

_Thinking:_

Interesting: git ls-files doesn't show ue04/bblj09 because it's untracked. So the ue04/einrichtung.md is new/untracked.

Also note ue02/bblj09 includes notiz.md — that may be a copy of exercise material (notiz.md is likely given by exercise). Fine.

Let me also count total structure: 4 exercise dirs, 782 tracked files. Let me give an overview: ue01 steckbriefe (~? files), ue02 ~105 dirs, ue03 ~95 dirs, ue04 only bblj09 + _vorlage.

Check counts quickly.

**Tool: shell**

**Input:**
```json
{
  "command": "\"ue01 steckbriefe: \" + (Get-ChildItem ue01\\steckbriefe -File).Count; \"ue02 Unterordner: \" + (Get-ChildItem ue02 -Directory).Count; \"ue03 Unterordner: \" + (Get-ChildItem ue03 -Directory).Count; \"ue04 Unterordner: \" + (Get-ChildItem ue04 -Directory).Count; Get-ChildItem ue04\\_vorlage"
}
```

ue01 steckbriefe: 151
ue02 Unterordner: 110
ue03 Unterordner: 96
ue04 Unterordner: 2


    Verzeichnis: C:\Users\bblj09\Documents\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
-a----        05.11.2026     10:46           2001 einrichtung.md                                                       




---

## Assistant

_Thinking:_

Now compose answer in German. Mention branch ue04-bblj09, username bblj09. List repo contents, then personal files. Mention einrichtung.md is untracked and sitzung.md missing (required for ue04). Also note encoding issue (mojibake) in files? The display shows broken umlauts — could be PowerShell console encoding, not necessarily file. Don't overstate. Maybe mention it's likely just terminal encoding.

I'll answer concisely.

## Das Repository

Es ist das Übungsrepository zur Veranstaltung **Softwaretechnik** (THM Friedberg). Auf `main` liegen 782 versionierte Dateien in vier Übungsverzeichnissen:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | `steckbriefe/` mit 151 Steckbriefen, je eine Markdown-Datei pro Person |
| `ue02/` | 110 Unterordner, je Person eine Ausarbeitung zum Projektmodell |
| `ue03/` | 96 Unterordner, je Person Anforderungen an den Terminplaner |
| `ue04/` | bisher nur `_vorlage/` und dein Ordner `bblj09/` |

Dazu kommen `README.md` (Spielregeln) und `AGENTS.md` (Hinweise für KI-Agenten). Aktueller Branch: **`ue04-bblj09`**, also ist dein GitHub-Benutzername **`bblj09`**.

## Deine Dateien

Versioniert (committet):

- `ue01/steckbriefe/Bblj09.md` – Steckbrief (Studiengang, Vorerfahrung, Erwartungen)
- `ue02/bblj09/notiz.md` – Gesprächsnotiz zum Terminplaner
- `ue02/bblj09/phasenplan.md` – Phasenplan mit allen SWT-Phasen
- `ue02/bblj09/spezifikation.md` – Gliederung der Spezifikation mit Beispielen
- `ue03/bblj09/anforderungen.md` – 11 Anforderungen (FA/QA/RB) plus eine unausgesprochene Anforderung
- `ue03/bblj09/kontext.md` – Stakeholder, Systemkontext, irrelevante Umgebung
- `ue03/bblj09/zuordnung.md` – Einordnung in FA, QA, RB und „Lösung (WIE)“

Noch **nicht** versioniert (steht als `??` in `git status`):

- `ue04/bblj09/einrichtung.md` – ausgefüllte Vorlage für Übung 4 (Agent läuft, opencode 2.2.5, Windows, OpenCode Zen, DeepSeek V4.1 Flash Free). Die Abschnitte „Antwort des Agenten geprüft“ und „Wenn es nicht läuft“ sind noch Platzhalter.

Auffällig: Für Übung 4 fehlt laut `ue04/README.md` noch die Datei **`sitzung.md`** (Export der Agentensitzung) neben `einrichtung.md`. Außerdem enthalten die Dateien teils kaputte Umlaute (`fǬr`, `�?"`) — das kann an der Konsolenausgabe liegen, lohnt aber einen Blick im Editor, bevor du committest.
