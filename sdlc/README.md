# sdlc — Prozessartefakte

Hier liegt alles, was der Software Development Lifecycle an Dokumenten erzeugt.
Ein Arbeitspaket wandert sichtbar von oben nach unten durch die Ordner.

```
backlog/
  unrefined/    rohe Stories, wie sie vom Produkt kommen
  refined/      gegen die Definition of Ready geschärfte Stories
  plans/        Implementierungspläne (ST-001_plan.md, ST-001_plan_v2.md)
  reviews/      Review-Reports aus der Test-/Release-Phase

standards/
  definition_of_ready.md    wann ist eine Story bereit zur Umsetzung
  definition_of_done.md     wann gilt eine Implementierung als fertig
  architecture.md           wie das System gebaut ist
  code_style.md             wie Code auszusehen hat
  prompts/                  die Standard-Prompts je SDLC-Schritt
  examples/                 angewendete Beispiele zum Nachschlagen
```

Die [Standard-Prompts](standards/prompts/README.md) sind der Einstieg in jeden
Schritt: pro Phase eine Datei, mit den Pfaden dieses Repositories eingesetzt.

Ergänzend außerhalb dieses Ordners:

- [`docs/`](../docs/README.md) — Architekturdokumentation, Diagramme,
  Entscheidungen, Teststrategie
- [`tests/`](../tests/README.md) — Testcode und Testdaten

## Namenskonvention

Ein Arbeitspaket behält seinen Identifier über alle Ordner hinweg:

```
unrefined/ST-001.md  →  refined/ST-001.md  →  plans/ST-001_plan.md
                                           →  plans/ST-001_plan_v2.md
                                           →  reviews/ST-001_review.md
```

So ist auf einen Blick erkennbar, wo ein Ticket steht und was ihm noch fehlt.
