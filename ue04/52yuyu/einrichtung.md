# Einrichtung Coding Agent – Übung 4

## Aufbau

| Frage / Eigenschaft | Antwort / Wert |
| :--- | :--- |
| **Werkzeug** | opencode (CLI Agent) |
| **Modellzugang** | OpenCode Zen (DeepSeek V4.1 Flash Free) |
| **Läuft der Agent?** | ja |

## Antworten zu den Kontrollfragen

1. **Was prüft `opencode --version`, was prüft „Sag Hallo und nenne dein Modell.“ – und warum genügt das eine nicht ohne das andere?**
   * `opencode --version` prüft nur, ob das CLI-Werkzeug auf dem Rechner lokal installiert ist[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span).
   * „Sag Hallo...“ prüft die Netzwerkverbindung, Authentifizierung und Erreichbarkeit des Sprachmodells im Backend[span_8](start_span)[span_8](end_span)[span_9](start_span)[span_9](end_span).
   * Beides ist nötig: Ein installiertes Tool ohne Modellverbindung funktioniert nicht, und ein erreichbares Modell bringt nichts ohne das CLI-Werkzeug[span_10](start_span)[span_10](end_span)[span_11](start_span)[span_11](end_span).

2. **Warum lässt sich opencode mit Modellen ganz verschiedener Anbieter betreiben?**
   * Weil `opencode` entkoppelt konzipiert ist[span_12](start_span)[span_12](end_span)[span_13](start_span)[span_13](end_span). Es nutzt einheitliche API-Schnittstellen, um Prompts an beliebige LLM-Anbieter (OpenAI, Anthropic, OpenCode Zen etc.) zu senden und die Antworten lokal im Repository zu verarbeiten[span_14](start_span)[span_14](end_span)[span_15](start_span)[span_15](end_span).

3. **Wer ein Claude-Abo hat, kann damit in opencode nicht arbeiten. Was spräche dagegen, stattdessen einen API-Schlüssel zu nehmen?**
   * **Abo:** Nutzungsbedingungen von Anthropic verbieten die Verwendung des Web-/App-Abos in Dritthersteller-Tools[span_16](start_span)[span_16](end_span).
   * **API-Schlüssel:** Rechnet strikt nach Token-Verbrauch ab[span_17](start_span)[span_17](end_span). Da Agenten bei jeder Aktion große Teile des Projektkontextes mitsenden, können die Kosten schnell sehr hoch werden im Vergleich zu einer Flatrate[span_18](start_span)[span_18](end_span).

## Antwort des Agenten geprüft

Der Agent hat die Ordnerstruktur korrekt gescannt und meine Dateien aus den bisherigen Übungen identifiziert. Es wurden keine fremden Dateien erfunden.
