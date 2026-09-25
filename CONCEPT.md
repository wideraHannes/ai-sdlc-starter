# Repository-Konzept

## Zweck

Ein **Demo-Projekt**, an dem der Software Development Lifecycle mit
KI-Unterstützung wiederholt wird — mit Beispielen und einer Struktur, die den
Ablauf sichtbar macht.

Grundlage ist der [SDLC Workshop Refresher](prerequisites/sdlc_refresher.md) aus
dem Workshop *AI-Assisted Coding* der
[codecentric AG](https://www.codecentric.de/).

## Leitgedanke

Jeder SDLC-Schritt erzeugt eine **Markdown-Datei**, die der nächste Schritt als
Input liest. Diese Dateien steuern die KI und machen ihre Arbeit wiederholbar,
überprüfbar und im Team teilbar.

```
unrefined  →  refined  →  plan  →  Implementierung  →  review  →  docs
              ↑ DoR                       ↑ Tests       ↑ DoD       ↺
```

Die Ordnerstruktur bildet diesen Fluss ab — ein Ticket wandert sichtbar durch die
Phasen, statt in einem Tool zu verschwinden. Wo was liegt, beschreibt
[`sdlc/README.md`](sdlc/README.md).

Zu jedem Schritt gibt es einen [Standard-Prompt](sdlc/standards/prompts/README.md)
und Beispiele zum Nachschlagen. Definition of Ready und Definition of Done liegen
fertig im Repository — als Anschauungsmaterial, nicht als letztes Wort: beide
werden gemeinsam mit der KI neu erarbeitet und überschrieben.

## Arbeitsweise

- **Jede Session endet mit einem eingecheckten Ergebnis.** Kein Stand bleibt nur
  in einer KI-Session.
- **Wiederholt sich ein Prompt, wird er ein Skill** und ist ab da per
  `/skill-name` aufrufbar.

## Prinzipien

- **Kontext schlägt Befehle.** Die KI wie einen Senior-Entwickler behandeln, der
  um 3 Uhr nachts geweckt und vor ein unbekanntes Projekt gesetzt wurde: fähig,
  aber ohne jeden Kontext.
- **Dialog statt Einzeiler.** Nicht "erstelle eine Definition of Done", sondern
  "hilf uns eine DoD zu erstellen — was gehört rein? Stell eine Frage nach der
  anderen."
- **Reviews in frischer Session.** Wer den Code geschrieben hat, ist auf die
  eigenen Entscheidungen voreingenommen — die KI genauso wie ein Mensch.
- **Steuerungsdokumente kurz halten.** Alles in `architecture.md` und
  `code_style.md` kostet in *jeder* Session Kontext.
- **Manuell prüfen, nach Priorität.** Steuerungsdokumente zuerst, dann
  Stories/Pläne/Reviews, dann Tests, dann Business-Logik, dann der Rest.
- **Tests, die man nicht hat fehlschlagen sehen, sind wertlos.**

## Loslegen

Dieses Repository ist eine **Vorlage**: der Prozess steht, das Projekt fehlt.
Jeder Durchlauf beginnt mit einer frischen Kopie.

1. **Domäne und Tech-Stack festlegen.** Klein genug, dass eine Story in einer
   Session umsetzbar ist.
2. **Rohe Stories nach `sdlc/backlog/unrefined/`** legen (`ST-001.md`, …).
   Bewusst unfertig: sie sind der Input für den ersten Schritt.
3. **Anfangen** mit [`sdlc/standards/prompts/01_plan.md`](sdlc/standards/prompts/01_plan.md).

`architecture.md` und `code_style.md` werden *nicht* vorab ausgefüllt. Sie
entstehen im Durchlauf selbst — gemeinsam mit der KI, vor dem ersten
Implementierungsplan. Dasselbe gilt für Definition of Ready und Done: die
vorhandenen Fassungen sind Anschauungsmaterial, kein Ergebnis.
