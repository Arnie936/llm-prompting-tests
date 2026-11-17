# Faltbare Drohne in FreeCAD aus einem Paper

Voraussetzung: Claude Code mit FreeCAD 1.x (per Python steuerbar). Im Ordner `referenzen/` liegt das Paper „The Foldable Drone: A Morphing Quadrotor that can Squeeze and Fly“ (Falanga et al., 2018) als PDF.

```text
In Referenzen liegt eine PDF. Bau die Drohne daraus bitte in FreeCAD nach. Du hast maximal 55 Minuten Zeit. Soll eine coole Demo sein.

Das muss am Ende drin sein:

1. Modell: Zentralkörper mit Servos, Akku und Elektronik, vier Arme mit Motoren, Propellern und Landebeinen. Halte die Maße aus dem Paper ein, wo es welche gibt (Spannweite, Propeller, Höhenversatz der Arme). Alles, was du nur aus Fotos ableitest, kennzeichnest du als geschätzt.

2. Faltbar wie im Paper: Die vier Armwinkel stehen in einer Tabelle "Params" und treiben das ganze Modell parametrisch. Die vier Konfigurationen aus dem Paper (X, H, O, T) müssen sich damit einstellen lassen. Wenn du von den Winkeln im Paper abweichen musst, zum Beispiel wegen Servo-Grenzen oder Kollisionen, begründe das.

3. Vorführ-Starter fürs Video: eine Datei zum Doppelklicken, die FreeCAD mit der Drohne öffnet und ein Panel mit großen Buttons X, H, O, T und „Alle abspielen“ zeigt. Die Arme klappen animiert in die jeweilige Konfiguration. Das Modell muss sich mit der Maus frei drehen lassen (im 3D-Fenster ziehen, nicht nur über den Navigationswürfel), und die Demo arbeitet auf einer Kopie, damit das Original unverändert bleibt. Verstell keine globalen FreeCAD-Einstellungen, oder stell sie danach wieder her.

4. Ausgaben in "output": die FCStd-Datei, ein STEP-Export, ein Hero-Render, ein Übersichtsbild aller vier Konfigurationen, ein GIF der Faltung und ein JSON-Report mit Maßen und Prüfergebnissen. Die Skripte, die Modell und Renders erzeugen, liegen in "scripts".

5. Prüfen: Alle Teilkörper müssen gültig sein. Öffne die Datei neu und kontrolliere, dass alle vier Konfigurationen korrekt aussehen. Sag ehrlich, was du nicht geprüft hast.

6. Abschlussbericht: wie ich das Modell in einem Video in wenigen Schritten vorführe, eine Tabelle mit den Winkeln für X, H, O und T, und eine ehrliche Einschätzung, ob man das so mit dem 3D-Drucker ausdrucken kann und ob es dann fliegen würde. Falls nicht, was dafür fehlt.
```
