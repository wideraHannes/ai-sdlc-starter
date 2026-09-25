# Standard-Prompts

Die wiederkehrenden Prompts des SDLC — einer pro Schritt, mit den Pfaden dieses
Repositories. Zum Kopieren, nicht zum Auswendiglernen.

| Datei | Schritt | Erzeugt |
| --- | --- | --- |
| [`01_plan.md`](01_plan.md) | Story Refinement | `backlog/refined/ST-XXX.md` |
| [`02_code.md`](02_code.md) | Implementierungsplanung & Umsetzung | `backlog/plans/ST-XXX_plan.md`, Code |
| [`03_test_release.md`](03_test_release.md) | Review & Rework | `backlog/reviews/ST-XXX_review.md` |
| [`04_documentation.md`](04_documentation.md) | Dokumentation | `docs/` |

`ST-XXX` ist überall durch den echten Identifier des Arbeitspakets zu ersetzen.

## Wie diese Prompts zu lesen sind

Sie sind **Startpunkte für ein Gespräch**, keine Zauberformeln. Wo ein Prompt eine
Rückfrage auslöst, ist das ein gutes Zeichen: die KI holt Kontext, den sie sonst
erfunden hätte.

Die Sprache ist egal — wer lieber auf Englisch promptet, tut das. Was zählt, sind
die mitgelieferten Dateien und das, was als Ergebnis erwartet wird.

## Dos & Don'ts

**Nicht so:** „erstelle eine Definition of Done" — ein nackter Befehl liefert
generische Boilerplate.

**Auch nicht:** „bitte …", „kannst du …" — Höflichkeitsfloskeln tragen nichts bei.

**Sondern:** „Hilf uns, eine Definition of Done zu erstellen. Was gehört hinein?
[…] Stell eine Frage nach der anderen." So kommt das Wissen des Teams heraus
statt des Durchschnitts aus den Trainingsdaten.

## Wenn ein Prompt zum dritten Mal getippt wird

Dann gehört er nicht mehr hierher, sondern wird ein Skill und ist ab da per
`/skill-name` aufrufbar. Jede Überschrift in diesen Dateien ist ein Kandidat dafür.
