# Einrichtung — Coding Agent

<!-- Aufgaben 1 und 2 des Übungsblatts. Ersetzen Sie jedes „…“ durch Ihre
     Angabe; die Überschriften bleiben stehen. Löschen Sie die Kommentare,
     sobald Sie fertig sind. Die Sitzung mit dem Agenten gehört nicht
     hierher, sondern als Export in die Datei sitzung.md daneben. -->

## Aufbau

| Angabe | Ihre Angabe |
|---|---|
| Läuft der Agent? | Nein|
| Werkzeug | opencode|
| Version | entfällt (opencode CLI nicht installiert / command not found) |
| Betriebssystem | macOs|
| Modellzugang | OpenCode Zen |
| Modell | entfällt (da keine Modellauswahl im Terminal möglich war)|

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

**Befehl und Ausgabe:** Starten des Agenten im Terminal

```text
Ahmets-MacBook-Pro:thm_wk-1208_softwaretechnik-uebungen ahnetyikits$ opencode
bash: opencode: command not found
…
```

**Bereits versucht:** …
Unter der Überschrift **„## Wenn es nicht läuft“** ersetzen Sie die drei Platzhalter `...` durch den gescheiterten Befehl und die Fehlermeldung aus Ihrem Terminal.

Ersetzen Sie die Zeilen 47 bis 55 komplett durch diesen vorbereiteten Block:

```markdown
**Schritt, an dem es scheitert:** Starten des Agenten im Terminal

**Befehl und Ausgabe:**

```text
Ahmets-MacBook-Pro:thm_wk-1208_softwaretechnik-uebungen ahnetyikits$ opencode
bash: opencode: command not found

```

**Bereits versucht:** Aufruf von opencode im VS Code Terminal; Befehl steht systemweit nicht zur Verfügung (CLI nicht installiert).

```

<Steps>
  <Step subtitle="sitzung.md löschen" title="1. Nicht benötigte Datei entfernen">
    Laut Anleitung im Auskommentierten (`ohne laufenden Agenten entfällt sitzung.md`) benötigen Sie keine `sitzung.md`. Falls Sie diese vorhin angelegt haben, löschen Sie sie im Explorer links per Rechtsklick -> **Delete**.
    *Verification:* Die Datei `sitzung.md` ist aus Ihrem Ordner `ue04/ahyi` entfernt.
  </Step>

  <Step subtitle="einrichtung.md speichern" title="2. Datei abspeichern">
    Drücken Sie **`Cmd + S`**, um `einrichtung.md` zu speichern.
    *Verification:* Das kleine weiße/blaue Punkt-Symbol am oberen Rand des Tabs verschwindet.
  </Step>

  <Step subtitle="VS Code Terminal" title="3. Fertigen Stand committen und pushen">
    Geben Sie diese drei Befehle nacheinander im Terminal ein:
    ```bash
    git add .
    git commit -m "ue04: einrichtung.md ausgefüllt (Agent nicht verfügbar)"
    git push -u origin ue04-ahyi
    ```
    *Verification:* Das Terminal meldet Erfolg (`To github.com:...` und `Branch 'ue04-ahyi' set up to track...`).
  </Step>
</Steps>

<ElicitationsGroup message="Wie hat das Pushen geklappt?">
  <Elicitation label="Git Push war erfolgreich" query="Der Git Push hat geklappt. Wie erstelle ich jetzt den Pull Request auf GitHub?"/>
  <Elicitation label="Fehler im Terminal" query="Beim git push gab es eine Fehlermeldung."/>
</ElicitationsGroup>

```