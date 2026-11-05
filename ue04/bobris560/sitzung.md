# Repository-Inhalt und eigene Dateien

**Session ID:** ses_e52827bfaffeoGh5YIeEya46St
**Created:** 5.11.2026, 21:54:06
**Updated:** 5.11.2026, 21:55:54

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

Let me explore the repository to answer. Need to check branch, git status, directory structure, and figure out which files belong to the user. The AGENTS.md says username is in branch name. Let me check.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current; git status --short; git remote -v"
}
```

ue04-bobris560
origin	https://github.com/Bobris560/thm_wk-1208_softwaretechnik-uebungen.git (fetch)
origin	https://github.com/Bobris560/thm_wk-1208_softwaretechnik-uebungen.git (push)


**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\kassi\\thm_wk-1208_softwaretechnik-uebungen\\README.md"
}
```

Read file C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\README.md, lines 1-74
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

Branch: ue04-bobris560. Let me list directory structure and find files under ue04/bobris560 or similar.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Force | Select-Object Mode,Name; Get-ChildItem -Directory ue0* | Select-Object FullName"
}
```


Mode   Name     
----   ----     
d--h-- .git     
d----- ue01     
d----- ue02     
d----- ue03     
d----- ue04     
-a---- AGENTS.md
-a---- README.md
                
                
                
                




**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline -20; git log --oneline --author=\"Bobris560\" -20"
}
```

