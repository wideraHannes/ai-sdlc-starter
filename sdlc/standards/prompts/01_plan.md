# Plan — Story Refinement

Ziel: aus einem rohen Backlog-Eintrag eine Story machen, aus der ein Agent bauen
kann, ohne zu raten.

---

## Definition of Ready erarbeiten

Einmalig — und bewusst als Dialog, nicht als Auftrag.

```
Wir brauchen eine "Definition of Ready" für unser Projekt, damit jedes Ticket
eine definierte Qualität hat.

Enthalten sein sollte:
- Story-Satz ("Als … möchte ich … damit …")
- fachlicher Kontext, wo nötig
- Akzeptanzkriterien

Was gehört deiner Meinung nach noch in eine Story?
Stell eine Frage nach der anderen.

Halte das Ergebnis kurz und knapp.
Speichere es als sdlc/standards/definition_of_ready.md
```

## Story refinen

```
Sieh dir die Story in sdlc/backlog/unrefined/ST-XXX.md an.

Schärfe sie gegen @sdlc/standards/definition_of_ready.md.

Wo dir fachlicher Kontext fehlt, frag nach, statt ihn zu erfinden.

Speichere das Ergebnis als sdlc/backlog/refined/ST-XXX.md
```

Ein Beispiel für eine Story, die die DoR erfüllt:
[`../examples/story_example.md`](../examples/story_example.md)

## Story gegen die DoR prüfen

Zum Gegenlesen — am besten in einer frischen Session.

```
Prüfe sdlc/backlog/refined/ST-XXX.md gegen
@sdlc/standards/definition_of_ready.md.

Welche Kriterien sind erfüllt, welche nicht?
Wo ist die Story noch so vage, dass du beim Umsetzen raten müsstest?
```
