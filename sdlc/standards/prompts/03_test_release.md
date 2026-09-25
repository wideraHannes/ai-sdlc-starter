# Test / Release — Review & Rework

Ziel: das Ergebnis gegen einen Maßstab prüfen, der vorher feststand — und die
Findings bewerten, bevor sie abgearbeitet werden.

**Review und Rework laufen immer in einer separaten Session.** Wer den Code
geschrieben hat, ist auf die eigenen Entscheidungen voreingenommen — eine
KI-Session genauso wie ein Mensch.

---

## Definition of Done erarbeiten

Einmalig, wieder als Dialog.

```
Wir brauchen eine "Definition of Done" für unser Projekt, damit jede
Implementierung eine definierte Qualität hat und denselben Regeln folgt.

Enthalten sein sollte:
- Lesbarkeit
- Wartbarkeit
- Testabdeckung
- Einhaltung von architecture.md und code_style.md
- die Akzeptanzkriterien der Story

Welche Aspekte gehören deiner Meinung nach noch hinein?
Stell eine Frage nach der anderen.

Bleib unter 200 Zeilen — die Datei wird in jeder Review-Session gelesen.
Speichere sie als sdlc/standards/definition_of_done.md
```

## Review

```
Review die Änderungen, die für sdlc/backlog/refined/ST-XXX.md gemäß dem Plan
in sdlc/backlog/plans/ST-XXX_plan_v2.md gemacht wurden.

Ist die Implementierung *konsistent*, *sicher*, *wartbar*?

Folgt sie @sdlc/standards/architecture.md, @sdlc/standards/code_style.md und
@sdlc/standards/definition_of_done.md?

Speichere den Report als sdlc/backlog/reviews/ST-XXX_review.md
```

Dann: Findings **manuell** durchgehen und entscheiden, welche die Überarbeitung
wert sind. Nicht jedes Finding ist eines.

## Rework

```
Sieh dir sdlc/backlog/reviews/ST-XXX_review.md an.

Arbeite die folgenden Findings ab — eines nach dem anderen:
[hier die ausgewählten Findings nennen]

Folge @sdlc/standards/architecture.md und @sdlc/standards/code_style.md.
```

Danach erneut reviewen. Die Schleife läuft, bis das Ergebnis trägt.

## Tests

Zwei Regeln, die keine Abkürzung kennen:

- Tests werden **immer manuell geprüft**. KI-geschriebene Tests können subtil
  falsch sein — etwa so, dass sie immer grün sind.
- Ein Test, den man **nicht hat fehlschlagen sehen**, ist wertlos.
