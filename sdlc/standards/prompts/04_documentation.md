# Release — Dokumentation

Ziel: Dokumentation, die nicht veraltet. Mit KI ist ihr Erstellen und
Aktualisieren billig genug, dass es keine Ausrede mehr gibt.

---

## Arc42-Dokumentation erstellen

```
Ich möchte eine Architekturdokumentation für diese Anwendung nach der
Arc42-Vorlage erstellen.

Sieh dir zuerst die vorhandenen Dokumente in @docs/, die Standards
in @sdlc/standards/ und die @README.md an.

Nutze für Diagramme Mermaid oder PlantUML.

Speichere das Ergebnis unter docs/
```

## README für den Einstieg

```
Erstelle eine Übersicht, mit der ein neuer Entwickler in dieses Projekt
hineinfindet: was die Anwendung tut, wie sie gebaut ist, wie man sie lokal
zum Laufen bekommt.

Sieh dir dafür den Code und @docs/ an.

Aktualisiere damit die README.md
```

## Architekturdiagramm

```
Erstelle ein Mermaid-Diagramm der Softwarearchitektur.

Halte dich an das, was tatsächlich im Code steht — nicht an das, was in
@docs/ behauptet wird.
```

## Steuerungsdokumente aktualisieren

```
Die Änderung an ST-XXX ist umgesetzt.

Welche Dokumente sind dadurch veraltet — architecture.md, code_style.md,
docs/?

Nenne sie einzeln mit der Stelle, die nicht mehr stimmt. Ändere noch nichts.
```

Bei `architecture.md` und `code_style.md` anschließend **manuell kürzen**: alles,
was darin steht, kostet in *jeder* Session Kontext.

## Textbasierte Formate

Alles, was dokumentiert wird, bleibt textbasiert und damit versioniert und im
Diff lesbar:

- **Markdown** für Fließtext
- **Mermaid** oder **PlantUML** für Diagramme, **ASCII-Art** als einfache Alternative
- **AsciiDoc**, wo formatierter Text nötig ist (ersetzt Word)

GitHub und GitLab rendern Mermaid direkt; Confluence braucht ein gerendertes
Bild. Für VS Code gibt es Plugins mit Live-Vorschau für Mermaid, PlantUML und
AsciiDoc.
