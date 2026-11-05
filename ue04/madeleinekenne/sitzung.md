# Repository contents and my files

**Session ID:** ses_e53f391a0ffeKFH26e7knKmHc2
**Created:** 05/11/2026, 14:10:58
**Updated:** 05/11/2026, 14:13:30

---

## User

Was liegt in diesem Repository, und welche Dateien stammen von mir?

---

## Assistant

_Thinking:_

Der Benutzer fragt auf Deutsch: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" - also "What's in this repository, and which files are mine?"

Ich sollte das Repository erkunden. Lass mich zuerst die Git-Historie und den Status prüfen, um zu sehen, welche Dateien vom Benutzer stammen (committed vs. uncommitted, Autor).

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\" && git status && echo \"=== LOG ===\" && git log --oneline -20 && echo \"=== AUTHORS ===\" && git log --format='%an <%ae>' | sort -u"
}
```

At line:1 char:83
+ ... esktop\first-project\thm_wk-1208_softwaretechnik-uebungen" && git sta ...
+                                                                ~~
The token '&&' is not a valid statement separator in this version.
At line:1 char:97
+ ... roject\thm_wk-1208_softwaretechnik-uebungen" && git status && echo "= ...
+                                                                ~~
The token '&&' is not a valid statement separator in this version.
At line:1 char:119
+ ... twaretechnik-uebungen" && git status && echo "=== LOG ===" && git log ...
+                                                                ~~
The token '&&' is not a valid statement separator in this version.
At line:1 char:144
+ ...  git status && echo "=== LOG ===" && git log --oneline -20 && echo "= ...
+                                                                ~~
The token '&&' is not a valid statement separator in this version.
At line:1 char:170
+ ... OG ===" && git log --oneline -20 && echo "=== AUTHORS ===" && git log ...
+                                                                ~~
The token '&&' is not a valid statement separator in this version.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : InvalidEndOfLine
 

Exited with code 1

---

## Assistant

_Thinking:_

Powershell uses `;` not `&&`. Let me use `;`.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git status; echo \"=== LOG ===\"; git log --oneline -20; echo \"=== AUTHORS ===\"; git log --format='%an <%ae>' | sort -u"
}
```

On branch ue04-madeleinekenne
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	ue04/

