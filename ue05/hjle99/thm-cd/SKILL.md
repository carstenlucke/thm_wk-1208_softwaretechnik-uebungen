---
name: thm-cd
description: Verwendet das Corporate Design der Technischen Hochschule Mittelhessen (THM) für Webseiten, HTML-Seiten, CSS, Benutzeroberflächen und Infografiken. Verwenden, wenn eine Gestaltung im THM-Design, mit THM-Farben oder im Corporate Design der Hochschule verlangt wird.
---

# Corporate Design der THM

## Offizielle Farben

| Farbe | Hex-Wert | RGB |
|---|---|---|
| THM Grün | #80BA24 | 128, 186, 36 |
| THM Grau | #4A5C66 | 74, 92, 102 |
| THM Rot | #9C132E | 156, 19, 46 |
| THM Gelb | #F4AA00 | 244, 170, 0 |
| THM Hellblau | #00B8E4 | 0, 184, 228 |
| THM Blau | #002878 | 0, 40, 120 |

## Verwendung der Farben

- THM Grün ist die Hauptfarbe und dient für Akzente, Überschriften und dekorative Flächen.
- THM Grau ist die Hauptfarbe und wird für Fließtext verwendet.
- THM Rot, Gelb, Hellblau und Blau sind Sekundärfarben für besondere Hervorhebungen und Infografiken.
- THM Blau kann für Links verwendet werden.
- Weiß kann als Hintergrundfarbe verwendet werden.

## Lesbarkeit

- Fließtext auf weißem Hintergrund muss THM Grau (#4A5C66) verwenden.
- THM Grün darf nicht als Fließtextfarbe auf weißem Hintergrund verwendet werden.
- Normaler Text muss ein Kontrastverhältnis von mindestens 4,5:1 erreichen.
- Weiße Schrift darf nur auf ausreichend dunklen Hintergründen verwendet werden.

## CSS-Regeln

Definiere alle Farben zentral im :root-Selektor mit CSS-Variablen.

Beispiel:

```css
:root {
  --thm-gruen: #80BA24;
  --thm-grau: #4A5C66;
  --thm-rot: #9C132E;
  --thm-gelb: #F4AA00;
  --thm-hellblau: #00B8E4;
  --thm-blau: #002878;
  --thm-weiss: #FFFFFF;
}

body {
  background: var(--thm-weiss);
  color: var(--thm-grau);
}
```

Verwende im gesamten Dokument die CSS-Variablen anstelle wiederholter Farbwerte.

## Was zu vermeiden ist

- Keine zusätzlichen Farben erfinden.
- Keine Farbverläufe verwenden.
- Keine Schatten verwenden.
- Keine zusätzlichen Farbtöne durch Transparenz oder Filter erzeugen.
- Keine falschen Hex-Werte verwenden.
- Keine unlesbaren Farbkombinationen verwenden.

## Vorgehen

1. Lade diesen Skill, sobald eine Aufgabe das Corporate Design der THM verlangt.
2. Verwende ausschließlich die festgelegten Farbwerte.
3. Weise jeder Farbe eine passende Rolle zu.
4. Definiere die Farben zentral als CSS-Variablen.
5. Prüfe die Lesbarkeit und den Kontrast.
6. Kontrolliere, dass keine unerlaubten Farben vorkommen.