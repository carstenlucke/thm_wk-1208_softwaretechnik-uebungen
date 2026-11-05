 # Repository-Inhalt und meine Dateien

**Session ID:** ses_e571cf59dffeHz4d12sSvA6DpE
**Created:** 5.11.2026, 00:26:54
**Updated:** 5.11.2026, 00:27:30

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

Der User fragt, was in diesem Repository liegt und welche Dateien von ihm stammen. Ich muss zuerst den Branch prüfen (laut AGENTS.md), und dann das Repository erkunden.

Ich werde zuerst den aktuellen Branch prüfen und die Verzeichnisstruktur ansehen.

**Tool: shell**

**Input:**
```json
{
  "command": "git branch --show-current"
}
```

ue04-nyaornela


**Tool: shell**

**Input:**
```json
{
  "command": "ls -la"
}
```

Get-ChildItem : Es wurde kein Parameter gefunden, der dem Parameternamen "la" entspricht.
In Zeile:1 Zeichen:4
+ ls -la
+    ~~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindingException
    + FullyQualifiedErrorId : NamedParameterNotFound,Microsoft.PowerShell.Commands.GetChildItemCommand
 

Exited with code 1

---

## Assistant

_Thinking:_

Der Branch ist `ue04-nyaornela`. Also ist der Benutzername `nyaornela`. Ich bin auf einem Feature-Branch, nicht auf main, also kann ich arbeiten.

Lass mich die Verzeichnisstruktur erkunden.

**Tool: shell**

**Input:**
```json
{
  "command": "git status"
}
```

On branch ue04-nyaornela
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   ue03/nko/anforderungen.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	ue04/nyaornela/

no changes added to commit (use "git add" and/or "git commit -a")


**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Force"
}
```



    Verzeichnis: C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
d--h--        05.11.2026     00:26                .git                                                                 
d-----        04.11.2026     16:32                ue01                                                                 
d-----        04.11.2026     16:32                ue02                                                                 
d-----        04.11.2026     16:32                ue03                                                                 
d-----        04.11.2026     16:36                ue04                                                                 
-a----        04.11.2026     16:32           2208 AGENTS.md                                                            
-a----        04.11.2026     16:32           3286 README.md                                                            




---

## Assistant

_Thinking:_

Es gibt eine modifizierte Datei `ue03/nko/anforderungen.md` und ein untracked Verzeichnis `ue04/nyaornela/`. Der Branch-Name ist `ue04-nyaornela`, also der Benutzername ist `nyaornela`.

Aber laut AGENTS.md: "Geändert oder angelegt wird ausschließlich, was unter `ueNN/<benutzername>/` der Person liegt." Die modifizierte Datei `ue03/nko/anforderungen.md` liegt unter `nko`, nicht `nyaornela`. Das könnte ein Fehler sein oder eine unabsichtliche Änderung. Ich sollte das nicht einfach ändern. Lass mich zuerst die Struktur erkunden und die Dateien verstehen.

Lass mich die Verzeichnisse erkunden.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem -Recurse ue01,ue02,ue03,ue04 | Select-Object FullName,Mode,Length | Format-Table -AutoSize"
}
```

