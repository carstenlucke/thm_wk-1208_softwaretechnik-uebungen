# Von Hand und mit dem Agenten — Terminplaner für die THM

Agent: Claude Code, jede Aufgabe in einer neuen Sitzung.

## Aufgabe 1 — Use-Case-Diagramm

- **Erfundenes:** nichts. Alle Akteure und Use-Cases stammen aus Beschreibung 1. Die Notiz zum Sekretariat („nur für die betreuten Lehrenden“) steht so im Text.
- **Fehlendes:** Der Agent hat die Bedingung „[Sprechstunde ausgebucht]“ an den «extend»-Pfeil geschrieben, aber keinen Erweiterungspunkt in „Zeitfenster buchen“ eingetragen. In meiner Zeichnung fehlt er ebenfalls; erst beim Vergleich ist mir aufgefallen, dass er im Use-Case stehen müsste (`extension points: ausgebucht`).
- **Use-Case oder Schritt:** „Mit Hochschulkonto anmelden“ ist kein Use-Case, sondern ein Schritt bzw. eine Vorbedingung. Niemand benutzt den Terminplaner, um sich anzumelden; die Anmeldung hat für den Akteur kein eigenes Ergebnis. Alle anderen Use-Cases schließen mit einem Ergebnis ab. Das Aufteilen in 15-Minuten-Fenster hat der Agent zu Recht nicht als Use-Case gezeichnet.
- **«include» und «extend»:** Die Richtungen stimmen. «include» zeigt vom Basis-Use-Case auf den eingebundenen („Buchung stornieren“ → „Lehrperson benachrichtigen“, „Sprechstunde absagen“ → „Gebuchte Studierende benachrichtigen“), «extend» zeigt von der Erweiterung auf den Basis-Use-Case („Auf Warteliste setzen“ → „Zeitfenster buchen“). Das stimmt mit meiner Zeichnung überein.
- **Anmeldedienst:** Der Agent hat ihn als Akteur mit «System» gezeichnet (richtig), aber an den Use-Case „Anmelden“ gehängt, den die vier Use-Cases per «include» einbinden. «include» hieße, dass sich die Studentin bei jedem Buchen anmeldet; Beschreibung 2 sagt aber „Ist sie noch nicht angemeldet …“. In meiner Zeichnung ist er ein sekundärer Akteur rechts an den vier Use-Cases, die eine Anmeldung voraussetzen.
- **Kleinigkeit:** Der Akteur heißt „Lehrende“ (Plural). Ein Akteur ist eine Rolle, also besser „Lehrperson“. Habe ich gelassen, weil es die Bedeutung nicht ändert.

**Meine Korrektur in `usecase.puml`:** Den Use-Case „Mit Hochschulkonto anmelden“ und die vier «include»-Pfeile darauf gelöscht. Der Anmeldedienst ist jetzt direkt mit „Sprechstunde anlegen“, „Sprechstunde absagen“, „Zeitfenster buchen“ und „Buchung stornieren“ verbunden, und eine Notiz nennt die Anmeldung als Vorbedingung. Grund: Anmelden ist kein Ziel eines Akteurs, sondern Voraussetzung; der Anmeldedienst wirkt aber an diesen vier Use-Cases mit.

## Aufgabe 2 — Aktivitätsdiagramm

- **Bahnen, Start und Ende:** beide Bahnen da, jede Aktion in der richtigen Bahn, ein Startknoten, ein Endknoten.
- **Verzweigung und Zusammenführung:** „Schon angemeldet?“ wird nach „Mit Hochschulkonto anmelden“ wieder zusammengeführt (Raute vor „Freie Zeitfenster anzeigen“). Die Schleife hat ihren eigenen Zusammenführungsknoten.
- **Rückweg „inzwischen vergeben“:** führt richtig zurück vor „Freie Zeitfenster der Sprechstunde anzeigen“, nicht etwa zu „Zeitfenster auswählen“. Das stimmt mit meiner Zeichnung überein.
- **„Zugleich“:** als Gabelung mit Vereinigung gezeichnet, drei parallele Aktionen. Richtig.
- **Fehler:** Nach der Vereinigung stand noch eine Aktion „Buchung abgeschlossen“. Das ist keine Tätigkeit, sondern das Ergebnis; „sind alle drei erledigt, ist die Buchung abgeschlossen“ heißt: Vereinigung, dann Endknoten. Diese Aktion habe ich selbst im Text gelöscht.
- **Kleinigkeit:** Die Bedingungen an den Kanten stehen ohne eckige Klammern („nein“, „ja“). In der UML wären es Guards wie `[vergeben]`; PlantUML zeichnet sie so, das habe ich gelassen.

**Die Änderung um die Warteliste:** Laut `git diff` hat der Agent nur 13 Zeilen eingefügt und sonst nichts umgestellt. Neu ist direkt nach „Freie Zeitfenster anzeigen“ die Verzweigung „Noch ein Zeitfenster frei?“; bei „nein“ folgen „Warteliste anbieten“ (Terminplaner), „Warteliste annehmen?“ (Studentin) und bei „ja“ „Studentin auf die Warteliste setzen“ mit eigenem Endknoten. Das ist richtig eingefügt. Fehler: Der Zweig „Warteliste annehmen? → nein“ war leer, d.h. der Ablauf lief weiter zu „Zeitfenster auswählen“, obwohl keines frei ist. Der Agent hat das selbst gemeldet und nachgefragt, statt etwas zu erfinden. Ich habe dort einen Endknoten in der Bahn „Studentin“ ergänzt (Annahme: Wer ablehnt, beendet den Ablauf ohne Buchung). Unschön bleibt, dass erst angezeigt und dann geprüft wird, ob überhaupt etwas frei ist; „beim Anzeigen“ lässt das aber zu.

