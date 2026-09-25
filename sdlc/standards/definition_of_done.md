# Definition of Done

**Was ist das?** Die Checkliste, die eine Implementierung erfüllen muss, um als **fertig** zu gelten. Sie ist der Maßstab, gegen den reviewt wird — von Menschen und von der KI.

**Warum gerade mit KI wichtig?** Ein Agent meldet "fertig", sobald der Code läuft. Ob er lesbar, getestet und architekturkonform ist, prüft er nur, wenn man es ihm als Kriterium mitgibt. Die DoD ist genau diese Vorgabe in Dateiform.

---

Eine Implementierung ist fertig, wenn:

- [ ] Alle **Akzeptanzkriterien** der Story sind erfüllt
- [ ] **Tests** decken das neue Verhalten ab — und wurden *fehlschlagen gesehen*
- [ ] Die gesamte **Test-Suite ist grün**
- [ ] Der Code folgt `architecture.md` und `code_style.md`
- [ ] **Lesbarkeit:** sprechende Namen, keine toten Pfade, keine auskommentierten Reste
- [ ] **Fehlerbehandlung** ist bewusst gestaltet, nicht nur "happy path"
- [ ] **Sicherheit:** keine Secrets im Code, Eingaben werden validiert
- [ ] **Dokumentation** ist aktualisiert, wo sie durch die Änderung veraltet wäre
- [ ] Ein **Review in frischer Session** wurde durchlaufen und die Findings bewertet

Diese Datei bleibt bewusst **unter 200 Zeilen**. Sie wird in jeder Review-Session gelesen und kostet damit jedes Mal Kontext.
