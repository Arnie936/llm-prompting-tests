# RoboDojo-Test: Roboterarm in Blender und MuJoCo

Voraussetzung: Claude Code mit Blender. Fehlende Abhängigkeiten (z. B. MuJoCo) richtet das Modell selbst ein.

```text
Laut dem Artikel ist Claude gut in RoboDojo: https://www.anthropic.com/claude-fable-and-mythos-5-2 Du musst das für mich beweisen mit folgender Aufgabe:

Baue hier eine vorführbare Robotik-Demo: Entwirf und modelliere einen eigenen, visuell beeindruckenden Roboterarm mit Greifer in Blender und mache denselben Roboter funktionsfähig. Der Roboter kann entweder durch Claude kontrolliert werden (nehme an, du könntest über meine CLI drauf zugreifen, aber auch die API passt; falls das nicht geht, kannst du auch was wie MuJoCo nehmen). Ich möchte ihn per Tastatur oder Maus steuern und autonom verstreute Würfel sortieren lassen. Die Steuerung soll auf verschobene Würfel reagieren. Bewegungen und Greifen müssen durch simulierte Motoren und physische Kontakte entstehen. Gestalte alles selbst, richte fehlende Projektabhängigkeiten ein und teste mehrere zufällige Anordnungen. Prüfe auch die Darstellung und verbessere Fehler selbstständig. Liefere die Blender-Datei, eine einfach startbare interaktive Simulation und eine kurze Bedienungsanleitung. Entscheide die Details selbst und setze es vollständig um.

Falls du weitere Ideen hast, die rein sollten, setz sie um, es soll ein super beeindruckendes Demo für YouTube werden. Aber du hast nur ca. 20–40 Minuten Zeit, das alles umzusetzen!
```

## Stufe 2: Vision statt Code

```text
Frage: Wenn der Roboter die Würfel sucht, läuft das alles über Code, oder? Kannst du aber auch als Gehirn übernehmen und mit Vision das Ganze lösen? Und könnten wir auch die Schwierigkeit weiter erhöhen? RoboDojo misst, meine ich, ja schwerere Sachen, oder?
```

```text
Wir machen es so: Du baust die Vision-Variante, aber so, dass wir switchen können: einmal der klassische Code, der schnell ist, und einmal deine Vision-Variante. Damit das Ganze schwerer wird, soll bei der Vision-Variante eine Prompting-Box dabei sein. Da schreibe ich rein, was passieren soll, und der Roboterarm macht das. Du hast wieder 30–40 Min. Zeit!
```