## Aufgabe 3 — Klassendiagramm

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | 0 | 0 |
| technische statt fachlicher Datentypen | 12 (keine technischen Typen, aber alle 12 Attribute ganz ohne Typ) | 0 |
| Erfundenes (Attribute, Klassen, Operationen) | 0 | 0 |
| fehlende oder abweichende Multiplizitäten | 0 | 0 |
| Assoziation statt Komposition | 0 | 0 |

Weitere Beobachtungen ohne Regeln:

- Alle fünf Assoziationen sind gerichtet (`-->`, `<--`), also mit Navigationspfeilen. Navigierbarkeit ist eine Entwurfsentscheidung und gehört nicht ins Datenmodell.
- Die Assoziation Zeitfenster–Buchung heißt „hat“; im Text steht kein Verb dafür („für jedes Zeitfenster gibt es höchstens eine Buchung“). Kein echter Fehler.
- Besser als erwartet: keine `id`, keine Operationen, Komposition und Generalisierung richtig, alle Multiplizitäten wie im Text. Der Hauptmangel waren die fehlenden Datentypen.

**Was die Regeln behoben haben und was nicht:** Behoben: Jedes Attribut hat jetzt einen fachlichen Typ (`Kennung`, `Uhrzeit`, `Zeitpunkt`, `Raum` …), alle Assoziationen sind ungerichtet und beschriftet. Neu entstanden ist ein Fehler durch eine unklare Regel: „Klassen im Singular“ hat der Agent so gelesen, dass aus „Studierende“ die Klasse `Student` wird. „Studierende“ ist aber auch im Singular richtig („die/der Studierende“) und steht so im Text. Die Regel ist also unklar, der Agent hat sie nicht übergangen. Besser: „Übernimm die Klassennamen wörtlich aus der Beschreibung, im Singular.“ Ob `ort : Ort` oder `ort : Raum` richtig ist, lässt der Text offen.

### Meine Regeln für Datenmodelle

- Übernimm nur Klassen, Attribute und Beziehungen, die die Beschreibung nennt. Ergänze nichts, auch wenn es naheliegt.
- Schreib keine Operationen; ein Datenmodell enthält nur Daten.
- Führe keine künstlichen Schlüssel ein (`id`, `nr`, `uuid`), wenn die Beschreibung sie nicht nennt.
- Gib jedem Attribut einen fachlichen Datentyp in der Form `name : Typ`. Benenne den Typ mit einem Wort der Fachsprache, großgeschrieben (z. B. `Kennung`, `Name`, `Titel`, `Datum`, `Uhrzeit`, `Zeitpunkt`, `Ort`, `Raum`, `Text`). Verwende nie technische Typen wie `String`, `int`, `Date`, `boolean`.
- Lass Sichtbarkeiten (`+`, `-`) weg.
- Schreib an beide Enden jeder Assoziation eine Multiplizität, genau nach dem Text: „genau ein“ = `1`, „höchstens ein“ = `0..1`, „mindestens ein“ = `1..*`, „mehrere“ = `1..*`, „beliebig viele“ = `*`.
- Zeichne Assoziationen ungerichtet (`--`), ohne Navigationspfeile, und beschrifte jede mit dem Verb aus der Beschreibung.
- Zeichne eine Komposition (`*--`, Raute beim Ganzen), wenn ein Teil zu genau einem Ganzen gehört und mit ihm gelöscht wird; sonst eine einfache Assoziation. Verwende keine Aggregation.
- Fasse gemeinsame Attribute mehrerer Klassen in einer abstrakten Oberklasse zusammen, wenn der Text sie als Arten eines Allgemeineren nennt („zusätzlich“), und zeichne eine Generalisierung (`<|--`).
- Benenne Klassen mit einem Substantiv im Singular.

## Aufgabe 4 — Zustandsdiagramm

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| Endzustände fehlen: Von `abgesagt`, `wahrgenommen` und `verfallen` führt kein Übergang zu einem Endknoten, obwohl sie sich laut Beschreibung „nicht mehr ändern“. | berechtigt | Die drei Zustände beenden den Lebenslauf des Zeitfensters; die Vorlage (Tür, `defekt --> [*]`) zeigt genau diese Notation. Behoben: je ein Übergang `--> [*]`. |
| „Beginn erreicht“ steht wie ein gewöhnliches Ereignis da, ist aber ein Zeit-/Änderungsereignis; UML schreibt dafür `when(…)` bzw. `at(…)`. | berechtigt | Niemand löst „Beginn erreicht“ aus, es tritt ein, wenn die Zeit erreicht ist. Behoben: an allen drei Übergängen `when(Beginn erreicht)`. |

Nicht gemeldet und nach meiner Prüfung richtig: der Oberzustand `angeboten` mit dem einen Übergang „Sprechstunde absagen“, die Bedingung `[jetzt ≤ Beginn − 2 h]` am Stornieren und dass nur `gebucht` zu `wahrgenommen` führt.

## Ein System, vier Sichten

<!-- Vor der nächsten Vorlesung. -->

### Was kommt mehrfach vor?

| Element | Use-Case | Aktivität | Klassen | Zustand |
|---|---|---|---|---|
| … | … | … | … | … |

<!-- Je Zelle: unter welchem Namen und in welcher Form das Element dort
     vorkommt (Akteur, Use-Case, Aktion, Klasse, Zustand …), oder „—“. -->

### Wo passt es nicht zusammen?

- …

### Aus „Zeitfenster“ wird „Termin“

**Stellen:** … in … Dateien
