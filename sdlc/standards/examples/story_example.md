# Beispiel: Eine Story, die die Definition of Ready erfüllt

Dieses Dokument ist **kein echtes Ticket**, sondern ein Anschauungsbeispiel für die
[Definition of Ready](../definition_of_ready.md).

---

# ST-001: Passwort zurücksetzen

**Als** registrierter Nutzer
**möchte ich** mein Passwort per E-Mail zurücksetzen können,
**damit** ich wieder Zugriff auf mein Konto bekomme, wenn ich es vergessen habe.

## Akzeptanzkriterien
- Bei Eingabe einer registrierten E-Mail wird eine Mail mit Reset-Link versendet
- Der Link ist 60 Minuten gültig und nur einmal verwendbar
- Bei Eingabe einer *nicht* registrierten E-Mail erscheint dieselbe Bestätigung
  (keine Auskunft darüber, ob ein Konto existiert)
- Nach erfolgreichem Reset werden alle bestehenden Sessions beendet

## Nicht Teil dieser Story
- Zurücksetzen per SMS
- Änderung des Passworts bei eingeloggtem Nutzer

## Abhängigkeiten
- Mailversand (ST-014) muss verfügbar sein