nothing added to commit but untracked files present (use "git add" to track)
=== LOG ===
55e62bc Sauvegarde avant changement de branche
c0e72a0 Anforderungen für ue03
e0478ff Anforderungen für mken
327b99f Ue02 qdb (#269)
ab74b9d Ue02 abdu113 (#268)
dd388e0 Übung 2: Ergebnisse von iesp (#267)
3dbac37 Übung 2: Ergebnisse von jp26 (#266)
6879784 Übung 2 Ergebnisse von dsc (#265)
649eead Ue02 anushka (#264)
6afc647 Übung 2 (#263)
96d8da1 Übung 2 für uwar (#262)
788eb63 Ue02 tnd (#261)
52f252e Ue02 flk (#260)
94699c1    Übung 2 für mabl: Notiz, Phasenplan und Spezifikation (#259)
fba6eec Ue02 tariq k2004 (#257)
e7e0f51 Ue02 ysbi82 (#256)
87dd443 Ue02 sam (#254)
473aa84 Übung 2: Ergebnisse von talh (#253)
23ff2d7 Ergebnisse von Agub (#252)
99c9df8 ÜBung 2 (#251)
=== AUTHORS ===
1Lawand <lawand.omar@mnd.thm.de>
4903-quyenho <diem.quyen.isabelle.ho@mnd.thm.de>
52yuyu <younes.guerinat@mnd.thm.de>
abdu113 <absamed01@gmail.com>
addni <342348781+addni@users.noreply.github.com>
Afrem Aydin <afrem.aydin@mnd.thm.de>
ahmed-8x <algumaeliahmed@gmail.com>
Ahmet Yikit <ahmet.yikit@mnd.thm.de>
Ali-thm <aarz92@thm.de>
Anas23088 <anaselmakrini08@gmail.com>
anddun <andreas.dunst@mnd.thm.de>
andel0 <andzelo.julijan@gmail.com>
Andreas Dunst <andreas.dunst@mnd.thm.de>
AnnaLena563 <anna-lena.engel@mnd.thm.de>
Anshupandey018 <anshupandey868@gmail.com>
antoniogub03 <antonio.gubo@mnd.thm.de>
anushka677 <anushka.kannan@mnd.thm.de>
Apewithtren <vincent.bandit01@gmail.com>
Arsema Gebremichael <a.gebremichael@outlook.de>
asng24 <abhishek.singh@mnd.thm.de>
aunal6006-pixel <265140875+aunal6006-pixel@users.noreply.github.com>
AVon507 <alexander.vonbirn@mnd.thm.de>
bblj09 <belal.boulajraf@mnd.thm.de>
Bibesh kumar Mandal <167051318+Bibesh1@users.noreply.github.com>
bogh233 <344741187+bogh233@users.noreply.github.com>
Carsten Lucke <github@lucke.info>
ChaiWithRameez <rameez.dawood.ahmad@mnd.thm.de>
ChannyMonnieSunnie <channy.rauch@mnd.thm.de>
cngdbgsvvz-byte <cngdbgsvvz@privaterelay.appleid.com>
daidat123 <quoc.dat.bui@mnd.thm.de>
Daniel Schneider <daniel.schneider-2@mnd.thm.de>
Danish Ahil Tariq <ahildanish.t@gmail.com>
Davn25 <dogukan.avan@mnd.thm.de>
Dennis <dennishafner01@gmail.com>
DenoMeno03 <344766242+DenoMeno03@users.noreply.github.com>
Denzko <344692674+Denzko@users.noreply.github.com>
DLM28 <jannik.dillmann@mnd.thm.de>
dmmh1710 <dawood.mirza.muhammad@mnd.thm.de>
Doederich <125292496+Doederich@users.noreply.github.com>
Eaggapong Mueller <eaggapong.mueller@mnd.thm.de>
eliszng <elis.zengin@mnd.thm.de>
Emal Jar <emal.jar@mnd.thm.de>
EmranAliz <emran.alizada@mnd.thm.de>
EN7-MJ <344923410+EN7-MJ@users.noreply.github.com>
Erhan Kesbic <120945412+erhankesbic@users.noreply.github.com>
ErikCibis <erik.cibis@mnd.thm.de>
Falk <60698192+Falkitop@users.noreply.github.com>
farooqfrankfurt-gif <farooqfrankfurt@gmail.com>
Feyzahd <hatice.feyza.durna@mnd.thm.de>
Firas Al Mohamad <mohammad.firas.al.mohamad-2@mni.thm.de>
fortnitepro <341888466+fortnitepro67@users.noreply.github.com>
Georges0071 <wanssigeorges@gmail.com>
haitamji <haitam.jari@mnd.thm.de>
Hamsah1103 <344936668+Hamsah1103@users.noreply.github.com>
Huong Nguyen <thu.huong.nguyen-2@mnd.thm.de>
HussainButt7 <hussain.butt@mnd.thm.de>
Ilias04j <jelloli.ilias@icloud.com>
Ilkan Akcakoyun <akmarketingag@gmail.com>
Irem69 <344748387+Irem69@users.noreply.github.com>
Italo-esposto <italo.esposto@mnd.thm.de>
ivloic321 <ivan.loic.baba.sah@mnd.thm.de>
Jan Peter <49416044+IceSand296@users.noreply.github.com>
janasgr <167817584+janasgr@users.noreply.github.com>
Jan-at <jan.alt@mnd.thm.de>
Janis Nagel <254171637+c7fsqg7ywh-sketch@users.noreply.github.com>
javu11 <jasmin.vural@mnd.thm.de>
jayus04 <jayus.kotian@gmail.com>
JP26704 <joey.pflueger@mnd.thm.de>
kamyabrz <kamyab.razeghizeidi@mnd.thm.de>
kelliane16 <ange.kelliane.yimga.fopa@mnd.thm.de>
KiruTiger <kiruthiga.nesakulasingam@mnd.thm.de>
leiak24 <leon.bruzdziak@mnd.thm.de>
LemonTiger1992 <262156283+LemonTiger1992@users.noreply.github.com>
leroghost <leroghost@gmail.com>
lkrasniqi03 <leon.krasniqi@mnd.thm.de>
LorenzPrz <lorenz.przybilla@mnd.thm.de>
lswl60 <lars.seewald@mnd.thm.de>
Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
maksimum24 <maksim.batyi@mnd.thm.de>
malik55y <342533672+malik55y@users.noreply.github.com>
marroer19-hub <marroer19@gmail.com>
Marvin <168030571+nivbl10@users.noreply.github.com>
MasterHazelnut <166650295+MasterHazelnut@users.noreply.github.com>
mauritzduchardt <mauritz.duchardt@gmail.com>
mazm96 <256360296+mazm96@users.noreply.github.com>
mbgrn04 <mimouna.bougrine@mnd.thm.de>
MelissaUpietz <melissa.upietz@mnd.thm.de>
meloknc <343567290+meloknc@users.noreply.github.com>
mes-byte <amra.fehratovic@mnd.thm.de>
minosch23 <madinaw73@gmail.com>
modden <yaqub.ahmadi@mnd.thm.de>
mohamedof069 <341910315+mohamedof069@users.noreply.github.com>
MohammadKheiro <mkhr68@thm.de>
moumelogmo <210382062+moumelogmo@users.noreply.github.com>
MPAL <181457584+Max-Byte-Pixel@users.noreply.github.com>
mskk155 <mariam.sekkali@mnd.thm.de>
msonextdoor <169039317+msonextdoor@users.noreply.github.com>
Mustafa Al Qaysi <148225090+muxstii@users.noreply.github.com>
Mustafa Jasim <mustafa.jasim002@gmail.com>
Nathan <nathan.ghebretensae@mnd.thm.de>
NiaEna <344734263+NiaEna@users.noreply.github.com>
nicmar-29 <nicol.mardini@mnd.thm.de>
nil50 <344911830+nil50@users.noreply.github.com>
nilsowen <184246694+nilsowen@users.noreply.github.com>
nngwa35 <nayshawn.ngwa@mnd.thm.de>
nyaornela <ornela.dorcas.nya.kouopdo@mnd.thm.de>
offenbach0699 <altaf.tahiry@mnd.thm.de>
Orilon <orilon.nezaj@mnd.thm.de>
ouafaabouroua1-oss <ouafaa.bouroua@mnd.thm.de>
ouafaabouroua1-oss <ouafaa.bouroua1@icloud.com>
Paul Damm <paul.damm4@t-online.de>
PokerBuddie <kevin.zawistowski@mnd.thm.de>
ReemAlellan <reem.alellan@mnd.thm.de>
Saadzyane <saad.zyane@mnd.thm.de>
Sad Ahmed <sadbajwa200@gmail.com>
Sadidahmad <sadid.ahmad@mnd.thm.de>
SajanDeep99 <209100412+SajanDeep99@users.noreply.github.com>
Sam <smhs72@thm.de>
Shalin Koirala <shalin.koirala@mnd.thm.de>
sharafatmalik228-arch <sharafatmalik228@gmail.com>
Sinan M <21021968+sinanmsallem@users.noreply.github.com>
Sinan M'Sallem <21021968+sinanmsallem@users.noreply.github.com>
Skt435 <sadik.katakpaou-toure@mnd.thm.de>
sohail143-ofcity <341952904+sohail143-ofcity@users.noreply.github.com>
Sohta <341908666+sshj44@users.noreply.github.com>
sonnyn8 <sonny.nguyen@mnd.thm.de>
ssng61 <sahej.singh@mnd.thm.de>
ssni13 <shiva.saini@mnd.thm.de>
Talhakc22 <talha.kadir.cambel@mnd.thm.de>
Tarek Al Hahbare <bcsdtz8rmw@privaterelay.appleid.com>
Tariq Ahmad Khalil <tariq.ahmad.khalil@mnd.thm.de>
Tayfun <251621118+tyfnCC@users.noreply.github.com>
Terence <342191605+trys999@users.noreply.github.com>
Thien Ngan Nguyen (Jenny) <thien.ngan.nguyen@mnd.thm.de>
THM-Nos <nossair.belhaj@mnd.thm.de>
ttpr21 <tom.taepper@mnd.thm.de>
Ubaida13 <nader-ubaida.alishi@mnd.thm.de>
Umerwarraich99 <280030147+Umerwarraich99@users.noreply.github.com>
Valeria <valeria.stab@mnd.thm.de>
Viktoria <pet-grits@ya.ru>
vincrusch <vincent.ruscheinski@mnd.thm.de>
yamekk-stud <294207216+yamekk-stud@users.noreply.github.com>
yass819 <yassine.sbai@mnd.thm.de>
yazarfane <youssef.azarfane@mnd.thm.de>
Yosefhub <yosef.ibrahim@mnd.thm.de>
YunusKaradag76 <yunuskaradag469@gmail.com>
ZahraGit12 <batool.zahra.shah@mnd.thm.de>
zcoel <zeki.coel@mnd.thm.de>
Zehra Coban <zehracoban990@gmail.com>
zeufackcurtis <zeufackkasserovanoldcurtis@gmail.com>
Zidane Alfred Wandji <alfredzizou410@gmail.com>
Zohal-m <zohal.mojib@mnd.thm.de>


---

## Assistant

_Thinking:_

The user is on branch `ue04-madeleinekenne`. There are untracked files in `ue04/`. The git log shows many contributors. The user is likely "Madeleine kenne" (madeleine.ningpeye.kenne@mnd.thm.de). Let me explore the repo structure and check the untracked ue04 directory. Also check git config user.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git config user.name; git config user.email; echo \"=== TREE (top) ===\"; ls; echo \"=== ue04 ===\"; find ue04 -type f 2>/dev/null | head -50"
}
```

Madeleine kenne
madeleine.ningpeye.kenne@mnd.thm.de
=== TREE (top) ===


    Directory: C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen


Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
d-----         11/4/2026   3:45 PM                ue01                                                                 
d-----         11/4/2026   3:45 PM                ue02                                                                 
d-----         11/4/2026   3:45 PM                ue03                                                                 
d-----         11/4/2026   3:45 PM                ue04                                                                 
-a----         11/4/2026   3:45 PM           3002 README.md                                                            
=== ue04 ===
out-file : Could not find a part of the path 'C:\dev\null'.
At line:1 char:181
+ ... ="; ls; echo "=== ue04 ==="; find ue04 -type f 2>/dev/null | head -50
+                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : OpenError: (:) [Out-File], DirectoryNotFoundException
    + FullyQualifiedErrorId : FileOpenFailure,Microsoft.PowerShell.Commands.OutFileCommand
 



Exited with code 1

---

## Assistant

_Thinking:_

`find` not available. Use Get-ChildItem. Let me explore.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; Get-ChildItem -Recurse -File | Select-Object FullName | Out-String -Width 200"
}
```

softwaretechnik-uebungen\ue01\steckbriefe\asng24.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\athr.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\avon507.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Aza.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\azm96.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Bblj09.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\bima.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\bunter95.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\cms.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\davn68.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dhfn1611.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dlm28.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dmal2004.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dmmh1710.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dsc.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dsch.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\dszp.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ecib.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ekes.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\emalj.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\emrano.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\en7-mj.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ezen.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Fahm.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\flk.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\fortnitepro.md       
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\hams.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\hfdr12.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\hjri.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\HussainButt7.md      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\iaa.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\iesp.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ilias04j.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ivlbs.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\janp.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jat01.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\javu.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jemy.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jk04.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jp26.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jsug.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\jvng.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\kraz.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lebr.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lkrs.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lom.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Lpr.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lpr2.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\lswl60.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mabl.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\masalabyte.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\maxbarrosschauer.md  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mbgrn04.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mduc.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\meq.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mf23.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mjab.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\MK.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mken.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mkon.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mks24.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mnag.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mosm.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mpal.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mskk15.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mu.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\mw.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\my55.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nblh.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ngh.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nicolino.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nko.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nly50.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\NN.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\nohl.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\NUAli.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\onzj.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\oubou.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\pdam.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\peng.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\pgml.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\pz01.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\qdb.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\qho.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\real.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\renn.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sahmad.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sahmed.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sam.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sazy1.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sd99.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\shiva.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\skrl78.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\skt435.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Smu.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\snab.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sngu.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\sshj44.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\stmx.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\TariqK2004.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tcam.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\thng.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Tiger.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tnd.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tngan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\trry.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ttpr21.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\tyfncc.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\uwar.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\val.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\vic26.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\virus.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\vkab.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\yamekk.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ygue.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ykar.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\yoibr42.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\Z-266.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\ZahraGit12.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zc.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zcbn.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zcoel.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\zomj.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\_beispiel.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue01\steckbriefe\_vorlage.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\README.md                        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\aayd\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\aayd\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\aayd\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\abdu113\notiz.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\abdu113\phasenplan.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\abdu113\spezifikation.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\af\notiz.md                      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\af\phasenplan.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\af\spezifikation.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\agbr\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\agbr\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\agbr\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Agub\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Agub\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Agub\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Agub\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ahyi\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ahyi\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ahyi\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anas23088\notiz.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anas23088\phasenplan.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anas23088\rollen.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anas23088\spezifikation.md       
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anddun\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anddun\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anddun\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\andel0\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\andel0\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\andel0\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anpa\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anpa\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anpa\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anpa\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anushka\notiz.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anushka\phasenplan.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anushka\rollen.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\anushka\spezifikation.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\athr\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\athr\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\athr\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507\notiz.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507\phasenplan.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\avon507\spezifikation.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ayue\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\bblj09\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\bima\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\bima\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\bima\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\datr03\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\datr03\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\datr03\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dlm28\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710\notiz.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710\phasenplan.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dmmh1710\spezifikation.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dsc\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dsch\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\dszp\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\emrano\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\en7-mj\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ezen\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\fahm\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\flk\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\flk\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\flk\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro\notiz.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro\phasenplan.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\fortnitepro\spezifikation.md     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\hams\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\hams\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\hams\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\hfdr12\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\iaa\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\iesp\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j\notiz.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j\phasenplan.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ilias04j\spezifikation.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\IY69\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\janp\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\rollen.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\javu11\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\jp26\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\jvng\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\kraz\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\lebr\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\lom\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\lom\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\lom\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\Lpr\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mabl\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte\notiz.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte\phasenplan.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\masalabyte\spezifikation.md      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\notiz.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\phasenplan.md   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\rollen.md       
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\maxbarrosschauer\spezifikation.md
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04\notiz.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04\phasenplan.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mbgrn04\spezifikation.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mduc\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\rollen.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\meq\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mf23\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mjab\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mjas\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mk\phasenplan.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mkon\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mpal\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mu\notiz.md                      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mu\phasenplan.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mu\spezifikation.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mw\notiz.md                      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mw\phasenplan.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\mw\spezifikation.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\my55\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\my55\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\my55\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ngh\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino\notiz.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino\phasenplan.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nicolino\spezifikation.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nko\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nko\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nko\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\nly50\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\NN\notiz.md                      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\NN\phasenplan.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\NN\spezifikation.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\NUAli\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\oubou\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\pdam\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\pgml\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\rollen.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qdb\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qho\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qho\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\qho\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\real\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\real\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\renn\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\renn\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\renn\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmad\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\rollen.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sahmed\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sam\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sam\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sam\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\rollen.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\skrl78\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\skt435\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\skt435\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\snab\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\snab\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\snab\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sngu\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ssda78\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ssda78\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\sshj44\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ssng61\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ssng61\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\stmx\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\talh\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004\notiz.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004\phasenplan.md         
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\TariqK2004\spezifikation.md      
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tcam\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tiger\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd\notiz.md                     
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd\phasenplan.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tnd\spezifikation.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tngan\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\trry\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ttpr21\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\phasenplan.md             
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\rollen.md                 
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\tyfncc\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\uwar\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\vic26\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\virus\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\rollen.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\wnga\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ygue\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82\notiz.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\ysbi82\spezifikation.md          
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\notiz.md                    
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\phasenplan.md               
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\zcbn\spezifikation.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\notiz.md                   
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\phasenplan.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\zcoel\spezifikation.md           
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\notiz.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\_vorlage\spezifikation.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\_zugabe\rollen.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue03\README.md                        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\anforderungen.md            
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\kontext.md                  
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue03\mken\zuordnung.md                
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\anforderungen.md        
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue03\_vorlage\kontext.md              
C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue04\madeleinekenne\einrichtung.md    





[showing lines 22-462 of 462; full output saved to C:\Users\Ks_Store\.local\share\opencode\shell\dce9ed4a9d79ae57ba5e4caba6ff58f4a0e5f7a6\sh_1ac0ca114001Tv2YLm8jlcDP2E.out]

---

## Assistant

_Thinking:_

So the repo is a THM software engineering exercises repo. The user is "Madeleine kenne" (madeleine.ningpeye.kenne@mnd.thm.de). Their branch is ue04-madeleinekenne. Untracked: ue04/madeleinekenne/einrichtung.md.

Question: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" - What's in this repo, and which files are mine?

I need to identify which files "stammen von mir" (come from me / authored by me). Could be based on git author. Let me check git log for files authored by Madeleine. The commits: "Sauvegarde avant changement de branche", "Anforderungen für ue03", "Anforderungen für mken". Let me check which files those commits touched and author. Also the ue04 untracked file is hers (branch name). Let me also check git blame / log for mken directories.

Let me get more details: commits by Madeleine, files in those commits. Also check ue01/steckbriefe/mken.md and mken.md maybe hers. ue02 has no mken directory? Let me check. There's ue03/mken. ue04/madeleinekenne.

Let me search git log for her.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git log --all --author=\"Madeleine\" --oneline; echo \"=== name variants ===\"; git log --all --author=\"mken\" --oneline; echo \"=== madeleinekenne ===\"; git log --all --author=\"madeleinekenne\" --oneline"
}
```

55e62bc Sauvegarde avant changement de branche
c0e72a0 Anforderungen für ue03
e0478ff Anforderungen für mken
f31bcde Ajout de l'exercice ue02
2917c83 Ajout du steckbrief de mken
=== name variants ===
=== madeleinekenne ===
b05f4ee Anforderungen für mken (#326)
9407ef5 Steckbrief mken (#93)
f8353e1 Update mken.md with additional details


---

## Assistant

_Thinking:_

Let me check commit details.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; for c in 55e62bc c0e72a0 e0478ff f31bcde 2917c83 b05f4ee 9407ef5 f8353e1; do echo \"===== $c =====\"; git show --stat --oneline $c | head -20; done"
}
```

Portable shell scanner cannot analyze command: invalid-structure

---

## Assistant

_Thinking:_

The for loop with `;`? Actually error "invalid-structure". Maybe because of newlines? Let me run separate commands or use a single line. Let me just run git show for each.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git show --stat --oneline 55e62bc"
}
```

55e62bc Sauvegarde avant changement de branche
 ue03/mken/anforderungen.md | 25 +++++++++++++------------
 ue03/mken/kontext.md       |  4 +---
 ue03/mken/zuordnung.md     | 36 ++++++++++++++++++++++++++++++++++++
 3 files changed, 50 insertions(+), 15 deletions(-)


---

## Assistant

_Thinking:_

Let me check the remaining commits individually.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git show --stat --oneline c0e72a0"
}
```

c0e72a0 Anforderungen für ue03
 ue03/mken/kontext.md   | 37 +++++++++++++++++++++++++++++++++++++
 ue03/mken/zuordnung.md |  0
 2 files changed, 37 insertions(+)


---

## Assistant

_Thinking:_

Let me check e0478ff.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git show --stat --oneline e0478ff"
}
```

e0478ff Anforderungen für mken
 ue03/mken/anforderungen.md | 19 +++++++++++++++++++
 1 file changed, 19 insertions(+)


---

## Assistant

_Thinking:_

Let me check f31bcde.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git show --stat --oneline f31bcde"
}
```

f31bcde Ajout de l'exercice ue02
 ue02/notiz.md         | 26 ++++++++++++++++++++++++++
 ue02/spezifikation.md | 16 ++++++++++++++++
 2 files changed, 42 insertions(+)


---

## Assistant

_Thinking:_

Wait f31bcde "Ajout de l'exercice ue02" added ue02/notiz.md and spezifikation.md at root ue02? That seems odd - maybe an older commit. Let me check author.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git show --format='%an <%ae>%n%s' --no-patch f31bcde; echo \"---\"; git show --format='%an <%ae>%n%s' --no-patch 2917c83; echo \"---\"; git show --format='%an <%ae>%n%s' --no-patch b05f4ee; echo \"---\"; git show --format='%an <%ae>%n%s' --no-patch 9407ef5; echo \"---\"; git show --format='%an <%ae>%n%s' --no-patch f8353e1"
}
```

Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
Ajout de l'exercice ue02
---
Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
Ajout du steckbrief de mken
---
madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
Anforderungen für mken (#326)
---
madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
Steckbrief mken (#93)
---
madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
Update mken.md with additional details


---

## Assistant

_Thinking:_

So Madeleine authored several commits. Some via PRs merged into main (b05f4ee, 9407ef5, f8353e1). Let me check which files those PRs touched.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; echo \"=== b05f4ee ===\"; git show --stat --oneline b05f4ee; echo \"=== 9407ef5 ===\"; git show --stat --oneline 9407ef5; echo \"=== f8353e1 ===\"; git show --stat --oneline f8353e1"
}
```

=== b05f4ee ===
b05f4ee Anforderungen für mken (#326)
 ue03/mken/anforderungen.md | 19 +++++++++++++++++++
 ue03/mken/kontext.md       | 37 +++++++++++++++++++++++++++++++++++++
 ue03/mken/zuordnung.md     |  0
 3 files changed, 56 insertions(+)
=== 9407ef5 ===
9407ef5 Steckbrief mken (#93)
 ue01/steckbriefe/mken.md | 10 ++++++++++
 1 file changed, 10 insertions(+)
=== f8353e1 ===
f8353e1 Update mken.md with additional details
 ue01/steckbriefe/mken.md | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)


---

## Assistant

_Thinking:_

So Madeleine's files:
- ue01/steckbriefe/mken.md
- ue02? The local commit f31bcde added ue02/notiz.md and ue02/spezifikation.md at root (not in a subfolder). Wait that's weird—maybe that's an old version before restructuring. Let me check whether those files still exist. The current tree shows ue02/ has many subdirs but no root notiz.md/spezifikation.md probably. Let me check. Actually f31bcde might be an early commit on a different branch. Let me check if files exist now.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; ls ue02/notiz.md ue02/spezifikation.md 2>&1; echo \"---\"; git ls-files | grep -i \"ue02/notiz.md\\|ue02/spezifikation.md\""
}
```

ls : Cannot find path 'C:\Users\Ks_Store\Desktop\first-project\thm_wk-1208_softwaretechnik-uebungen\ue02\notiz.md' 
because it does not exist.
At line:1 char:84
+ ... echnik-uebungen"; ls ue02/notiz.md ue02/spezifikation.md 2>&1; echo " ...
+                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\Ks_Sto...n\ue02\notiz.md:String) [Get-ChildItem], ItemNotFound 
   Exception
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.GetChildItemCommand
 
---
grep : The term 'grep' is not recognized as the name of a cmdlet, function, script file, or operable program. Check 
the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:156
+ ... d ue02/spezifikation.md 2>&1; echo "---"; git ls-files | grep -i "ue0 ...
+                                                              ~~~~
    + CategoryInfo          : ObjectNotFound: (grep:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
 

Exited with code 1

---

## Assistant

_Thinking:_

grep not available. Use Select-String. Let me check git ls-files for those.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git ls-files | Select-String \"ue02/notiz.md|ue02/spezifikation.md\""
}
```

(no output)

---

## Assistant

_Thinking:_

So those root ue02 files no longer exist (probably deleted in later restructure). The current files from Madeleine:
- ue01/steckbriefe/mken.md
- ue03/mken/* (anforderungen.md, kontext.md, zuordnung.md)
- ue04/madeleinekenne/einrichtung.md (untracked, on her branch)

Also possibly ue02/mken? Let me check if there's a ue02/mken directory. The list didn't show mken in ue02. Let me search.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git ls-files | Select-String \"mken\""
}
```


ue01/steckbriefe/mken.md
ue03/mken/anforderungen.md
ue03/mken/kontext.md
ue03/mken/zuordnung.md




---

## Assistant

_Thinking:_

So only those tracked files plus untracked ue04. Let me also check if there's a ue02 directory for mken maybe named differently? The user asked "welche Dateien stammen von mir?" Could mean authored by them. Let me be thorough: check git log --all --author for their email to find all commits, then files. Already did. Also there might be files where they are co-author. Let me check commits with their email in body.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git log --all --format='%H %an <%ae>' | Select-String \"madeleine.ningpeye.kenne\""
}
```


55e62bc066560f07d6ba163fd318b7b45f9ad4ca Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
b05f4eebae14bf2cf8f546a0cefd5a815b2a0f70 madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
c0e72a00d19b3d8461b82deeda166257c401bad2 Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
e0478ff399127c8c01f2019581c9cf864c6f41d1 Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
f31bcde3a4d57b629a30bb258bac0b2da9f7c207 Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>
9407ef5a9b9aa03246e6b7fd04a2062e6651ae99 madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
f8353e14495fe8a2d16fbd78a7cb1c3e4ce32382 madeleinekenne <madeleine.ningpeye.kenne@mnd.thm.de>
2917c831e733bb7356021f98bae8b7a30c7e855e Madeleine kenne <madeleine.ningpeye.kenne@mnd.thm.de>




---

## Assistant

_Thinking:_

Let me also check commits where she might be co-author in message. Search git log --all -S or grep co-authored. Quick.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git log --all --format='%H %s' | Select-String \"Co-authored-by.*madeleine|madeleine.*Co-authored\" "
}
```

(no output)

---

## Assistant

_Thinking:_

No co-authors. Now the user asked "Was liegt in diesem Repository, und welche Dateien stammen von mir?" So answer: repo is a THM software engineering exercises collection (ue01..ue04). Files authored by her: list. Also there's untracked ue04/madeleinekenne/einrichtung.md.

Let me read README.md and the ue04 file to give context. Also maybe inspect ue03/mken files. Let me read README.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; Get-Content README.md"
}
```

# Softwaretechnik �?" �obungsrepository

Dieses Repository geh��rt zu den �obungen der Veranstaltung **Softwaretechnik**
(THM, Campus Friedberg, Fachbereich MND). Hier reichen Sie ein, was in den
�obungen entsteht �?" auf dem Weg, auf dem in Softwareprojekten gearbeitet wird:
Ǭber einen eigenen Fork, einen Branch und einen Pull Request.

## Aufbau

Jede �obung hat ein eigenes Verzeichnis mit einer eigenen `README.md`, die
sagt, was dort einzureichen ist.

| Verzeichnis | �obung |
|---|---|
| [`ue01/`](ue01/) | Erste Schritte mit Git und GitHub |
| [`ue02/`](ue02/) | Das Projektmodell am Fall |
| [`ue03/`](ue03/) | Anforderungen an den Terminplaner |

## So reichen Sie etwas ein

1. Legen Sie einmalig einen **Fork** dieses Repositorys an und **klonen** Sie
   ihn auf Ihren Rechner.
2. Legen Sie fǬr jedes Vorhaben einen eigenen **Branch** an.
3. Halten Sie Ihre �"nderungen als **Commits** fest und Ǭbertragen Sie sie per
   **Push** in Ihren Fork.
4. Stellen Sie einen **Pull Request** an dieses Repository.

Den Weg Schritt fǬr Schritt beschreibt das
[�obungsblatt zur �obung 1](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/).

## Vor jeder weiteren �obung

Dieses Repository w��chst mit jeder �obung. Bringen Sie vorher Ihren Fork und
Ihren Rechner auf den neuen Stand:

1. Klicken Sie auf der Startseite Ihres Forks auf **Sync fork ��' Update
   branch**.
2. Holen Sie den neuen Stand aus dem Fork auf Ihren Rechner:

   ```console
   $ git switch main
   $ git pull
   ```

Den Branch fǬr die neue �obung zweigen Sie erst danach ab.

## Spielregeln

- **KǬrzel statt Klarname.** Dieses Repository ist ��ffentlich. W��hlen Sie ein
  KǬrzel, das Sie selbst wiedererkennen, und behalten Sie es Ǭber alle
  �obungen bei. Es wird Teil von Datei- und Branchnamen: nur Kleinbuchstaben
  und Ziffern, keine Umlaute, keine Leerzeichen. Liegt unter
  `ue01/steckbriefe/` schon eine Datei mit Ihrem KǬrzel, h��ngen Sie eine
  Ziffer an.
- **�-ffentlich ist mehr als das KǬrzel.** Am Pull Request steht Ihr
  GitHub-Benutzername, in jedem Commit stehen Name und E-Mail-Adresse aus
  Ihrer Git-Einrichtung. Wie Sie Ihre Adresse verbergen, steht in
  [Aufgabe 0 des �obungsblatts](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/#aufgabe-0--einrichten). Schreiben Sie auch in Ihre Dateien nichts, was nicht
  jeder lesen darf �?" keine Matrikelnummer, keine Anschrift.
- **Nur eigene Dateien.** Sie ��ndern ausschlie�Ylich, was Sie selbst angelegt
  haben; Vorlagen und die Dateien anderer bleiben unberǬhrt. So kommen sich
  die Pull Requests nicht in die Quere.
- **Nicht auf `main` arbeiten.** `main` Ihres Forks folgt allein dem Stand
  dieses Repositorys; nur so l��sst er sich sp��ter abgleichen.
- **Ein Anliegen je Pull Request**, mit einem Titel, der sagt, was sich
  ��ndert.
- **Aussagekr��ftige Commit-Nachrichten**, etwa `Steckbrief fǬr mmus anlegen`.


---

## Assistant

_Thinking:_

README mentions ue01, ue02, ue03. But repo has ue04 too (untracked/new). Let me check ue04 README? There is ue04/madeleinekenne/einrichtung.md. Let me read it. Also check ue03 README and ue02. The user might want an overview. Let me provide concise answer.

Let me read the ue04 file.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; Get-Content ue04\\madeleinekenne\\einrichtung.md"
}
```

# Einrichtung �?" Coding Agent

<!-- Aufgaben 1 und 2 des �obungsblatts. Ersetzen Sie jedes �?z�?݃?o durch Ihre
     Angabe; die �oberschriften bleiben stehen. L��schen Sie die Kommentare,
     sobald Sie fertig sind. Die Sitzung mit dem Agenten geh��rt nicht
     hierher, sondern als Export in die Datei sitzung.md daneben. -->

## Aufbau

| Angabe | Ihre Angabe |
|---|---|
| L��uft der Agent? | �?� |
| Werkzeug | �?� |
| Version | �?� |
| Betriebssystem | �?� |
| Modellzugang | �?� |
| Modell | �?� |

<!-- L��uft der Agent?: ja, teilweise oder nein. Teilweise hei�Yt, er
     startet, aber ein Schritt danach scheitert (Anmeldung, Antwort,
     Export). Bei teilweise und nein belegen Sie unten unter �?zWenn es nicht
     l��uft�?o, woran es scheitert; ohne laufenden Agenten entf��llt sitzung.md.
     Werkzeug: opencode, oder wer schon damit arbeitet, Claude Code, Codex,
     GitHub Copilot (in VS Code oder als Copilot CLI) oder ein anderer
     Agent. Version: Ausgabe von `opencode --version` bzw.
     die Versionsangabe Ihres Werkzeugs.
     Betriebssystem: macOS, Windows, Windows mit WSL oder Linux.
     Modellzugang: GitHub Copilot, ChatGPT, OpenCode Zen (kostenlos), Claude
     oder ein anderer. Modell: so, wie es in der Auswahl hei�Yt, in opencode
     unter /models. -->

## Antwort des Agenten geprǬft

<!-- Aufgabe 2, Schritt 8: Vergleichen Sie die Antwort des Agenten in
     sitzung.md mit dem, was Sie selbst wissen. Hat er alle Ihre Dateien
     gefunden? Hat er etwas Fremdes fǬr Ihres gehalten oder etwas erfunden?
     Zwei bis drei S��tze. -->

�?�

## Wenn es nicht l��uft

<!-- Pflicht bei �?zteilweise�?o und �?znein�?o; bei �?zja�?o l��schen Sie alles unter
     der �oberschrift. In den Kasten geh��rt der Befehl, der scheitert, samt
     seiner Ausgabe, w��rtlich aus dem Terminal kopiert. -->

**Schritt, an dem es scheitert:** �?�

**Befehl und Ausgabe:**

```text
�?�
```

**Bereits versucht:** �?�


---

## Assistant

_Thinking:_

So ue04 is "Coding Agent" exercise. The user's file is untracked (not yet committed). 

Now I should answer the user's question. The question: "Was liegt in diesem Repository, und welche Dateien stammen von mir?" They might be testing the agent (Aufgabe 2 step 8: compare agent's answer with what they know). So I should be accurate and not invent. Let me be precise.

Repository overview:
- THM Softwaretechnik exercise repo.
- Directories: ue01 (Git/GitHub first steps), ue02 (project model), ue03 (requirements for scheduler), ue04 (coding agent setup) — ue04 not in README yet but exists.
- README.md at root.
- Many student submissions in subfolders by Kürzel.

Files authored by Madeleine (mken / madeleinekenne):
Tracked:
- ue01/steckbriefe/mken.md
- ue03/mken/anforderungen.md
- ue03/mken/kontext.md
- ue03/mken/zuordnung.md
Untracked (on branch ue04-madeleinekenne):
- ue04/madeleinekenne/einrichtung.md

Note: early commit f31bcde added ue02/notiz.md and ue02/spezifikation.md but those no longer exist in current tree (probably removed/restructured). Should I mention? The user asked "welche Dateien stammen von mir?" Could include historical. But to avoid confusion, mention current files and note that an earlier commit added ue02 files that no longer exist. Actually let me verify whether those files were deleted or moved. Let me check git log for those paths.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git log --all --oneline -- \"ue02/notiz.md\" \"ue02/spezifikation.md\""
}
```

f31bcde Ajout de l'exercice ue02


---

## Assistant

_Thinking:_

Only one commit added them; never deleted in history? Maybe they were on a branch that got rebased. Since current main doesn't have them. Let me check if f31bcde is ancestor of current HEAD.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git merge-base --is-ancestor f31bcde HEAD && echo \"ancestor of HEAD\" || echo \"NOT ancestor of HEAD\"; git branch -a --contains f31bcde"
}
```

At line:1 char:126
+ ... chnik-uebungen"; git merge-base --is-ancestor f31bcde HEAD && echo "a ...
+                                                                ~~
The token '&&' is not a valid statement separator in this version.
At line:1 char:153
+ ... base --is-ancestor f31bcde HEAD && echo "ancestor of HEAD" || echo "N ...
+                                                                ~~
The token '||' is not a valid statement separator in this version.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : InvalidEndOfLine
 

Exited with code 1

---

## Assistant

_Thinking:_

Powershell needs `;` and if. Let me run.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git merge-base --is-ancestor f31bcde HEAD; echo \"exit: $?\""
}
```

exit: False


---

## Assistant

_Thinking:_

f31bcde is not ancestor of HEAD. So those files are on another branch maybe. Let me check branches containing it.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git branch -a --contains f31bcde"
}
```

  ue02mken


---

## Assistant

_Thinking:_

So there's a branch ue02mken containing those files. The current branch is ue04-madeleinekenne. The user might have multiple branches. Let me check all branches.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git branch -a"
}
```

  main
  steckbrief-mken
  ue02mken
  ue03-mken
* ue04-madeleinekenne
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/steckbrief-mken
  remotes/origin/ue03-mken


---

## Assistant

_Thinking:_

There are branches: steckbrief-mken, ue02mken, ue03-mken, ue04-madeleinekenne. Each contains her work for different exercises. Let me check what files are on each branch (vs main). The user's files "stammen von mir" across all branches. Let me inspect each branch's diff from main or files.

Let me list files unique to each branch. Use git diff --name-status main..branch.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; foreach ($b in \"steckbrief-mken\",\"ue02mken\",\"ue03-mken\",\"ue04-madeleinekenne\") { echo \"===== $b =====\"; git diff --name-status main..$b }"
}
```

n.md
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
D	ue03/agbr/zuordnung.md
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
D	ue03/mskk15/anforderungen.md
D	ue03/mskk15/kontext.md
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
===== ue02mken =====
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
R095	ue02/_vorlage/notiz.md	ue02/notiz.md
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
R099	ue02/dmmh1710/spezifikation.md	ue02/spezifikation.md
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
D	ue03/agbr/zuordnung.md
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
D	ue03/mskk15/anforderungen.md
D	ue03/mskk15/kontext.md
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
===== ue03-mken =====
D	AGENTS.md
M	README.md
M	ue01/README.md
D	ue01/steckbriefe/IY69.md
M	ue01/steckbriefe/_beispiel.md
M	ue01/steckbriefe/_vorlage.md
D	ue01/steckbriefe/datr03.md
D	ue01/steckbriefe/div.md
M	ue01/steckbriefe/dmmh1710.md
D	ue01/steckbriefe/fpz.md
M	ue01/steckbriefe/kraz.md
D	ue01/steckbriefe/mjas.md
M	ue01/steckbriefe/nko.md
M	ue01/steckbriefe/pz01.md
D	ue01/steckbriefe/slr63.md
D	ue01/steckbriefe/ssng61.md
D	ue01/steckbriefe/uk.md
D	ue01/steckbriefe/wnga.md
D	ue01/steckbriefe/ysbi82.md
M	ue02/README.md
D	ue02/akyf/notiz.md
D	ue02/akyf/phasenplan.md
D	ue02/akyf/spezifikation.md
D	ue02/div/notiz.md
D	ue02/div/phasenplan.md
D	ue02/div/rollen.md
D	ue02/div/spezifikation.md
D	ue02/ivlbs/notiz.md
D	ue02/ivlbs/phasenplan.md
D	ue02/ivlbs/spezifikation.md
D	ue02/jemy/notiz.md
D	ue02/jemy/phasenplan.md
D	ue02/jemy/rollen.md
D	ue02/jemy/spezifikation.md
D	ue02/jsug/notiz.md
D	ue02/jsug/phasenplan.md
D	ue02/jsug/spezifikation.md
M	ue02/lom/notiz.md
M	ue02/ngh/phasenplan.md
M	ue02/ngh/spezifikation.md
D	ue02/nohl/notiz.md
D	ue02/nohl/phasenplan.md
D	ue02/nohl/spezifikation.md
D	ue02/pz01/notiz.md
D	ue02/pz01/phasenplan.md
D	ue02/pz01/spezifikation.md
D	ue02/real/phasenplan.md
M	ue02/sngu/phasenplan.md
D	ue02/thm-nos/notiz.md
D	ue02/thm-nos/phasenplan.md
D	ue02/thm-nos/spezifikation.md
D	ue02/thng/notiz.md
D	ue02/thng/phasenplan.md
D	ue02/thng/spezifikation.md
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
M	ue03/README.md
D	ue03/TariqK2004/anforderungen.md
D	ue03/TariqK2004/kontext.md
D	ue03/TariqK2004/zuordnung.md
D	ue03/aayd/anforderungen.md
D	ue03/aayd/kontext.md
D	ue03/aayd/zuordnung.md
D	ue03/af/anforderungen.md
D	ue03/af/kontext.md
D	ue03/af/zuordnung.md
D	ue03/agbr/anforderungen.md
D	ue03/agbr/kontext.md
D	ue03/agbr/zuordnung.md
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
D	ue03/mkon/anforderungen.md
D	ue03/mkon/kontext.md
D	ue03/mkon/zuordnung.md
D	ue03/moh/anforderungen.md
D	ue03/moh/kontext.md
D	ue03/moh/zuordnung.md
D	ue03/mpal/anforderungen.md
D	ue03/mpal/kontext.md
D	ue03/mpal/zuordnung.md
D	ue03/mskk15/anforderungen.md
D	ue03/mskk15/kontext.md
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
===== ue04-madeleinekenne =====
D	AGENTS.md
M	README.md
M	ue01/README.md
D	ue01/steckbriefe/IY69.md
M	ue01/steckbriefe/_beispiel.md
M	ue01/steckbriefe/_vorlage.md
D	ue01/steckbriefe/datr03.md
D	ue01/steckbriefe/div.md
M	ue01/steckbriefe/dmmh1710.md
D	ue01/steckbriefe/fpz.md
M	ue01/steckbriefe/kraz.md
D	ue01/steckbriefe/mjas.md
M	ue01/steckbriefe/nko.md
M	ue01/steckbriefe/pz01.md
D	ue01/steckbriefe/slr63.md
D	ue01/steckbriefe/ssng61.md
D	ue01/steckbriefe/uk.md
D	ue01/steckbriefe/wnga.md
D	ue01/steckbriefe/ysbi82.md
M	ue02/README.md
D	ue02/akyf/notiz.md
D	ue02/akyf/phasenplan.md
D	ue02/akyf/spezifikation.md
D	ue02/div/notiz.md
D	ue02/div/phasenplan.md
D	ue02/div/rollen.md
D	ue02/div/spezifikation.md
D	ue02/ivlbs/notiz.md
D	ue02/ivlbs/phasenplan.md
D	ue02/ivlbs/spezifikation.md
D	ue02/jemy/notiz.md
D	ue02/jemy/phasenplan.md
D	ue02/jemy/rollen.md
D	ue02/jemy/spezifikation.md
D	ue02/jsug/notiz.md
D	ue02/jsug/phasenplan.md
D	ue02/jsug/spezifikation.md
M	ue02/lom/notiz.md
M	ue02/ngh/phasenplan.md
M	ue02/ngh/spezifikation.md
D	ue02/nohl/notiz.md
D	ue02/nohl/phasenplan.md
D	ue02/nohl/spezifikation.md
D	ue02/pz01/notiz.md
D	ue02/pz01/phasenplan.md
D	ue02/pz01/spezifikation.md
D	ue02/real/phasenplan.md
M	ue02/sngu/phasenplan.md
D	ue02/thm-nos/notiz.md
D	ue02/thm-nos/phasenplan.md
D	ue02/thm-nos/spezifikation.md
D	ue02/thng/notiz.md
D	ue02/thng/phasenplan.md
D	ue02/thng/spezifikation.md
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
M	ue03/README.md
D	ue03/TariqK2004/anforderungen.md
D	ue03/TariqK2004/kontext.md
D	ue03/TariqK2004/zuordnung.md
D	ue03/aayd/anforderungen.md
D	ue03/aayd/kontext.md
D	ue03/aayd/zuordnung.md
D	ue03/af/anforderungen.md
D	ue03/af/kontext.md
D	ue03/af/zuordnung.md
D	ue03/agbr/anforderungen.md
D	ue03/agbr/kontext.md
D	ue03/agbr/zuordnung.md
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
M	ue03/mken/anforderungen.md
M	ue03/mken/kontext.md
M	ue03/mken/zuordnung.md
D	ue03/mkon/anforderungen.md
D	ue03/mkon/kontext.md
D	ue03/mkon/zuordnung.md
D	ue03/moh/anforderungen.md
D	ue03/moh/kontext.md
D	ue03/moh/zuordnung.md
D	ue03/mpal/anforderungen.md
D	ue03/mpal/kontext.md
D	ue03/mpal/zuordnung.md
D	ue03/mskk15/anforderungen.md
D	ue03/mskk15/kontext.md
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


[showing lines 300-2250 of 2250; full output saved to C:\Users\Ks_Store\.local\share\opencode\shell\dce9ed4a9d79ae57ba5e4caba6ff58f4a0e5f7a6\sh_1ac0dd63c001C1s5jXK6gDogXp.out]

---

## Assistant

_Thinking:_

The diff main..branch shows tons of deletions because main has all students' files, and branch only keeps mken's? Actually the branch was created by deleting others? The diff is huge. This is confusing. The branches are likely "sparse" forks where only her files remain? Actually no—branch ue04-madeleinekenne diff shows D (deleted) for almost all other students' files, and M for mken files. That means relative to main, the branch deleted everyone else's files and modified mken's. That's weird for a PR (would delete all). But maybe these branches are "personal" snapshots where she kept only her files? Or maybe the diff direction is wrong? main..branch means changes to go from main to branch. If branch has fewer files, they show as D.

But the actual current working tree (ue04-madeleinekenne checked out) has ALL files (ue01, ue02, ue03 with all students). Wait earlier Get-ChildItem showed all students' files present. So the working tree has everything. But git diff main..branch says branch deleted them? That contradicts. Let me check: maybe main is ahead of branch? Actually branch might be behind main (older main) and main added all those files later. So diff main..branch shows files that exist in main but not in branch (because branch is older), i.e., D. So branches are older snapshots. The branch's actual added files (A) relative to its base would be mken's. Let me instead find merge-base and diff from merge-base.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; foreach ($b in \"steckbrief-mken\",\"ue02mken\",\"ue03-mken\",\"ue04-madeleinekenne\") { echo \"===== $b =====\"; $mb = git merge-base main $b; echo \"merge-base: $mb\"; git diff --name-status $mb..$b }"
}
```

===== steckbrief-mken =====
merge-base: b2fa46875fb3dfeb54edda7c04dab6c499d0586b
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path> [<pathspec>...]

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.
  -B            detect complete rewrites.
  -M            detect renames.
  -C            detect copies.
  --find-copies-harder
                try unchanged files as candidate for copy detection.
  -l<n>         limit rename attempts up to <n> paths.
  -O<file>      reorder diffs according to the <file>.
  -S<string>    find filepair whose only one side contains the string.
  --pickaxe-all
                show all files diff when -S is used and hit is found.
  -a  --text    treat all files as text.

===== ue02mken =====
merge-base: b2fa46875fb3dfeb54edda7c04dab6c499d0586b
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path> [<pathspec>...]

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.
  -B            detect complete rewrites.
  -M            detect renames.
  -C            detect copies.
  --find-copies-harder
                try unchanged files as candidate for copy detection.
  -l<n>         limit rename attempts up to <n> paths.
  -O<file>      reorder diffs according to the <file>.
  -S<string>    find filepair whose only one side contains the string.
  --pickaxe-all
                show all files diff when -S is used and hit is found.
  -a  --text    treat all files as text.

===== ue03-mken =====
merge-base: 327b99f21f0bb37a03bded83b383aae07b844774
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path> [<pathspec>...]

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.
  -B            detect complete rewrites.
  -M            detect renames.
  -C            detect copies.
  --find-copies-harder
                try unchanged files as candidate for copy detection.
  -l<n>         limit rename attempts up to <n> paths.
  -O<file>      reorder diffs according to the <file>.
  -S<string>    find filepair whose only one side contains the string.
  --pickaxe-all
                show all files diff when -S is used and hit is found.
  -a  --text    treat all files as text.

===== ue04-madeleinekenne =====
merge-base: 327b99f21f0bb37a03bded83b383aae07b844774
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path> [<pathspec>...]

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.
  -B            detect complete rewrites.
  -M            detect renames.
  -C            detect copies.
  --find-copies-harder
                try unchanged files as candidate for copy detection.
  -l<n>         limit rename attempts up to <n> paths.
  -O<file>      reorder diffs according to the <file>.
  -S<string>    find filepair whose only one side contains the string.
  --pickaxe-all
                show all files diff when -S is used and hit is found.
  -a  --text    treat all files as text.


Exited with code 1

---

## Assistant

_Thinking:_

The variable $mb contains spaces? Actually error "usage: git diff" suggests $mb empty or command malformed. The foreach in powershell with $mb assignment and git diff $mb..$b — maybe $mb has trailing newline? Actually output shows merge-base hash then usage. The git diff command probably failed because $mb..$b syntax? Should be fine. But maybe $mb is empty due to variable scope? It printed merge-base. Wait the usage appears; maybe git diff requires two commits separated by space not ..? No, .. works. Let me check: maybe $mb contains CRLF? Let me use git diff "$mb" "$b" instead. Or use git diff $mb $b. Let me just run for one branch.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; $mb = \"b2fa46875fb3dfeb54edda7c04dab6c499d0586b\"; git diff --name-status $mb $b 2>&1 | Select-Object -First 5; echo \"---try two-dot---\"; git diff --name-status \"$mb..steckbrief-mken\" 2>&1 | Select-Object -First 5"
}
```

M	README.md
M	ue01/README.md
A	ue01/steckbriefe/AF.md
A	ue01/steckbriefe/AR.md
A	ue01/steckbriefe/Agub.md
---try two-dot---
A	ue01/steckbriefe/mken.md


---

## Assistant

_Thinking:_

Ah, using "$mb..branch" two-dot shows only commits unique to branch? Actually two-dot symmetric-ish? It showed only mken.md added. Wait first command `git diff $mb $b` (space) showed all files added (huge list because branch has all files? No—space diff compares trees, shows A for files present in branch but not base). The two-dot "$mb..branch" maybe means commits reachable from branch not mb, and diff of those commits? It showed only mken.md. Hmm.

Actually for identifying "files authored by me", the PRs merged into main already added mken's files to main. The branches are working branches. The user likely only cares about current checkout and git history. Let me not overcomplicate.

The cleanest answer: files that are hers (authored by Madeleine kenne / mken / madeleinekenne):
- ue01/steckbriefe/mken.md
- ue02/mken/*? Wait is there ue02/mken? Earlier git ls-files | Select-String mken showed only ue01 and ue03. So no ue02/mken in main. But branch ue02mken added ue02/notiz.md and ue02/spezifikation.md (renamed from _vorlage) plus maybe her own folder? Let me check the ue02mken branch's added files (A) relative to merge-base, filtering for "mken" or non-D. Actually the branch diff showed R095/R099 renames to ue02/notiz.md and ue02/spezifikation.md (root), meaning she worked at root ue02, not a personal folder. That's an older pattern. But those commits (f31bcde) added root files that are not in current main. Were they merged? f31bcde is not ancestor of HEAD (we checked). So her ue02 work was never merged into main? Or merged differently. Let me check if origin has ue02mken branch. git branch -a showed remotes/origin/steckbrief-mken and ue03-mken, but NOT ue02mken or ue04-madeleinekenne. So those branches are local only.

Thus "files that stem from me" in the current repository state (main + local branches + untracked):
- On main (merged PRs): ue01/steckbriefe/mken.md, ue03/mken/{anforderungen,kontext,zuordnung}.md
- Local branch ue02mken: ue02/notiz.md, ue02/spezifikation.md (and maybe root changes) — but not merged.
- Local branch ue04-madeleinekenne: ue04/madeleinekenne/einrichtung.md (untracked) plus modified mken files.

The user probably just wants to know in the current repo. The current checked-out branch is ue04-madeleinekenne. The working tree has all files. The untracked file is hers. Let me answer based on current state plus git authorship.

I think a good answer:
1. Repo overview: THM Softwaretechnik exercises, folders ue01-ue04, each student submits in own Kürzel folder; README explains workflow.
2. Her files: 
   - ue01/steckbriefe/mken.md (Steckbrief)
   - ue03/mken/anforderungen.md, kontext.md, zuordnung.md
   - ue04/madeleinekenne/einrichtung.md (new, untracked, on current branch)
   - Possibly ue02 work on branch ue02mken: ue02/notiz.md, ue02/spezifikation.md (not merged into main)
3. Note git config identifies her as Madeleine kenne.

Also mention that many other files belong to other students; she should not modify those.

I should be careful not to overstate. Let me verify ue02 branch's actual unique added file names. Use git diff b2fa468...ue02mken --name-status and filter A/R. Actually simpler: git ls-tree of branch for mken-ish. But root files not clearly hers. Let me check the commit f31bcde diff names (we saw notiz.md, spezifikation.md at ue02 root). And branch ue02mken also has those via rename. So yes.

Let me also check steckbrief-mken branch added file.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; echo \"=== steckbrief-mken added (A) ===\"; git diff --name-status b2fa46875fb3dfeb54edda7c04dab6c499d0586b steckbrief-mken | Select-String \"^A\"; echo \"=== ue02mken added (A/R) ===\"; git diff --name-status b2fa46875fb3dfeb54edda7c04dab6c499d0586b ue02mken | Select-String \"^[AR]\" | Select-String \"mken|notiz.md|spezifikation.md\""
}
```

=== steckbrief-mken added (A) ===

A	ue01/steckbriefe/mken.md
=== ue02mken added (A/R) ===
A	ue02/notiz.md
A	ue02/spezifikation.md




---

## Assistant

_Thinking:_

So steckbrief-mken added ue01/steckbriefe/mken.md. ue02mken added ue02/notiz.md, spezifikation.md. ue03-mken and ue04 branches modified ue03/mken files and added untracked ue04 file.

Now I have enough. Let me craft final answer in German, concise but complete. Include note about untracked file. Also mention git identity. Ensure no false claims.

Let me also double check current branch's modified tracked files: ue03/mken/* modified (M) in ue04-madeleinekenne relative to base. And README modified. Those modifications are hers (on her branch) but may not be intended. Should I mention? The user asked which files stem from her. The modified README etc. are probably accidental or base changes. Hmm. Actually the branch diff showed M README.md, M ue01/README.md, M ue02/README.md, M ue03/README.md, and M ue02/lom/notiz.md etc. and M ue03/mken/*. That seems like the branch contains unrelated modifications to other students' files? That would violate "Nur eigene Dateien." But maybe these M are due to merge-base being older and main having changes; diff base..branch compares branch tree to old base, and branch may have kept old versions while main updated them, resulting in M? Wait if base is ancestor of both, branch's version vs base: if branch didn't change a file, it should match base (no M). M means branch changed it relative to base. So ue04 branch did modify README and lom/notiz etc.? That's suspicious. But maybe the "M" are actually because branch is based on an older main where those files differed? No, M in diff base..branch means branch's blob differs from base's blob. So yes branch modified them. That might be accidental edits. But the user didn't ask about that. I could mention as a caution: on current branch there are also modifications to files not authored by her (README, lom/notiz, ngh, sngu) — possibly unintentional, and per repo rules she should only change her own files. That's valuable. Let me verify which files are M on ue04 branch.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git diff --name-status 327b99f21f0bb37a03bded83b383aae07b844774 ue04-madeleinekenne | Select-String \"^M\""
}
```

(no output)

---

## Assistant

_Thinking:_

Hmm, no M? Wait earlier the diff main..branch showed M for README etc., but base..branch shows none? Let me re-run base..branch filtering. Actually earlier command `git diff --name-status 327b99f... ue04-madeleinekenne` output started with D lines only? The output was huge deletions. Wait the merge-base for ue04 is 327b99f. base..branch diff should show changes branch made since base. It showed many D (deletions)?? That doesn't make sense—branch can't have deleted all those files relative to base unless branch is a subset. Actually maybe branch IS a subset (she deleted other students' files in her branch). But working tree has all files... Wait if branch deleted them, checking out branch would remove them. But working tree has them. Contradiction again.

Let me check current HEAD and status. Current branch ue04-madeleinekenne. git status said only untracked ue04/. So working tree matches branch. But Get-ChildItem showed all ue01/ue02/ue03 files. So branch does contain all files. Then why diff base..branch shows D for all? Because base 327b99f might be NEWER than branch? No, merge-base is common ancestor; branch should have files at least as many as base.

Wait maybe 327b99f is not an ancestor but merge-base computed weirdly because branches diverged with unrelated histories? Let me check if 327b99f is ancestor of branch.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git merge-base --is-ancestor 327b99f21f0bb37a03bded83b383aae07b844774 ue04-madeleinekenne; echo \"exit: $?\"; echo \"--- is 327 ancestor of main? ---\"; git merge-base --is-ancestor 327b99f21f0bb37a03bded83b383aae07b844774 main; echo \"exit: $?\""
}
```

exit: True
--- is 327 ancestor of main? ---
exit: True


---

## Assistant

_Thinking:_

So 327 is ancestor of both. Then why diff base..branch shows deletions? Let me look more carefully—maybe the diff output earlier was main..branch not base..branch? Let me re-run base..branch with stat summary.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git diff --stat 327b99f21f0bb37a03bded83b383aae07b844774 ue04-madeleinekenne | tail -5"
}
```

tail : The term 'tail' is not recognized as the name of a cmdlet, function, script file, or operable program. Check 
the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:163
+ ... 27b99f21f0bb37a03bded83b383aae07b844774 ue04-madeleinekenne | tail -5
+                                                                   ~~~~
    + CategoryInfo          : ObjectNotFound: (tail:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
 

Exited with code 1

---

## Assistant

_Thinking:_

Let me get the diff stat summary.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git diff --shortstat 327b99f21f0bb37a03bded83b383aae07b844774 ue04-madeleinekenne"
}
```

 3 files changed, 91 insertions(+)


---

## Assistant

_Thinking:_

So only 3 files changed, 91 insertions. The earlier huge D list was from `main..branch`? No, earlier I ran `git diff --name-status main..$b` which compares main to branch; since main has many more files (later additions), branch appears to delete them. So the huge list was misleading. The real branch changes (base..branch) are 3 files. Let me get their names.

**Tool: shell**

**Input:**
```json
{
  "command": "cd \"C:\\Users\\Ks_Store\\Desktop\\first-project\\thm_wk-1208_softwaretechnik-uebungen\"; git diff --name-status 327b99f21f0bb37a03bded83b383aae07b844774 ue04-madeleinekenne"
}
```

A	ue03/mken/anforderungen.md
A	ue03/mken/kontext.md
A	ue03/mken/zuordnung.md


---

## Assistant

_Thinking:_

So on ue04 branch, relative to base, only added ue03/mken files. The ue01 steckbrief was added on steckbrief-mken branch (merged via PR). The ue04/madeleinekenne/einrichtung.md is untracked.

So her files total:
- ue01/steckbriefe/mken.md (from steckbrief-mken, merged to main)
- ue02/notiz.md, ue02/spezifikation.md (from ue02mken, local only, not merged)
- ue03/mken/{anforderungen,kontext,zuordnung}.md (from ue03-mken/ue04, merged to main via PR #326)
- ue04/madeleinekenne/einrichtung.md (untracked, current)

Good. Let me also check steckbrief-mken base and whether it added only mken.md (yes).

Now final answer. Keep it concise. Mention git identity. Mention repo structure. End with list. Also note that other files are other students'; don't edit.

## Was in diesem Repository liegt

Dies ist das **Übungsrepository der Veranstaltung „Softwaretechnik“** (THM, Campus Friedberg, FB MND). Es sammelt die Einreichungen der Studierenden über Forks, Branches und Pull Requests. Jede Übung hat ein eigenes Verzeichnis mit eigener `README.md`:

| Verzeichnis | Inhalt |
|---|---|
| `ue01/` | Erste Schritte mit Git/GitHub (Steckbriefe unter `ue01/steckbriefe/`) |
| `ue02/` | Projektmodell (je Studierender ein Unterordner mit `notiz.md`, `phasenplan.md`, `spezifikation.md`, optional `rollen.md`) |
| `ue03/` | Anforderungen an den Terminplaner (je Studierender ein Unterordner mit `anforderungen.md`, `kontext.md`, `zuordnung.md`) |
| `ue04/` | Coding-Agent-Einrichtung (`einrichtung.md` je Studierender) |
| `README.md` (Wurzel) | Regeln, Einreichungsablauf, Spielregeln |

Ihre Git-Identität ist als **Madeleine kenne** (`madeleine.ningpeye.kenne@mnd.thm.de`) konfiguriert, Kürzel **mken** (bzw. Branch-Name `madeleinekenne`).

## Dateien, die von Ihnen stammen

**Bereits in `main` gemergt (über Pull Requests):**
- `ue01/steckbriefe/mken.md`
- `ue03/mken/anforderungen.md`
- `ue03/mken/kontext.md`
- `ue03/mken/zuordnung.md`

**Auf lokalem Branch `ue02mken` (nicht in `main` gemergt):**
- `ue02/notiz.md`
- `ue02/spezifikation.md`

**Auf dem aktuellen Branch `ue04-madeleinekenne` (neu, noch untracked):**
- `ue04/madeleinekenne/einrichtung.md`

Alles andere in den Ordnern `ue01/`–`ue04/` gehört zu anderen Studierenden bzw. sind Vorlagen (`_vorlage`, `_beispiel`, `_zugabe`) und die Repository-Infrastruktur. Gemäß den Spielregeln des Repositories sollten Sie nur Ihre eigenen Dateien ändern.
