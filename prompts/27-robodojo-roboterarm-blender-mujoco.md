# RoboDojo-Test: Roboterarm in Blender und MuJoCo

Voraussetzung: Claude Code mit Blender und Python. Fehlende Abhängigkeiten wie MuJoCo richtet das Modell selbst ein. Für den Vision-Modus ruft die Simulation die Claude CLI oder die API auf.

```text
Laut dem Artikel ist Claude gut in RoboDojo: https://www.anthropic.com/claude-fable-and-mythos-5-2 Du musst das für mich beweisen mit folgender Aufgabe:

Baue hier eine vorführbare Robotik-Demo: Entwirf und modelliere einen eigenen, visuell beeindruckenden Roboterarm mit Greifer in Blender und mache denselben Roboter in einer Physik-Simulation wie MuJoCo funktionsfähig. Blender und Simulation lesen dieselbe Bauteil-Beschreibung. Bewegungen und Greifen müssen durch simulierte Motoren und physische Kontakte entstehen, der Greifer hält nur über Reibung.

Der Roboter hat zwei Gehirne, zwischen denen ich per Taste umschalte:

1. Code-Modus (schnell): Der Arm sortiert autonom verstreute Würfel nach Farbe. Werden Würfel verschoben, weggeworfen oder aus dem Greifer geschlagen, plant er neu.

2. Vision-Modus (Claude als Gehirn): Claude bekommt nur ein Kamerabild von oben mit Maßraster und die Greiferöffnung, keine Positionen aus der Simulation. Über eine Prompt-Box tippe ich Aufträge ein, zum Beispiel „Sortiere alle Würfel“, „Bau einen Turm aus zwei grünen Würfeln“ oder „Welche Würfel liegen noch lose herum?“. Claude antwortet mit Aktionen (greifen, ablegen, stapeln, schieben, zoomen), die über dieselben Motoren laufen wie im Code-Modus. Die Motorregelung bleibt klassischer Code. Vor jeder Aufnahme fährt der Arm aus dem Bild. Im Fenster sehe ich, was Claude denkt und welches Bild es gerade bekommen hat. Kann ein Auftrag nicht erfüllt werden, bricht Claude ab und sagt warum.

Steuerung: Ich will den Arm auch per Tastatur und Maus selbst steuern. Dazu Tasten fürs Video: Modus umschalten, Prompt-Box öffnen, alle Würfel durcheinanderwerfen, neue Anordnung (setzt alles zurück, also Neustart per Knopfdruck), nur den Arm zurücksetzen, einzelne Würfel mit der Maus verschieben, Kamerafahrt, Screenshot und eine Hilfe-Einblendung mit allen Tasten. Dazu ein fester Seed per Kommandozeile für reproduzierbare Anordnungen.

Gestalte alles selbst, richte fehlende Projektabhängigkeiten ein und teste mehrere zufällige Anordnungen automatisch, auch mit Störungen. Teste den Vision-Modus mit mehreren Aufträgen und berichte Ergebnis, Anzahl der Claude-Aufrufe, Dauer und Ablesegenauigkeit als Tabelle. Prüfe auch die Darstellung und verbessere Fehler selbstständig.

Liefere die Blender-Datei, eine per Doppelklick startbare interaktive Simulation und eine kurze Bedienungsanleitung vom Öffnen bis zum Bedienen. Erkläre zum Schluss ehrlich, was in der Demo Claude entscheidet und was Code ist, und wie sich die Demo zu RoboDojo verhält.

Falls du weitere Ideen hast, die rein sollten, setz sie um, es soll ein super beeindruckendes Demo für YouTube werden. Aber du hast nur ca. 40–60 Minuten Zeit, das alles umzusetzen!
```