n.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\notiz.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\phasenplan.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\rollen.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\spezifikation.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\notiz.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\phasenplan.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\spezifikation.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\notiz.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\phasenplan.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\spezifikation.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\notiz.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\phasenplan.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\spezifikation.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\notiz.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\phasenplan.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\rollen.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\spezifikation.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\notiz.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\phasenplan.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\spezifikation.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82\notiz.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82\spezifikation.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\notiz.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\phasenplan.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\spezifikation.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\notiz.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\phasenplan.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\spezifikation.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\notiz.md                  
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\phasenplan.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\zsh\spezifikation.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\notiz.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\spezifikation.md     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue02\_zugabe\rollen.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\af                            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088                     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka                       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507                       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233                       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\cms                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710                      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\flk                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j                      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\janp                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\javu                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lom                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte                    
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\meq                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\MK                            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mken                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\moh                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mskk15                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mu                            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mw                            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\my55                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino                      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nko                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NN                            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\qho                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\real                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sam                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\snab                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\talh                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004                    
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\trry                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc                        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\val                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\virus                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zc                            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn                          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel                         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh                           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage                      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\README.md                     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\aayd\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\af\anforderungen.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\af\kontext.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\af\zuordnung.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\agbr\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ahyi\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\akyf\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088\anforderungen.md    
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088\kontext.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anas23088\zuordnung.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anddun\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\andel0\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anpa\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka\anforderungen.md      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka\kontext.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\anushka\zuordnung.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507\anforderungen.md      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507\kontext.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\avon507\zuordnung.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ayue\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\azm96\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bblj09\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\anforderungen.md      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\kontext.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\bogh233\zuordnung.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\cms\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\davn68\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dlm28\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710\anforderungen.md     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710\kontext.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dmmh1710\zuordnung.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\dsch\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ecib\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\emrano\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\en7-mj\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ezen\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\fahm\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\flk\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\hfdr12\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\iaa\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j\anforderungen.md     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j\kontext.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ilias04j\zuordnung.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\IY69\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\janp\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\javu\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jemy\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jsug\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\jvng\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\kraz\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lkrs\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lom\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lom\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\lom\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\Lpr\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte\anforderungen.md   
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte\kontext.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\masalabyte\zuordnung.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer\anforderun...
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer\kontext.md   
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\maxbarrosschauer\zuordnung.md 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mduc\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\meq\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\meq\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\meq\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mjab\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\MK\anforderungen.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\MK\kontext.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\MK\zuordnung.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mkon\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\moh\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\moh\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\moh\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mpal\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mskk15\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mskk15\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mu\anforderungen.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mu\kontext.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mu\zuordnung.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mw\anforderungen.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mw\kontext.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\mw\zuordnung.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\my55\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\my55\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\my55\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino\anforderungen.md     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino\kontext.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nicolino\zuordnung.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nko\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nko\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nko\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nly50\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NN\anforderungen.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NN\kontext.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NN\zuordnung.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nohl\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\NUAli\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\onzj\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\oubou\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pdam\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pgml\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\pz01\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\qho\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\qho\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\qho\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\real\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\real\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\real\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmad\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sahmed\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sam\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sam\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sam\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\skrl78\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\snab\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\snab\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\snab\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sngu\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sraks\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ssda78\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\sshj44\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\stmx\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\talh\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\talh\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\talh\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004\anforderungen.md   
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004\kontext.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\TariqK2004\zuordnung.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tcam\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tiger\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tnd\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\trry\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\trry\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\trry\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc\anforderungen.md       
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc\kontext.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\tyfncc\zuordnung.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\uwar\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\val\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\val\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\val\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\vic26\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\virus\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\virus\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\virus\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\wnga\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ygue\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\ykar\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\z-266\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zc\anforderungen.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zc\kontext.md                 
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zc\zuordnung.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn\anforderungen.md         
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn\kontext.md               
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcbn\zuordnung.md             
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\anforderungen.md        
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\kontext.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zcoel\zuordnung.md            
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\anforderungen.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\kontext.md                
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\zsh\zuordnung.md              
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\anforderungen.md     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\kontext.md           
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\nyanyaornelaa                     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage                      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\README.md                     
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\nyanyaornelaa\einrichtung.md      
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\nyanyaornelaa\sitzung.md          
C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\_vorlage\einrichtung.md       




[showing lines 571-996 of 996; full output saved to C:\Users\nyaornela\.local\share\opencode\shell\7dd341224b16cd3c90e00aa7e99ad050caef68f5\sh_1a8e3292a001dstA2YjtIn23MC.out]

---

## Assistant

_Thinking:_

Das ist eine sehr große Ausgabe. Lass mich die Struktur besser verstehen. Der Benutzername ist `nyaornela` (aus dem Branch `ue04-nyaornela`). Die Dateien, die ihm gehören, sind unter `ue04/nyaornela/`. Es gibt auch eine modifizierte Datei `ue03/nko/anforderungen.md`, die nicht zu ihm gehören würde (das ist `nko`).

Lass mich die git history und die Dateien des Users genauer ansehen. Zuerst die README.md um die Regeln zu verstehen.

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

Der Benutzername ist `nyaornela`. Die Frage ist, was in diesem Repository liegt und welche Dateien von ihm stammen. Lass mich die ue04/README.md lesen und die Dateien des Users. Auch die git log um zu sehen, was committed ist.

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

