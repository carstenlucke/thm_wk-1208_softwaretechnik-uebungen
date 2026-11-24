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

<!-- Schritt 4: Was stimmte am Diagramm des Agenten nicht, und was haben
     Sie verbessert? -->

- …

**Die Änderung um die Warteliste:** …

<!-- Schritt 7: Hat der Agent nur ergänzt, was verlangt war? Ist die neue
     Verzweigung richtig eingefügt? -->

## Aufgabe 3 — Klassendiagramm

<!-- Schritte 4 und 7: Zahl der Verstöße je Art, ohne und mit Ihren
     Regeln. -->

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | … | … |
| technische statt fachlicher Datentypen | … | … |
| Erfundenes (Attribute, Klassen, Operationen) | … | … |
| fehlende oder abweichende Multiplizitäten | … | … |
| Assoziation statt Komposition | … | … |

**Was die Regeln behoben haben und was nicht:** …

### Meine Regeln für Datenmodelle

<!-- Schritt 5: knapp und eindeutig, als Liste. Der Agent liest diesen
     Abschnitt in Schritt 6. -->

- …

## Aufgabe 4 — Zustandsdiagramm

<!-- Schritt 5: jede Abweichung, welche der Agent gemeldet hat, mit Ihrem
     Urteil (berechtigt / nicht berechtigt) und einem Satz Begründung. -->

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| … | … | … |

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
