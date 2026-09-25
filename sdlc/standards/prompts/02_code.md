# Code — Implementierungsplanung & Umsetzung

Ziel: den Agenten nicht "einfach coden" lassen. Erst planen, den Plan kritisch
gegenlesen, dann umsetzen.

---

## Implementierungsplan schreiben

```
Erstelle einen Implementierungsplan für die Story
sdlc/backlog/refined/ST-XXX.md.

Sieh dir zuerst die aktuelle Implementierung an.

- Welche *Teile* der Anwendung müssen geändert werden, und warum?
- Welche *Tests* sollten geschrieben werden?

Folge @sdlc/standards/architecture.md und @sdlc/standards/code_style.md.

Speichere den Plan als sdlc/backlog/plans/ST-XXX_plan.md
```

## Plan reviewen

In einer **frischen Session**. Die Formulierung „ein anderer Entwickler" ist
Absicht: gegenüber fremder Arbeit ist die Kritik ehrlicher als gegenüber der
eigenen.

```
Ein Senior-Entwickler hat einen Plan für sdlc/backlog/refined/ST-XXX.md
geschrieben: sdlc/backlog/plans/ST-XXX_plan.md

Review diesen Plan.

Was sind seine *Stärken*, was seine *Schwächen*?
Was würdest du *ändern* — und warum?

Schreibe eine überarbeitete Fassung nach
sdlc/backlog/plans/ST-XXX_plan_v2.md
```

Danach: den Plan **selbst** lesen. Er ist das Dokument, aus dem der ganze Rest
folgt — ein Fehler hier pflanzt sich in jede Zeile Code fort.

## Plan umsetzen

```
Setze sdlc/backlog/refined/ST-XXX.md gemäß dem Plan in
sdlc/backlog/plans/ST-XXX_plan_v2.md um.

Wo es sinnvoll ist, nutze Sub-Agents für einzelne Aufgaben, um den Kontext
der Hauptsession klein zu halten.

Folge @sdlc/standards/architecture.md und @sdlc/standards/code_style.md.
```
