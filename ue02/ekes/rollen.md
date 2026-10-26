# Rollen — Terminplaner für die THM

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @erhankesbic

## Der Kunde

| Bereich | Wer ist das an der THM? | Woran machen Sie es fest? |
|---|---|---|
| Fachbereich (eigentlicher Auftraggeber) | Das Präsidium der THM, zuständig ist der Bereich Studium und Lehre | Es will das System für die ganze Hochschule, gibt den Auftrag, bezahlt und nimmt am Ende ab. |
| IT-Bereich | Das Hochschulrechenzentrum (HRZ) der THM | Es betreibt die Server und das Hochschulkonto, auf denen das System später läuft. |

## Das Projektteam

Vier Personen: A, B, C und D.

| Rolle | Wer |
|---|---|
| Projektmanager | A |
| Projektleiter | B |
| Chefdesigner | B |
| Entwickler | B, C |
| Qualitätsbeauftragter | D |

Diese Rollen haben wir zusammengelegt, da Projektleiter und Chefdesigner beide den Überblick über das ganze System brauchen und das Projekt klein ist.

Diese Rollen halten wir getrennt, da man die eigenen Fehler schlecht findet. Deshalb entwickelt D nicht mit und prüft nur. Außerdem bleibt A nur Projektmanager, weil A mit der THM über Geld und Termine verhandelt und dabei nicht selbst im Team stecken soll.

## Drei Situationen

| Situation | Wer entscheidet? | Wer muss davon erfahren? |
|---|---|---|
| Ein Sekretariat wünscht sich während der Implementierung zusätzlich eine Raumbuchung. | Der Fachbereich der THM zusammen mit A (Projektmanager), weil es eine neue Anforderung ist, die mehr Zeit und Geld kostet. | B (Projektleiter und Chefdesigner), der Plan und Spezifikation anpassen muss, die Entwickler und das Sekretariat. |
| Der Systemtest zeigt, dass Benachrichtigungen bei vielen gleichzeitigen Buchungen erst nach Minuten ankommen. | B (Projektleiter und Chefdesigner) entscheidet, wie der Fehler behoben wird. | Die Entwickler, D (Qualitätsbeauftragter), der danach erneut testet, und A, falls sich der Termin verschiebt. |
| Um den Einführungstermin zu halten, braucht das Projekt zwei weitere Entwickler. | A (Projektmanager), weil es um Personal und Kosten geht. | B, der die neuen Leute einplant, und der Fachbereich der THM, falls das Projekt dadurch teurer wird. |