66eafe1 ue04: einrichtung.md ausgefüllt
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
f8b8fd7 Steckbrief slr63 (#258)
eddf457 Steckbrief wnga (#244)
9ce2e16 Steckbrief hinzufügen (#239)
d1b75bb Steckbrief von ssng61 (#232)


---

## Assistant

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Recurse ue01,ue02,ue03,ue04 -File | Select-Object FullName | Format-Table -AutoSize -Wrap"
}
```

gen\ue02\dsch\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\flk\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\flk\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\flk\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro\notiz.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro\phasenplan.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro\spezifikation.md     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\hams\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\hams\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\hams\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j\notiz.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j\phasenplan.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j\spezifikation.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ivlbs\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ivlbs\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ivlbs\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\rollen.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\rollen.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jemy\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jemy\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jemy\rollen.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jemy\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jsug\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jsug\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jsug\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng\rollen.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\lom\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\lom\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\lom\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte\notiz.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte\phasenplan.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte\spezifikation.md      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\notiz.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\phasenplan.md   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\rollen.md       
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\spezifikation.md
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04\notiz.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04\phasenplan.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04\spezifikation.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\rollen.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mk\phasenplan.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mu\notiz.md                      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mu\phasenplan.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mu\spezifikation.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mw\notiz.md                      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mw\phasenplan.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\mw\spezifikation.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\my55\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\my55\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\my55\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino\notiz.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino\phasenplan.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino\spezifikation.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nko\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nko\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nko\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\NN\notiz.md                      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\NN\phasenplan.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\NN\spezifikation.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nohl\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nohl\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\nohl\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pz01\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pz01\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\pz01\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\rollen.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qho\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qho\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\qho\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\real\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\real\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\real\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\renn\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\renn\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\renn\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\rollen.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sam\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sam\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sam\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\rollen.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\skt435\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\skt435\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\snab\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\snab\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\snab\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ssda78\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ssda78\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ssng61\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ssng61\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\rollen.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004\notiz.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004\phasenplan.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004\spezifikation.md      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\thm-nos\notiz.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\thm-nos\phasenplan.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\thm-nos\spezifikation.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\thng\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\thng\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\thng\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\rollen.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\phasenplan.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\rollen.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\rollen.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82\notiz.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82\spezifikation.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\notiz.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\phasenplan.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\spezifikation.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\notiz.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\phasenplan.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\spezifikation.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\notiz.md                     
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\phasenplan.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\spezifikation.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\notiz.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\spezifikation.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue02\_zugabe\rollen.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\README.md                        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\af\anforderungen.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\af\kontext.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\af\zuordnung.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088\anforderungen.md       
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088\kontext.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088\zuordnung.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka\anforderungen.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka\kontext.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka\zuordnung.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507\anforderungen.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507\kontext.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507\zuordnung.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\anforderungen.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\kontext.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\zuordnung.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710\anforderungen.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710\kontext.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710\zuordnung.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j\anforderungen.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j\kontext.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j\zuordnung.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\lom\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\lom\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\lom\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte\anforderungen.md      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte\kontext.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte\zuordnung.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer\anforderungen.md
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer\kontext.md      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer\zuordnung.md    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\meq\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\meq\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\meq\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\MK\anforderungen.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\MK\kontext.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\MK\zuordnung.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\moh\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\moh\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\moh\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mskk15\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mskk15\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mu\anforderungen.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mu\kontext.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mu\zuordnung.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mw\anforderungen.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mw\kontext.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\mw\zuordnung.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\my55\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\my55\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\my55\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino\anforderungen.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino\kontext.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino\zuordnung.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nko\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nko\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nko\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\NN\anforderungen.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\NN\kontext.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\NN\zuordnung.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\qho\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\qho\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\qho\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\real\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\real\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\real\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sam\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sam\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sam\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\snab\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\snab\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\snab\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\talh\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\talh\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\talh\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004\anforderungen.md      
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004\kontext.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004\zuordnung.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\trry\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\trry\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\trry\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc\anforderungen.md          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc\kontext.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc\zuordnung.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\val\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\val\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\val\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\virus\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\virus\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\virus\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zc\anforderungen.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zc\kontext.md                    
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zc\zuordnung.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn\anforderungen.md            
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn\kontext.md                  
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn\zuordnung.md                
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\anforderungen.md           
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\kontext.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\zuordnung.md               
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\anforderungen.md             
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\kontext.md                   
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\zuordnung.md                 
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\anforderungen.md        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\kontext.md              
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue04\README.md                        
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue04\bobris560\einrichtung.md         
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage\einrichtung.md          




[showing lines 228-786 of 786; full output saved to C:\Users\bobris560\.local\share\opencode\shell\db81af6394f73070215e49f808b1d6884c570278\sh_1ad7da840001B35j1Mw2faJB9N.out]

**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline --all --author=\"Bobris560\"; git show --stat --oneline 66eafe1"
}
```

66eafe1 ue04: einrichtung.md ausgefüllt
 ue04/bobris560/einrichtung.md | 28 ++++++++++++++++++++++++++++
 1 file changed, 28 insertions(+)


---

## Assistant

_Thinking:_

The user is bobris560. Only file committed is ue04/bobris560/einrichtung.md. But maybe there are local uncommitted changes? git status showed empty. So only that file. But maybe ue02/bobris560? Let me check whether such directories exist. The branch is ue04-bobris560, only committed ue04. But earlier exercises might exist under different names? Let's check for bobris directories in ue01-ue03. Also check git status porcelains including untracked. Status was empty. Let's search.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Directory ue01,ue02,ue03,ue04 | Where-Object { $_.Name -like '*bobris*' } | Select-Object FullName; git log --oneline --format='%h %an <%ae> %s' -- ue04/bobris560; git log --oneline --format='%h %an <%ae> %s' --all -- ue04/bobris560"
}
```


66eafe1 bobris560 <kassimimohammed54@gmail.com> ue04: einrichtung.md ausgefüllt
66eafe1 bobris560 <kassimimohammed54@gmail.com> ue04: einrichtung.md ausgefüllt
FullName                                                          
--------                                                          
C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue04\bobris560




**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\kassi\\thm_wk-1208_softwaretechnik-uebungen\\ue04\\bobris560\\einrichtung.md"
}
```

Read file C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue04\bobris560\einrichtung.md, lines 1-28
1: # Einrichtung — Coding Agent
2: 
3: 
4: 
5: ## Aufbau
6: 
7: | Angabe | Ihre Angabe |
8: |---|---|
9: | Läuft der Agent? | ja |
10: | Werkzeug | opencode |
11: | Version | v2.2.5 |
12: | Betriebssystem | Windows |
13: | Modellzugang | OpenCode Zen |
14: | Modell | Big Pickle |
15: 
16: 
17: 
18: ## Antwort des Agenten geprüft
19: 
20: <!-- Aufgabe 2, Schritt 8: Vergleichen Sie die Antwort des Agenten in
21:      sitzung.md mit dem, was Sie selbst wissen. Hat er alle Ihre Dateien
22:      gefunden? Hat er etwas Fremdes für Ihres gehalten oder etwas erfunden?
23:      Zwei bis drei Sätze. -->
24: 
25: …
26: 
27: ## Wenn es nicht läuft
28: 

---

## Assistant

_Thinking:_

Note: the file includes an email in git log, but I shouldn't expose it. Answer in German.

Let me summarize repository contents by exercise. ue01 — what's in it? Need to list top-level per ue. Let me quickly get counts and contents of ue01, and READMEs maybe. Also ue04 README explains task. Let me gather concise structure: ue01 likely steckbrief.md files; ue02 notiz/phasenplan/spezifikation per person; ue03 anforderungen/kontext/zuordnung; ue04 einrichtung. Let me check ue01 structure.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem ue01 | Select-Object Name; Get-ChildItem ue01 -File | Select-Object Name; Get-ChildItem ue01 -Directory | Measure-Object | Select-Object Count; (Get-ChildItem ue02 -Directory).Count; (Get-ChildItem ue03 -Directory).Count"
}
```


Name       
----       
steckbriefe
README.md  
README.md  
           
110
96




**Tool: read**

**Input:**
```json
{
  "path": "C:\\Users\\kassi\\thm_wk-1208_softwaretechnik-uebungen\\ue04\\README.md"
}
```

Read file C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue04\README.md, lines 1-40
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

ue01 has steckbriefe directory. Let me see its count and whether user's file exists there. Probably steckbriefe/<username>.md. Search for bobris in ue01.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem ue01\\steckbriefe | Select-Object Name | Select-Object -First 10; (Get-ChildItem ue01\\steckbriefe -File).Count; Get-ChildItem ue01\\steckbriefe -Recurse | Where-Object { $_.Name -like '*bobris*' } | Select-Object FullName"
}
```


Name        
----        
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
151




---

## Assistant

_Thinking:_

Only ue04/bobris560. But question "welche Dateien stammen von mir?" — Answer based on branch and commit authorship. Only one file. Could also mention that in ue04 README two files are required, sitzung.md is missing. Also note git status clean, no uncommitted files. Should we mention that email in commit is exposed? AGENTS says nothing personal in files/commits. There's an email in git log, but I shouldn't print it, maybe note that the commit's author email is a real Gmail address and visible publicly. But user asked what's in repo. Could mention briefly as hint? The rules say don't include personal data in outputs that are to be taken over. It is already in the repo's git history, not my doing. Might mention as a note that the commit is under a different author name/email than GitHub username — actually username bobris560, commit author bobris560. That's a possible mismatch worth flagging. But careful not to expose email. I can say "Der Commit ist unter einem anderen Namen/einer anderen E-Mail-Adresse als deinem GitHub-Namen erfasst" without printing it.

Let me structure answer:

Repository: fork of THM Softwaretechnik exercises, branch ue04-bobris560, clean working tree.

Contents:
- ue01: 151 Steckbriefe in ue01/steckbriefe
- ue02: 110 person directories, each notiz.md, phasenplan.md, spezifikation.md (manche zusätzlich rollen.md), plus _vorlage, _zugabe
- ue03: 96 dirs, each anforderungen.md, kontext.md, zuordnung.md, plus _vorlage
- ue04: README, _vorlage/einrichtung.md, bobris560/einrichtung.md
- top-level README.md, AGENTS.md

Your files:
- only ue04/bobris560/einrichtung.md (new in commit 66eafe1 "ue04: einrichtung.md ausgefüllt")
- No files in ue01-ue03 under bobris560; ue02 may have earlier abbreviation? Checked no bobris dirs.
- Missing: ue04/bobris560/sitzung.md, which ue04 README requires.

Also note einrichtung.md still contains "…" placeholders in section "Antwort des Agenten geprüft" and "Wenn es nicht läuft" maybe further content. Let me read remaining lines 27-28 — file ends at 28, just "## Wenn es nicht läuft". So incomplete. Also the header has empty lines? The template maybe expected filled. Could note that sections are still blank.

Also flag author identity mismatch.

Wait — "welche Dateien stammen von mir?" Could the user be kassi? They ask in a context. The branch and directory say bobris560; commit author is bobris560. The GitHub remote is Bobris560. So user is bobris560 likely. Good.

Should I check if ue02 has an older abbreviation that belongs to user? The AGENTS says older dirs may have earlier chosen abbreviation. We only have branch info; can't know. But commit author check across all history may reveal files authored by same author. Let me run git log --all --author for the author name to see if they contributed elsewhere.

**Tool: shell**

**Input:**
```json
{
  "command": "git log --all --format='%h %ad %s' --date=short --author='bobris560'; git log --all --format='%h %ad %s' --date=short --author='Bobris560'"
}
```

66eafe1 2026-11-05 ue04: einrichtung.md ausgefüllt
c66f24d 2026-10-30 Aufgabe 3: Eigene Anforderungen
8ee84fd 2026-10-29 Aufgabe 2: Zuordnung Anforderung oder Lösung
5e544e7 2026-10-29 Aufgabe 1: Stakeholder und Systemkontext
e72a77a 2026-10-29 Steckbrief aktualisiert
1e7a628 2026-10-13 Steckbrief für moh  anlegen


---

## Assistant

_Thinking:_

There are earlier commits by the same author identity. Need to see which files touched.

**Tool: shell**

**Input:**
```json
{
  "command": "git show --stat --oneline c66f24d; git show --stat --oneline 8ee84fd; git show --stat --oneline 5e544e7; git show --stat --oneline e72a77a; git show --stat --oneline 1e7a628"
}
```

c66f24d Aufgabe 3: Eigene Anforderungen
 ue03/moh/anforderungen.md | 20 ++++++++++++++++++++
 1 file changed, 20 insertions(+)
8ee84fd Aufgabe 2: Zuordnung Anforderung oder Lösung
 ue03/moh/zuordnung.md | 37 +++++++++++++++++++++++++++++++++++++
 1 file changed, 37 insertions(+)
5e544e7 Aufgabe 1: Stakeholder und Systemkontext
 ue03/moh/kontext.md | 41 +++++++++++++++++++++++++++++++++++++++++
 1 file changed, 41 insertions(+)
e72a77a Steckbrief aktualisiert
 ue01/steckbriefe/moh.md | 14 ++++++++++++++
 1 file changed, 14 insertions(+)
1e7a628 Steckbrief für moh  anlegen
 ue01/steckbriefe/moh.md | 0
 1 file changed, 0 insertions(+), 0 deletions(-)


**Tool: shell**

**Input:**
```json
{
  "command": "git log --all --oneline --name-only --format='%h %ad %s' --date=short --author='bobris560' | Select-Object -First 80"
}
```

66eafe1 2026-11-05 ue04: einrichtung.md ausgefüllt

ue04/bobris560/einrichtung.md
c66f24d 2026-10-30 Aufgabe 3: Eigene Anforderungen

ue03/moh/anforderungen.md
8ee84fd 2026-10-29 Aufgabe 2: Zuordnung Anforderung oder Lösung

ue03/moh/zuordnung.md
5e544e7 2026-10-29 Aufgabe 1: Stakeholder und Systemkontext

ue03/moh/kontext.md
e72a77a 2026-10-29 Steckbrief aktualisiert

ue01/steckbriefe/moh.md
1e7a628 2026-10-13 Steckbrief für moh  anlegen

ue01/steckbriefe/moh.md


---

## Assistant

_Thinking:_

Interesting: earlier files under ue01/steckbriefe/moh.md and ue03/moh/*. These are probably the same person under earlier abbreviation "moh". According to AGENTS, older directories can carry an earlier chosen abbreviation and still belong to the person. So these likely belong to the user too. Need to verify ue02/moh? There's no ue02/moh directory (I saw mkon, mu, mw, my55 but no moh). Let me check. Actually ue02 list includes "mkon", "mu", "mw", "my55", no moh. So no ue02 submission.

But wait: is "moh" actually the user? The commit author identity is same as for bobris560 commit. That's a strong link. But is the author name/email the same? Yes, git log --author matched same string. So yes, likely same person. The AGENTS says older directories may use earlier abbreviation; they still belong. We can state "mit hoher Wahrscheinlichkeit" or "laut Commit-Autorschaft gehören auch ... dir". But careful about the repo being a fork: The commits e72a77a etc. may be inherited from the upstream repo? No, those files are under ue03/moh and author was bobris560. The branch ue04-bobris560 may be based on main that includes the user's earlier PRs merged. So moh = user's earlier abbreviation.

Let me check git log for ue03/moh maybe merged into main and present. Also check ue02 for any author commits with other directories under a different author name? Maybe user used another identity earlier. Let's check commit authors for files in ue02 and ue03/moh. We know moh. For ue02, search for author emails matching. Maybe the user's ue02 submission was under "moh"? There is no. Maybe user didn't do ue02. But perhaps under "mu"? Let's check authors of ue02 directories and see if any has same email. Use git log --all --format author email for ue02. Could be noisy. Let's search commits by author email domain gmail? Better: find commits by the same email across all files. `git log --all --author='kassimimohammed54@gmail.com'` already gives same five. So only moh.

But maybe the user had another email earlier. Can't know. Check user.name/user.email? Not necessary. The current one matches only moh + bobris560.

Let me verify contents of moh files to see if they reference name. Not needed. Let me confirm ue02 no moh.

Also need to mention that ue03/moh files are complete (20/37/41 lines) and ue01 steckbrief.

Let me read ue01/steckbriefe/moh.md maybe it contains personal data? We can just note. Maybe check ue03/moh files briefly for placeholders? The user asked what's there, not review. But useful to note ue04 file incomplete. Maybe check if ue03 files complete enough. Not necessary.

Let me get exact list and status cleanliness. Already know.

Potential concern: In ue04/einrichtung.md the "Antwort des Agenten geprüft" section is still "…" and "Wenn es nicht läuft" empty. The ue04 README requires sitzung.md. Mention.

Also the commit author email mismatch. Should I mention? AGENTS says commits shouldn't contain personal email? Actually README says commit name/email from Git setup are public and explains how to hide. It's allowed but the user may want to know. Not required. But the question asks which files are mine, and identifying by author is how we did it. We might note that the newer commit is authored under bobris560, not bobris560, but linked by same identity. Hmm, that exposes the name. The name is already public in git log; but AGENTS says avoid personal data in files and commit messages, not necessarily in chat. Still, better to say "unter demselben Git-Autor wie die früheren moh-Beiträge" without printing name/email. Actually I already printed it in tool output visible to user—fine, but final should avoid.

Let me verify ue02 doesn't have moh and maybe check readme ue01.

**Tool: shell**

**Input:**
```json
{
  "command": "Test-Path ue02\\moh; Get-ChildItem ue01\\steckbriefe\\moh.md | Select-Object Name,Length; Get-ChildItem ue03\\moh | Select-Object Name,Length"
}
```

False
Get-ChildItem : Der Pfad "C:\Users\bobris560\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\moh.md" kann nicht 
gefunden werden, da er nicht vorhanden ist.
In Zeile:1 Zeichen:21
+ Test-Path ue02\moh; Get-ChildItem ue01\steckbriefe\moh.md | Select-Ob ...
+                     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\bobris560\...ckbriefe\moh.md:String) [Get-ChildItem], ItemNotFound 
   Exception
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.GetChildItemCommand
 

Name             Length
----             ------
anforderungen.md    913
kontext.md         1636
zuordnung.md       1822




---

## Assistant

_Thinking:_

Interesting: ue01/steckbriefe/moh.md does not exist now, although commit e72a77a added it. Maybe it was later renamed/deleted? Let me check git log for that path and current filenames starting with moh. Maybe renamed to bobris560.md? Let's check.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem ue01\\steckbriefe | Where-Object { $_.Name -like 'moh*' -or $_.Name -like '*bobris*' -or $_.Name -like '*mohammed*' } | Select-Object Name; git log --all --oneline --name-status -- ue01/steckbriefe/moh.md; git log --all --oneline --name-status --diff-filter=DR -- ue01/steckbriefe"
}
```

e72a77a Steckbrief aktualisiert
M	ue01/steckbriefe/moh.md
1e7a628 Steckbrief für moh  anlegen
A	ue01/steckbriefe/moh.md
a5b9249 Beispiel-Steckbrief in _beispiel.md umbenennen
R100	ue01/steckbriefe/mmus.md	ue01/steckbriefe/_beispiel.md


---

## Assistant

_Thinking:_

The file was added on an older branch but not present in current main? Maybe those commits are on a branch not merged, and `--all` includes other branches. Let's check which branches contain these commits and whether the current branch has them. `git branch -a --contains e72a77a`.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch -a --contains e72a77a; git branch -a --contains 5e544e7; git branch -a --contains 66eafe1; git status -sb"
}
```

  steckbrief-moh
  ue03-moh
  remotes/origin/ue03-moh
* ue04-bobris560
  remotes/origin/ue04-bobris560
## ue04-bobris560...origin/ue04-bobris560


---

## Assistant

_Thinking:_

So e72a77a and 5e544e7 are only on branches `steckbrief-moh`, `ue03-moh`, not merged into ue04 branch. Wait, `git branch -a --contains e72a77a` output shows "steckbrief-moh", "ue03-moh", "remotes/origin/ue03-moh" then current branch line? Let's parse: output lines:
  steckbrief-moh
  ue03-moh
  remotes/origin/ue03-moh
* ue04-bobris560
  remotes/origin/ue04-bobris560

Hmm, that was combined output of three commands. Actually first command output maybe steckbrief-moh and ue03-moh and origin/ue03-moh? Then second command 5e544e7 same. Third command 66eafe1 -> ue04-bobris560 and origin/ue04-bobris560. So e72a77a is on steckbrief-moh and ue03-moh; 5e544e7 likewise; 66eafe1 on ue04-bobris560 only.

But the working tree does have ue03/moh files (committed on branch ue03-moh), yet current branch ue04-bobris560? Does current working tree include those because ue04 branched from ue03? Wait git status clean on ue04, and ue03/moh files exist in working tree and presumably tracked in current branch? Let's check `git ls-files ue03/moh`. If current branch doesn't contain 5e544e7, but files exist on disk, maybe they were merged via a different commit (cherry-pick, PR) with different commit hashes. Let's check log for ue03/moh on current branch.

**Tool: shell**

**Input:**
```json
{
  "command": "git ls-files ue03/moh; git log --oneline -- ue03/moh; git log --oneline -- ue01/steckbriefe/moh.md; git log --oneline --all -- ue03/moh"
}
```

ue03/moh/anforderungen.md
ue03/moh/kontext.md
ue03/moh/zuordnung.md
8d8cefb Übung 3: Ergebnisse von moh (#360)
8d8cefb Übung 3: Ergebnisse von moh (#360)
c66f24d Aufgabe 3: Eigene Anforderungen
8ee84fd Aufgabe 2: Zuordnung Anforderung oder Lösung
5e544e7 Aufgabe 1: Stakeholder und Systemkontext


---

## Assistant

_Thinking:_

So ue03/moh was merged via 8d8cefb (#360), with different commit. The local branch ue03-moh has original commits. And ue01/steckbriefe/moh.md — current branch? `git ls-files ue01/steckbriefe/moh.md` returned nothing (first git log for ue03/moh showed 8d8cefb twice? Let me parse output: 
- git ls-files ue03/moh: three files
- git log --oneline -- ue03/moh: 8d8cefb
- git log --oneline -- ue01/steckbriefe/moh.md: (empty?) 
- git log --oneline --all -- ue03/moh: 8d8cefb
Wait output lines:
```
ue03/moh/anforderungen.md
ue03/moh/kontext.md
ue03/moh/zuordnung.md
8d8cefb Übung 3: Ergebnisse von moh (#360)
8d8cefb Übung 3: Ergebnisse von moh (#360)
c66f24d Aufgabe 3: Eigene Anforderungen
8ee84fd Aufgabe 2: Zuordnung Anforderung oder Lösung
5e544e7 Aufgabe 1: Stakeholder und Systemkontext
```
So the third command (`git log --oneline -- ue01/steckbriefe/moh.md`) produced no output; fourth produced 8d8cefb + 5e544e7 etc? Actually `--all` for ue03/moh would include 8d8cefb, c66f24d, 8ee84fd, 5e544e7. That's 4 lines. Current branch produced one 8d8cefb. So yes, ue01/moh.md is not on current branch — the steckbrief branch wasn't merged? But maybe it was renamed to something else when merged. Let's search all history for commits by this author in current branch main. `git log --oneline --author=... --all` showed 1e7a628. But current branch doesn't contain it. Maybe the steckbrief commit wasn't merged into main, or was merged under another identity. Let's search ue01/steckbriefe for file content "moh". Also check `git branch -a --contains 1e7a628`.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch -a --contains 1e7a628; git log --oneline --all -- ue01/steckbriefe/moh.md; Get-ChildItem ue01\\steckbriefe -File | Where-Object { $_.BaseName -match 'moh' -or $_.BaseName -match 'bob' } | Select-Object Name; git log --all --oneline --author='bobris560' --name-status"
}
```

  steckbrief-moh
  remotes/origin/steckbrief-moh
e72a77a Steckbrief aktualisiert
1e7a628 Steckbrief für moh  anlegen
66eafe1 ue04: einrichtung.md ausgefüllt
A	ue04/bobris560/einrichtung.md
c66f24d Aufgabe 3: Eigene Anforderungen
A	ue03/moh/anforderungen.md
8ee84fd Aufgabe 2: Zuordnung Anforderung oder Lösung
A	ue03/moh/zuordnung.md
5e544e7 Aufgabe 1: Stakeholder und Systemkontext
A	ue03/moh/kontext.md
e72a77a Steckbrief aktualisiert
M	ue01/steckbriefe/moh.md
1e7a628 Steckbrief für moh  anlegen
A	ue01/steckbriefe/moh.md


---

## Assistant

_Thinking:_

So the steckbrief branch `steckbrief-moh` was never merged into main (maybe no PR or rejected). Therefore on the current branch, only ue04/bobris560/einrichtung.md and ue03/moh/* are present. Wait, ue03/moh was merged via PR #360, so it's part of main and current branch. So the user's files present in current checkout:

- ue03/moh/anforderungen.md, kontext.md, zuordnung.md (merged via 8d8cefb, originally authored by same person). Under AGENTS, older directory "moh" belongs.
- ue04/bobris560/einrichtung.md
- The ue01 steckbrief exists only on branch `steckbrief-moh`, not current branch/main.

But "welche Dateien stammen von mir?" might mean in the repository as a whole, including branches? Usually in the current working tree. I should answer both: in current checkout, and branches.

Need also check maybe other files in ue02 authored under another identity? The same author only has these commits. But maybe a different git identity. We can check `git log --all --format` for other authors? There are 110 ue02 submissions from many people. Without knowing, can't attribute. The branch name ue04-bobris560 and older "moh" link via same author. We should note uncertainty for moh: "Die Commits unter ue03/moh stammen vom selben Git-Autor; laut AGENTS können ältere Kürzel dazugehören – bitte bestätigen."

Wait, is "moh" definitely the same person? The author name bobris560 and GitHub bobris560. Could be two different people sharing a computer, but likely same. The AGENTS says if unclear which dirs belong, ask rather than guess. Here the evidence is strong (same Git author identity, and e72a77a also on branch steckbrief-moh). But it's possible the user opened someone else's fork? Remote is Bobris560. The local git author is bobris560. Hmm.

Also note: the commit message "Steckbrief für moh anlegen" and directory "moh" = first letters of Mohammed? Could be. Bobris560 maybe nickname. Likely same.

Maybe I should verify the current user config name/email matches commit author, without printing email. `git config user.name` etc. But already author matches.

Could also check other branches for ue02 under moh. Only steckbrief-moh, ue03-moh, ue04-bobris560. No ue02 branch.

Now, answer should be concise but informative. Include:

- Branch: ue04-bobris560 (not main), clean, remote fork.
- Structure overview with counts.
- Files attributable to user:
  1. ue04/bobris560/einrichtung.md (current branch, new)
  2. ue03/moh/{kontext.md,zuordnung.md,anforderungen.md} (current branch, via PR #360, originally from same Git author)
  3. ue01/steckbriefe/moh.md only on branch `steckbrief-moh`, not in current checkout/main.
- No ue02 submission found under bobris560/moh.
- Gaps: ue04 requires sitzung.md and einrichtung.md seems incomplete (section "Antwort des Agenten geprüft" still "…"; "Wenn es nicht läuft" empty). Maybe mention that.
- Note identity: commits are authored under a different display name than bobris560; don't print personal email.

Should I mention the ue01 branch unmerged? Yes, "nicht in main/aktuellen Branch enthalten". Maybe useful: if the steckbrief was supposed to be submitted, the PR may still be open or missing.

Could also mention that there are 151 steckbriefe, 110 ue02 dirs, 96 ue03 dirs. Actually ue02 count includes _vorlage and _zugabe, so ~108 people. ue03 count includes _vorlage, so 95 people. ue01 151 files includes maybe _beispiel. Fine, say "über 100" / "rund".

Let me verify ue02 count composition and whether user has files under another name. Could skip.

One more check: Does ue03/moh files get counted as "own" if current branch? Yes present. Let me read first lines to confirm they're filled. Not essential, but maybe check for placeholders. Also ue01 moh branch content. Let me view quickly to characterize.

**Tool: shell**

**Input:**
```json
{
  "command": "git show steckbrief-moh:ue01/steckbriefe/moh.md; Get-Content ue03\\moh\\kontext.md -TotalCount 12"
}
```

# Steckbrief moh

## Studiengang und Semester

Wirtschaftsinformatik B.Sc., 3. Semester

## Meine bisherige Erfahrung mit Softwareentwicklung

ich habe bis jetzt keine Erfahrungen außer Progammeirung

## Das erwarte ich von der Veranstaltung

Ich möchte verstehen, wie aus einer Idee ein Softwareprojekt wird.

# Stakeholder und Systemkontext �?" Terminplaner fǬr die THM


     
     

## Stakeholder


     

| Stakeholder | Worauf hat er Einfluss? |


---

## Assistant

_Thinking:_

The ue03 files have encoding issue (�?" and fǬr). That's a data quality issue. Should mention? The user asked what lies there and which files are mine. Could note encoding artifacts in ue03/moh/kontext.md maybe. But avoid overcomplicating. Maybe mention briefly as a hint.

Let me check whether all ue03/moh files have encoding issues.

**Tool: shell**

**Input:**
```json
{
  "command": "Select-String -Path ue03\\moh\\*.md -Pattern '�' | Select-Object Path,LineNumber,Line; Select-String -Path ue04\\bobris560\\einrichtung.md -Pattern '…' | Select-Object LineNumber,Line"
}
```


LineNumber Line
---------- ----
        25 .   




---

## Assistant

_Thinking:_

Select-String with '�' didn't match maybe because encoding read differently; output only second command. It shows line 25 "...". The first command output empty (the "LineNumber Line" header from second). So maybe the encoding is fine from PowerShell? Earlier Get-Content displayed �?" due to console encoding. Not necessarily file issue. Don't mention.

Now final answer in German, concise. Avoid email/name. Mention counts, structure, attribution, gaps, and offer to fix.

Let me formulate:

"Du bist auf Branch ue04-bobris560 (nicht main), Arbeitsverzeichnis ist sauber, Remote ist dein Fork Bobris560/…"

Repository contents:
- ue01: README + steckbriefe/ (~151)
- ue02: README + ~110 person dirs each notiz, phasenplan, spezifikation, teils rollen; _vorlage, _zugabe
- ue03: README + ~96 dirs each kontext, anforderungen, zuordnung; _vorlage
- ue04: README, _vorlage/einrichtung.md, bobris560/einrichtung.md
- AGENTS.md, README.md

Your files:
- ue04/bobris560/einrichtung.md, commit 66eafe1, only file in that commit.
- ue03/moh/* — same Git author, merged as #360. Flag: older abbreviation; confirm it's yours.
- ue01/steckbriefe/moh.md — exists only on branch steckbrief-moh, not merged/current.
- No ue02 submission found under bobris560 or moh.

Notes:
- ue04 requires sitzung.md missing.
- einrichtung.md incomplete: "Antwort des Agenten geprüft" still "…", "Wenn es nicht läuft" empty.
- Commit author identity is not bobris560 (but no need to show).

Question: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" Just answer. Maybe ask if they want me to fill missing things. Keep concise.

Use file paths. Mention "laut Git-Autorschaft".

Let's ensure "moh" is in current branch and assigned. Yes.

Could say "Die Dateien unter ue03/moh stammen laut Commit-Historie vom selben Git-Autor wie dein ue04-Commit. Da 'moh' ein älteres Kürzel sein kann, würde ich das als deine Dateien zählen – bestätige das bitte kurz." That follows AGENTS: ask when unclear.

The final should be in German. No personal data. Don't print the author name/email. Good.

**Stand:** Branch `ue04-bobris560` (nicht `main`), Arbeitsverzeichnis sauber, Remote ist dein Fork `Bobris560/…`.

## Was im Repository liegt

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | `README.md` und `steckbriefe/` mit rund 150 Steckbriefen |
| `ue02/` | rund 110 Personenverzeichnisse mit je `notiz.md`, `phasenplan.md`, `spezifikation.md` (teils zusätzlich `rollen.md`), dazu `_vorlage/` und `_zugabe/` |
| `ue03/` | rund 95 Personenverzeichnisse mit je `anforderungen.md`, `kontext.md`, `zuordnung.md`, dazu `_vorlage/` |
| `ue04/` | `README.md`, `_vorlage/einrichtung.md` und `bobris560/einrichtung.md` |
| Wurzel | `README.md`, `AGENTS.md` |

## Dateien, die von dir stammen

- **`ue04/bobris560/einrichtung.md`** — der einzige Inhalt deines Commits `66eafe1` („ue04: einrichtung.md ausgefüllt“).
- **`ue03/moh/kontext.md`, `zuordnung.md`, `anforderungen.md`** — laut Commit-Historie vom selben Git-Autor; eingebracht über PR #360. `moh` ist vermutlich dein früheres Kürzel — bitte kurz bestätigen, dann zähle ich sie sicher als deine.
- **`ue01/steckbriefe/moh.md`** — existiert nur auf dem Branch `steckbrief-moh`, nicht in deinem aktuellen Branch und nicht in `main`. Falls der Steckbrief eingereicht werden sollte, ist er dort noch nicht angekommen.
- Ein `ue02`-Beitrag unter `bobris560` oder `moh` ist nicht vorhanden.

## Auffälligkeiten

- In `ue04/bobris560/einrichtung.md` fehlt der Abschnitt „Antwort des Agenten geprüft“ noch (steht auf `…`), und „Wenn es nicht läuft“ ist leer.
- Die für Übung 4 ebenfalls verlangte Datei **`ue04/bobris560/sitzung.md`** fehlt.
- Die Commits laufen unter einer anderen Git-Autor-Identität als deinem GitHub-Namen `bobris560`. Das ist nicht falsch, aber gut zu wissen, weil das Repository öffentlich ist.

Soll ich die fehlenden Teile in `einrichtung.md` ergänzen oder `sitzung.md` anlegen?