**Tool: shell**

**Input:**
```json
{
  "command": "git log --oneline -20"
}
```

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
ceafee0 Überschrift im Steckbrief auf Kürzel kürzen (#228)


**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem ue04/nyaornela; echo \"---\"; Get-ChildItem ue03/nko"
}
```



    Verzeichnis: C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue04\nyaornela


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
-a----        04.11.2026     16:32           2001 einrichtung.md                                                       
-a----        05.11.2026     00:25              0 sitzung.md                                                           
---


    Verzeichnis: C:\Users\nyaornela\S1 Wi\softwaretechnik\Workspace\thm_wk-1208_softwaretechnik-uebungen\ue03\nko


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
-a----        05.11.2026     00:25           1102 anforderungen.md                                                     
-a----        04.11.2026     16:32           2357 kontext.md                                                           
-a----        04.11.2026     16:32           1642 zuordnung.md                                                         




---

## Assistant

_Thinking:_

Die Frage ist einfach eine Informationsfrage: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" Ich soll antworten, nicht unbedingt etwas ändern.

Der Benutzername ist `nyaornela`. Dateien, die von ihm stammen: `ue04/nyaornela/einrichtung.md` und `ue04/nyaornela/sitzung.md` (leer). Plus eine modifizierte Datei `ue03/nko/anforderungen.md`, die nicht zu ihm gehört — das ist eine ungewöhnliche Änderung. Ich sollte das hinweisen.

Lass mich noch checken, ob es committete Dateien von `nyaornela` gibt in früheren Übungen. Der Branch heißt ue04-nyaornela, also nur ue04. Aber ältere Verzeichnisse können ein früher gewähltes Kürzel tragen. Lass mich suchen nach "nyaornela" in ue01, ue02, ue03.

**Tool: shell**

**Input:**
```json
{
  "command": "Get-ChildItem ue01,ue02,ue03 -Recurse -Directory | Where-Object { $_.Name -like \"*nya*\" -or $_.Name -like \"*nyaornela*\" } "
}
```

(no output)

**Tool: shell**

**Input:**
```json
{
  "command": "git log --all --oneline | grep -i nyaornela | head"
}
```

(no output)
Exited with code 1

---

## Assistant

_Thinking:_

Keine früheren Verzeichnisse mit nyaornela. Also stammen die Dateien von ihm nur in ue04/nyaornela/. Die modifizierte Datei ue03/nko/anforderungen.md gehört zu nko, nicht zu ihm — das ist eine fremde Datei, die geändert wurde (laut git status "modified"). Ich sollte das hinweisen, da es gegen die Spielregeln verstößt (nur eigene Dateien ändern).

Lass mich die einrichtung.md lesen, um den Inhalt zu verstehen, und die nko/anforderungen.md diff.

**Tool: read**

**Input:**
```json
{
  "path": "ue04/nyaornela/einrichtung.md"
}
```

Read file ue04/nyaornela/einrichtung.md, lines 1-55
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
12: | Läuft der Agent? | … |
13: | Werkzeug | … |
14: | Version | … |
15: | Betriebssystem | … |
16: | Modellzugang | … |
17: | Modell | … |
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

**Tool: shell**

**Input:**
```json
{
  "command": "git diff ue03/nko/anforderungen.md"
}
```

diff --git a/ue03/nko/anforderungen.md b/ue03/nko/anforderungen.md
index 0927d5a..92b64b9 100644
--- a/ue03/nko/anforderungen.md
+++ b/ue03/nko/anforderungen.md
@@ -4,7 +4,7 @@
 |---|---|---|---|
 | A01 | Studierende bekommen eine Bästatigungsnachricht per mail nach der Buchung. | System | FA |
 | A02 | Termine können in jeder Uhrzeit gebucht werden. | System | QA |
-| A03 | lehrenden können gebuchten Termin nicht einfach löoschen, ohne dass die Studierende eine Nachricht vorher bekommt. | studierenden | FA |
+| A03 | lehrenden können gebuchten Termin nicht einfach löoschen, ohne dass die Studierende eine Nachricht vorher bekommt. | Studierende | FA |
 | A04 | Die Software läuft nur auf den servern der THM. | Projektleitung | RB |
 | A05 | Das System musst MySQL als Datenbank verwenden.| THM | RB |
 | A06 | Alle Daten sind sicher und nach DSGVO geschützt. | Studierende | RB |


---

## Assistant

_Thinking:_

Die Frage ist eine reine Informationsfrage. Ich soll antworten, was im Repository liegt und welche Dateien vom User stammen.

Ich muss vorsichtig sein: die Datei `ue03/nko/anforderungen.md` ist modifiziert (uncommitted) und gehört nicht zum User. Laut AGENTS.md gehört das nicht zum User. Ich sollte darauf hinweisen, dass diese Änderung nicht von ihm stammt und vermutlich versehentlich oder von anderem stammt. Aber ich soll nicht ändern, es sei denn gefragt.

Die Frage: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" Ich antworte informativ.

Repository-Inhalt: Übungsverzeichnisse ue01-ue04, mit vielen Studentenverzeichnissen. README.md, AGENTS.md.

Dateien, die vom User stammen (nyaornela):
- ue04/nyaornela/einrichtung.md (noch unfertig, Platzhalter)
- ue04/nyaornela/sitzung.md (leer)
- möglicherweise ältere Verzeichnisse mit anderem Kürzel — keine gefunden.

Zusätzlich gibt es eine uncommitted Änderung in ue03/nko/anforderungen.md, die nicht vom User stammt und gegen die Spielregeln verstößt (nur eigene Dateien ändern). Ich sollte das erwähnen und fragen, ob ich sie zurücksetzen soll? Die AGENTS.md sagt: "Vorlagen ... bleiben unberührt". Die Änderung an nko/anforderungen.md ist eine fremde Datei. Ich darf sie nicht ändern, außer der User fragt. Aber ich kann darauf hinweisen.

Eigentlich die Frage ist nur "Was liegt in diesem Repository, und welche Dateien stammen von mir?" — ich antworte mit einer Übersicht.

Ich antworte auf Deutsch, klar und präzise. Ich erwähne auch den Branch und die uncommitted Änderung.

## Was in diesem Repository liegt

Das ist das **Übungsrepository der Veranstaltung Softwaretechnik** (THM, Campus Friedberg). Es enthält vier Übungsverzeichnisse:

| Verzeichnis | Übung |
|---|---|
| `ue01/` | Erste Schritte mit Git und GitHub |
| `ue02/` | Das Projektmodell am Fall |
| `ue03/` | Anforderungen an den Terminplaner |
| `ue04/` | Einen Coding Agent einrichten |

Jede Übung hat eine eigene `README.md`, die sagt, was einzureichen ist. Pro Übung gibt es ein Verzeichnis pro Studierenden (GitHub-Benutzername in Kleinbuchstaben) sowie Vorlagen (`_vorlage/`, `_zugabe/`) und die `README.md`-Dateien. Oben liegen `README.md` und `AGENTS.md`.

## Welche Dateien von Ihnen stammen

Sie arbeiten auf dem Branch `ue04-nyaornela`, Ihr GitHub-Benutzername ist **`nyaornela`**. Ich habe in `ue01/`, `ue02/` und `ue03/` keine älteren Verzeichnisse gefunden, die Ihnen gehören könnten (kein `nyaornela` und kein anderes Kürzel, das Ihnen zugeordnet wäre). Ihre eigenen Dateien liegen also unter:

- `ue04/nyaornela/einrichtung.md` — noch mit Platzhaltern (`…`), also unfertig
- `ue04/nyaornela/sitzung.md` — leer (0 Bytes)

Beide Dateien sind derzeit **nicht committed** (untracked).

## Hinweis: eine Änderung außerhalb Ihrer Dateien

In Ihrem Arbeitsverzeichnis gibt es eine uncommitted Änderung in `ue03/nko/anforderungen.md` (ein Wort von „studierenden“ auf „Studierende“ geändert). Diese Datei gehört zum Verzeichnis `nko`, also **nicht zu Ihnen**, und fällt nicht unter Ihre eigenen Dateien. Laut den Spielregeln in `AGENTS.md` sollten fremde Dateien unberührt bleiben. Ich habe diese Änderung **nicht** zurückgesetzt, da Sie das nicht angefragt haben — möchten Sie, dass ich sie wiederherstelle (`git restore ue03/nko/anforderungen.md`)?
  