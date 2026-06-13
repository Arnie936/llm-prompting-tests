# Prompting Tests für LLMs

17 anspruchsvolle Prompts zum Testen von LLMs, Coding Agents und agentischen Modellen.

---

## 1. Bienenstock-Simulation

```text
Erstelle eine visuell überzeugende, interaktive Simulation eines Bienenstocks als eigenständige HTML-Datei mit integriertem HTML, CSS und JavaScript.

Die Simulation soll nicht nur dekorativ sein, sondern ein kleines System modellieren:

- Ein wachsender Bienenstock mit hexagonalen Zellen, die dynamisch aufgebaut werden
- Unterschiedliche Rollen für Bienen: Arbeiterinnen, Sammlerinnen, Brutpflege
- Bienen sollen sichtbare Pfade zwischen Brutbereich, Honigspeicher, Eingang und Nahrungsquellen nutzen
- Nektar, Pollen und Wasser sollen als getrennte Ressourcen existieren
- Honig soll nur entstehen, wenn die nötigen Prozessschritte logisch durchlaufen wurden
- Brut soll Entwicklungsphasen haben: Ei → Larve → Puppe → erwachsene Biene
- Die Kolonie soll auf Umweltfaktoren reagieren: Wetter, Blütenverfügbarkeit, Temperatur, Räuber-/Krankheitsdruck

Interaktive Steuerung:

- Slider für Koloniegröße, Ressourcenverfügbarkeit, Wetterstabilität und Krankheitsdruck
- Buttons für Pause, 2x Geschwindigkeit, Reset und Stress-Test
- Einblendbare Layer für Bienenpfade, Temperaturzonen und Ressourcenflüsse

Visualisierung:

- Farbcodierte Wabenzellen je nach Zustand: leer, Brut, Pollen, Nektar, Honig
- Kleine Statistik-Panels für Population, Brut, Honigvorrat, Effizienz und Sterblichkeit
- Tooltips oder Inspektor beim Klick auf einzelne Wabenzellen

Anforderungen:

- Alles in einer einzigen HTML-Datei
- Keine externen Assets oder Frameworks
- Der Code soll gut strukturiert sein
- Füge im Code einen kurzen Abschnitt "Design decisions" ein, in dem du die Systemlogik erklärst
- Baue am Ende eine kleine Selbstprüfung ein: Prüfe beim Start, ob Rendering, Simulationstakt und UI funktionieren, und zeige einen kurzen Status an
```

---

## 2. 3D-Motorrad-Rennspiel

```text
Erstelle ein 3D-Motorrad-Rennspiel als eigenständige HTML-Datei mit HTML, CSS und JavaScript.

Das Spiel soll durch eine bewaldete Strecke führen und folgende Features haben:

- Fahrbare Motorradsteuerung mit Beschleunigung, Bremsen, Trägheit, Kurvenverhalten und Drift-Tendenz
- Boost-Zonen, die physikalisch nachvollziehbar die Geschwindigkeit erhöhen
- Kollisionsphysik mit Bäumen, Felsen, Streckenbegrenzungen und einfachen Gegnern
- Mindestens 3 Runden mit Rundenzeitmessung
- Einfache KI-Gegner, die der Strecke folgen und Fehler machen können
- Unterschiedliche Streckenabschnitte: Wald, Matsch, Sprungschanze, enge Kurven
- Oberflächen sollen Einfluss auf Grip und Geschwindigkeit haben

UI/HUD:

- Tacho, Rundenzähler, aktuelle Position, Boost-Anzeige, Schadensanzeige
- Start-Countdown
- Pause-Menü und Neustart-Funktion
- Minimap der Strecke

Extra-Anforderung:

- Baue ein kleines Debug-Overlay ein, das auf Wunsch FPS, Geschwindigkeit, Kollisionsstatus und Checkpoint-Status zeigt

Technische Anforderungen:

- Alles in einer einzigen HTML-Datei
- Keine externen Assets
- Muss direkt im Browser startbar sein
- Schreibe sauberen, modularen Code
- Dokumentiere kurz im Code, wie du Fahrphysik, Gegnerlogik und Kollisionen gelöst hast
```

---

## 3. First-Person-Shooter in HTML

```text
Erstelle einen spielbaren First-Person-Shooter als eigenständige HTML-Datei mit HTML, CSS und JavaScript.

Das Spiel soll enthalten:

- Echte First-Person-Steuerung mit Maus-Look und WASD
- Eine kleine, zusammenhängende 3D-Map mit mehreren Räumen und Deckungsmöglichkeiten
- Gegner mit einfacher KI: Patrouille, Verfolgung, Sichtlinie, Schießen, Respawn oder Siegbedingung
- Trefferlogik mit Projektilen oder Raycasting
- Munition, Nachladen, Lebenspunkte, Schadensfeedback
- Unterschiedliche Waffencharakteristik für mindestens 2 Waffen
- Ein kleines Zielsystem, z. B. eliminiere 10 Gegner oder erreiche den Ausgang

UI:

- Crosshair
- Ammo Counter
- Health Bar
- Trefferfeedback
- Pause-Menü mit Resume, Restart und Sensitivity

Zusätzliche Anforderungen:

- Ein funktionierendes Main Menu vor Spielstart
- Ein Optionsbereich für Maussensitivität und Schwierigkeit
- Optional ein kleines Tutorial-Overlay am Anfang
- Gegner dürfen nicht nur dumm herumstehen — sie sollen zumindest grundlegendes Verhalten zeigen

Technische Anforderungen:

- Alles in einer einzigen HTML-Datei
- Keine externen Assets oder Libraries
- Muss direkt im Browser funktionieren
- Baue eine kurze automatische Selbstdiagnose ein, die prüft, ob Pointer Lock, Rendering und Gegner-Spawn initialisiert wurden
```

---

## 4. C++ Skateboarding Game

```text
Create a complete, self-contained C++ skateboarding game in a single source file.

The game should feature:

- A late-90s California boardwalk-inspired skatepark
- A visible skateboarder character and skateboard
- Physics-based movement: acceleration, turning, gravity, friction, jumping/ollie
- Trick system: flips, spins, grabs or equivalent airborne actions
- Grinding on rails
- Combo and score system based on trick difficulty and chaining
- A follow camera that keeps the player readable
- NPC walkers and simple environmental motion to make the world feel alive
- HUD showing score, combo, speed, and controls

Additional constraints:

- No external assets required
- Must be immediately compilable and playable
- Include a simple start screen and restart flow
- Show brief trick feedback on landing
- Add at least one fail state, such as bailing or falling

Engineering requirements:

- All code in one file
- Add comments for the major systems: movement, tricks, scoring, rendering
- At the end of the file, include a short section describing known limitations and what would be improved next
```

---

## 5. Python 3D FPS Game

```text
Using Python, generate a playable 3D FPS game with the following features:

- A functional minimap showing the player and all enemies
- Visible projectile or tracer effects when shooting
- A working health bar
- A stylized menu screen with Start and Exit
- Pressing Escape must open the menu again during gameplay
- Enemy AI with at least patrol and chase behavior
- Ammo system, reload, and hit detection
- A win/lose condition

Constraints:

- Do NOT use Ursina
- Keep the implementation reasonably self-contained
- Prefer clear code structure over hacks
- The game should be actually runnable, not pseudo-code

Additions:

- Include a short diagnostic output at launch that confirms core systems initialized successfully
- Include a brief explanation of architecture choices and tradeoffs
```

---

## 6. Tower-Defense mit Balancing und Editor

```text
Erstelle ein vollständiges Tower-Defense-Spiel als eigenständige HTML-Datei mit HTML, CSS und JavaScript.

Das Spiel soll enthalten:

- Pfadbasierte Gegnerwellen
- Mindestens 4 unterschiedliche Tower-Typen mit klar unterschiedlichen Rollen
- Gegner mit verschiedenen Eigenschaften: schnell, tanky, fliegend oder resistent
- Upgrade-System für Türme
- Ökonomie-System mit Einkommen, Ausgaben und Wellenskalierung
- Sichtbare Projektil- oder Effektlogik
- Sieg- und Niederlagenzustand

Zusätzliche Schwierigkeit:

- Ein kleiner Map-Editor-Modus, in dem der Nutzer den Weg oder Tower-Plätze begrenzt anpassen kann
- Eine Balancing-Anzeige, die nach jeder Welle grob bewertet, ob die aktuelle Strategie effizient ist

Anforderungen:

- Alles in einer einzigen HTML-Datei
- Keine externen Assets
- Saubere UI mit Spielbereich, Shop, Wellensteuerung und Statuspanel
- Füge eine kurze Entwicklernotiz im Code hinzu, wie Balancing und Gegner-Skalierung umgesetzt wurden
```

---

## 7. Fabrik- und Automation-Simulation

```text
Erstelle eine interaktive 2D-Fabrik- und Produktionssimulation als eigenständige HTML-Datei mit HTML, CSS und JavaScript.

Ziel:
Der Spieler soll eine kleine Fabrik aufbauen, die Rohstoffe abbaut, transportiert und in höherwertige Produkte umwandelt.

Das Spiel soll enthalten:

- Förderbänder
- Extraktoren oder Miner
- Verarbeitungsmaschinen
- Lager
- Energie-/Stromsystem oder vergleichbare Produktionsbegrenzung
- Engpässe und Durchsatzprobleme sollen sichtbar werden
- Ein Zielsystem, z. B. produziere X Einheiten eines Endprodukts

UI/Visualisierung:

- Grid-basiertes Platzieren
- Overlay für Durchsatz oder Materialfluss
- Statistik für Input, Output, Lagerbestand und Bottlenecks
- Pause, Reset, Speed x2 / x4

Anforderungen:

- Alles in einer HTML-Datei
- Keine externen Libraries
- Im Code: kurze Dokumentation des Datenmodells und der Update-Logik
- Baue eine kleine Bottleneck-Erkennung ein, die automatisch problematische Stellen markiert
```

---

## 8. Ökosystem- und Evolution-Simulation

```text
Erstelle eine visuelle Ökosystem-Simulation als eigenständige HTML-Datei.

Die Simulation soll mindestens drei Ebenen enthalten:

- Pflanzen / Ressourcen
- Beutetiere
- Räuber

Anforderungen:

- Individuen sollen Zustände wie Energie, Alter, Reproduktion und Tod besitzen
- Populationen sollen sich dynamisch entwickeln
- Es soll ein einfaches Vererbungs- oder Mutationssystem geben, sodass sich z. B. Geschwindigkeit, Sichtweite oder Reproduktionsrate über Generationen verändern können
- Umweltfaktoren wie Trockenheit, Nahrungsknappheit oder Jahreszeiten sollen die Population beeinflussen

UI:

- Diagramme für Populationsverläufe
- Einstellbare Parameter per Slider
- Möglichkeit, einzelne Lebewesen anzuklicken und deren Eigenschaften zu inspizieren
- Buttons für Pause, Reset und beschleunigte Simulation

Technische Anforderungen:

- Alles in einer HTML-Datei
- Keine externen Assets
- Gute visuelle Lesbarkeit
- Im Code kurz erklären, welche Regeln für Reproduktion, Mutation und Nahrungsketten verwendet wurden
```

---

## 9. Echtzeit-Verkehrssimulation

```text
Erstelle eine interaktive Verkehrssimulation einer kleinen Stadt als eigenständige HTML-Datei.

Die Simulation soll enthalten:

- Straßennetz mit Kreuzungen
- Fahrzeuge, die Ziele anfahren
- Ampeln oder Vorfahrtsregeln
- Staus und Rückkopplungseffekte
- Unterschiedliche Fahrzeugtypen oder Prioritäten
- Eine einfache Fußgänger- oder Buslogik wäre ein Plus

Interaktion:

- Der Nutzer soll Ampelschaltungen oder Straßensperren ändern können
- Die Auswirkungen auf Durchfluss, Wartezeiten und Stau sollen live sichtbar werden
- Visualisierung von Durchschnittsgeschwindigkeit, Auslastung und Stau-Hotspots

Anforderungen:

- Alles in einer HTML-Datei
- Keine externen Libraries
- Gute Performance bei vielen Fahrzeugen
- Füge einen kleinen Analysemodus ein, der die kritischsten Engstellen erkennt und benennt
```

---

## 10. Orbital- und Missionssimulation

```text
Erstelle eine interaktive Orbital- und Missionssimulation als eigenständige HTML-Datei.

Inhalt:

- Eine 2D- oder 3D-Darstellung eines Planetensystems oder eines Planeten mit Mond
- Ein Raumfahrzeug, das sich mit vereinfachter Orbitalmechanik bewegt
- Möglichkeit, Schubmanöver auszuführen
- Anzeige von Geschwindigkeit, Richtung, Höhe/Distanz und verbleibendem Treibstoff
- Mindestens ein Missionsziel, z. B. Orbit erreichen, Mondvorbeiflug oder Landefenster treffen

Zusätzliche Anforderungen:

- Visualisiere Flugbahn-Prognosen
- Füge eine Missionskonsole oder Logbox hinzu
- Ein Tutorial oder kurze Missionsanweisung beim Start
- Die Simulation soll physikalisch nicht perfekt sein müssen, aber intern konsistent

Technische Anforderungen:

- Alles in einer HTML-Datei
- Keine externen Assets
- Klare Trennung zwischen Rendering, Physik und UI
- Dokumentiere im Code die verwendeten physikalischen Vereinfachungen
```

---

## 11. ComfyUI Workflow Test

```text
Du befindest dich in einem Ordner, der meine lokale ComfyUI-Installation enthält.

Aufgabe:
Erstelle einen neuen ComfyUI-Workflow, der ein lokal vorhandenes FLUX-Modell verwendet. Verwende bevorzugt ein kleines/schnelles FLUX-Modell, falls mehrere vorhanden sind, z. B. ein Modell mit Namen wie "flux", "schnell", "dev", "fp8", "gguf" oder ähnlich.

Wichtig:

- Untersuche zuerst die Ordnerstruktur.
- Finde heraus, wo Checkpoints, Modelle, VAE/Text-Encoder, ControlNets und Workflows gespeichert sind.
- Verwende keine externen Downloads.
- Verschiebe oder lösche keine bestehenden Dateien.
- Orientiere dich am Format vorhandener Workflow-Dateien, falls welche existieren.
- Erstelle einen einfachen, funktionierenden Text-to-Image-Workflow mit:
  - Prompt-Eingabe
  - FLUX-Modell
  - Sampler
  - Bildgenerierung
  - Save-Image-Node
- Falls ControlNet sinnvoll lokal verfügbar ist, füge optional eine deaktivierte ControlNet-Gruppe hinzu, aber der Workflow muss auch ohne ControlNet funktionieren.

Speichere den neuen Workflow dort, wo die anderen Workflows liegen, unter dem Namen:

"dein test.json"

Nach dem Speichern:

- Prüfe, ob die JSON-Datei gültig ist.
- Prüfe, ob alle referenzierten lokalen Modelldateien existieren.
- Gib mir eine kurze Zusammenfassung:
  1. Welches Modell wurde verwendet?
  2. Wo wurde der Workflow gespeichert?
  3. Welche Annahmen hast du getroffen?
  4. Gibt es Einschränkungen?
```

---

## 12. n8n Gmail Sponsoring Workflow Test

```text
Du befindest dich in einem Ordner, der zu meiner lokalen n8n-Installation gehört.

Aufgabe:
Erstelle einen importierbaren n8n-Workflow als JSON-Datei.

Der Workflow soll Folgendes machen:

Immer wenn eine neue E-Mail über Gmail eingeht:

1. Die E-Mail wird analysiert.
2. Es wird entschieden, ob es sich wahrscheinlich um eine Sponsoring-/Kooperationsanfrage handelt.
3. Wenn es Sponsoring ist:
   - Erstelle eine höfliche Antwort mit sinngemäß:
     "Vielen Dank für die Anfrage, aktuell besteht kein Interesse. Alles Gute."
   - Antworte auf die ursprüngliche E-Mail.
4. Wenn es kein Sponsoring ist:
   - Markiere die E-Mail als wichtig oder füge ein Label wie "Wichtig" hinzu.

Anforderungen:

- Untersuche zuerst die Ordnerstruktur.
- Prüfe, ob bereits n8n-Workflow-Exports vorhanden sind, und orientiere dich an deren Format.
- Falls keine Workflow-Exports vorhanden sind, erstelle eine saubere importierbare n8n-Workflow-JSON-Datei in einem sinnvollen Ordner, z. B. "./workflows" oder "./exports".
- Nenne die Datei:

"dein-test-gmail-sponsoring-workflow.json"

Technische Anforderungen:

- Verwende einen Gmail Trigger.
- Verwende einen LLM- oder Klassifizierungs-Schritt, um Sponsoring zu erkennen.
- Verwende klare Kriterien für Sponsoring, z. B. Wörter wie "sponsor", "partnership", "collaboration", "brand deal", "paid promotion", "Kooperation", "Werbung", "Produktplatzierung".
- Verwende eine If-/Switch-Logik für die Entscheidung.
- Verwende Gmail Reply für Sponsoring-Mails.
- Verwende Gmail Label/Important für normale Mails.
- Credentials dürfen nicht erfunden werden. Nutze Platzhalter oder vorhandene Credential-Referenzen, falls diese aus bestehenden Workflows eindeutig hervorgehen.
- Keine bestehenden Dateien löschen oder überschreiben, außer es gibt bereits exakt diese Testdatei.

Sicherheitsanforderung:

- Baue zusätzlich einen "Dry Run"-Schalter ein.
- Wenn Dry Run aktiv ist, soll keine echte Antwort gesendet werden, sondern nur geloggt werden, was passieren würde.
- Standardmäßig soll Dry Run aktiviert sein.

Zusätzliche Entscheidungslogik:

- Der Workflow soll Sponsoring-Mails nicht sofort ablehnen, wenn die Mail Wörter wie "budget", "paid", "long-term", "sponsored video" oder einen Betrag enthält.
- In diesem Fall soll die Mail stattdessen mit dem Label "Sponsoring prüfen" markiert werden.
- Nur offensichtliche Low-Quality-Sponsoring-Mails sollen automatisch abgelehnt werden.

Nach dem Speichern:

- Prüfe, ob die JSON-Datei valide ist.
- Gib mir eine kurze Zusammenfassung:
  1. Wo wurde der Workflow gespeichert?
  2. Welche Nodes wurden verwendet?
  3. Wie wird Sponsoring erkannt?
  4. Wie kann ich Dry Run deaktivieren?
  5. Welche Credentials muss ich in n8n noch verbinden?
```



## 13. ARES-6: ein sechsbeiniger Katastrophen-Roboter, der durch ein eingestürztes Lagerhaus krabbelt, Menschen scannt, Trümmer hebt, eine Mini-Drohne startet und bei Systemfehlern sichtbar ausrastet.

````text
You are an expert full-stack creative coding agent.

Your task is to build a complete interactive 3D browser simulation from scratch.

Do not use external paid assets.
Do not require the user to manually download 3D models.
Create everything procedurally with code unless absolutely necessary.
The final result must run locally in a browser.

PROJECT TITLE:
ARES-6 Disaster Rescue Spider Robot — Interactive Robotics Simulation

GOAL:
Create a cinematic, interactive, technical 3D robot simulation that feels like a real robotics test interface.

This should be impressive enough to be used as a YouTube demo showing what an LLM can build zero-shot.

The project should be a hard test for an LLM because it requires:
- 3D modeling
- UI design
- procedural robot construction
- animation systems
- interactive controls
- simulated sensors
- mission scenarios
- state management
- clean code architecture
- visual polish
- performance awareness

CORE CONCEPT:
ARES-6 is a six-legged disaster rescue robot designed for collapsed buildings, tunnels, warehouses, mines, and industrial accidents.

The robot can:
- walk with six mechanical legs
- lower and raise its body
- crawl under obstacles
- rotate its sensor head
- extend a camera mast
- scan for survivors
- detect heat signatures
- lift debris with a robotic claw
- launch a small scout drone
- enter different mission modes
- show telemetry in a technical dashboard

The app should not look like a toy.
It should look like a robotics lab prototype demo.

VISUAL STYLE:
- Dark cinematic robotics interface
- Black / dark grey background
- Technical dashboard UI
- Glowing sensor effects
- Yellow emergency markings on robot parts
- Industrial rescue aesthetic
- Floor grid
- Subtle fog or atmospheric depth if possible
- High contrast
- Serious, technical, not cartoonish
- Looks good in a YouTube thumbnail

MAIN SCREEN LAYOUT:
Create a full-screen web app with:

1. Center:
Interactive 3D viewport showing the robot and environment.

2. Left panel:
Robot controls.

3. Right panel:
Telemetry, mission data, sensor readouts, system status.

4. Top bar:
Project title and mode indicator.

5. Bottom bar:
Timeline / mission log / current command feedback.

3D SCENE REQUIREMENTS:
The scene must include:
- A ground grid
- A small disaster test environment
- Broken concrete blocks
- Metal beams
- A tunnel opening or collapsed wall section
- A small human heat-signature target represented abstractly, not graphically
- The ARES-6 robot in the center
- Optional dust particles, scan lines, or subtle lighting effects

ROBOT DESIGN:
Build the robot procedurally using 3D primitives.

Robot components:

1. Central Body
- Low, armored central chassis
- Rounded rectangular or box-based body
- Yellow rescue stripes
- Status LEDs
- Front sensor head
- Rear battery / power unit

2. Six Legs
The robot must have six legs:
- Front left
- Middle left
- Rear left
- Front right
- Middle right
- Rear right

Each leg should have:
- Hip joint
- Upper leg segment
- Knee joint
- Lower leg segment
- Ankle / foot joint
- Foot pad

Each leg should be visually mechanical:
- Cylinders for joints
- Rectangular or cylindrical limb segments
- Small hydraulic pistons if possible
- Foot pads that touch the ground

3. Sensor Head
- Rotating head on front or top
- Camera lens
- Lidar sensor
- Thermal sensor
- Search light

4. Camera Mast
- Telescopic mast that can extend upward
- Small camera module at the top
- Mast height must be controllable

5. Robotic Arm
- Mounted at the front
- Shoulder joint
- Elbow joint
- Wrist joint
- Two-finger claw
- Can open and close
- Can move toward debris

6. Scout Drone
- Small drone docked on the robot’s back
- Button to launch drone
- Drone rises, hovers, circles the robot, then returns
- Use simple shapes if needed

INTERACTION REQUIREMENTS:
The user must be able to rotate, zoom, and pan the 3D camera.

Use mouse controls:
- Left drag: orbit camera
- Scroll: zoom
- Right drag or shift-drag: pan, if supported

CONTROL PANEL REQUIREMENTS:

Create a left-side control panel with these sections:

SECTION 1: Robot State
- Button: Reset Simulation
- Button: Zero Pose
- Button: Emergency Shutdown
- Button: Reboot Systems
- Toggle: Autonomous Mode
- Toggle: Show Debug Frames
- Toggle: Show Wireframe
- Toggle: Show Sensor Cones

SECTION 2: Body Controls
- Slider: Body Height, range 0.25 to 1.1 meters
- Slider: Body Yaw, range -180 to 180 degrees
- Slider: Body Pitch, range -30 to 30 degrees
- Slider: Body Roll, range -30 to 30 degrees
- Button: Low Crawl Pose
- Button: High Clearance Pose
- Button: Stable Rescue Pose

SECTION 3: Locomotion
- Button: Start Walk Cycle
- Button: Stop Walk Cycle
- Button: Crawl Forward
- Button: Rotate In Place
- Button: Obstacle Climb Demo
- Slider: Walk Speed, range 0 to 100%
- Slider: Step Height, range 0 to 100%

The walk cycle should animate the six legs in an alternating tripod gait:
- Front left, middle right, rear left move together
- Front right, middle left, rear right move together
The motion does not need to be physically perfect, but it must visually communicate spider-like robotic walking.

SECTION 4: Individual Leg Control
Allow selecting one of the six legs.

For the selected leg provide:
- Slider: Hip Rotation
- Slider: Knee Bend
- Slider: Ankle Angle
- Button: Lift Foot
- Button: Plant Foot
- Button: Reset Leg

SECTION 5: Robotic Arm
- Slider: Shoulder Angle
- Slider: Elbow Angle
- Slider: Wrist Rotation
- Button: Open Claw
- Button: Close Claw
- Button: Grab Debris Demo
- Button: Release Debris

The grab debris demo should:
- Move the arm toward a small debris object
- Close the claw
- Lift the debris slightly
- Move it aside
- Release it

SECTION 6: Sensors
- Slider: Sensor Head Yaw
- Slider: Sensor Head Pitch
- Slider: Camera Mast Height
- Toggle: Lidar Scan
- Toggle: Thermal Scan
- Toggle: Search Light
- Button: Survivor Scan
- Button: Mark Target

Sensor visualizations:
- Lidar scan: rotating transparent cone, ring, or sweeping line
- Thermal scan: glowing colored highlight around the hidden target
- Search light: visible cone or beam from sensor head
- Survivor scan: animated progress bar and result in telemetry panel

SECTION 7: Scout Drone
- Button: Launch Drone
- Button: Recall Drone
- Toggle: Drone Camera Feed
- Slider: Drone Orbit Radius

Drone behavior:
- Starts docked on the robot
- Launches upward
- Hovers
- Orbits the robot
- Returns to dock when recalled

SECTION 8: Mission Presets
Create buttons:
- Mission: Tunnel Inspection
- Mission: Collapsed Warehouse
- Mission: Survivor Search
- Mission: Debris Removal
- Mission: System Failure Test

Each mission preset should change:
- Robot pose
- Active sensors
- UI status text
- Environment highlight
- Mission log messages

RIGHT TELEMETRY PANEL REQUIREMENTS:
Create a right-side panel showing live simulated data:

1. System Status
- Power level
- Motor temperature
- Hydraulic pressure
- CPU load
- Signal strength
- Damage level
- Current mode

2. Sensor Data
- Lidar active/inactive
- Thermal active/inactive
- Search light active/inactive
- Survivor probability
- Distance to target
- Obstacle density

3. Leg Status
Show all six legs with status:
- grounded
- lifting
- moving
- error
- idle

4. Mission Log
Show timestamped messages like:
- “ARES-6 initialized”
- “Lidar sweep started”
- “Thermal anomaly detected”
- “Possible survivor located”
- “Debris removal sequence started”
- “Drone launched”
- “Warning: left middle leg torque spike”

5. Mini Map
Create a simple 2D top-down minimap if possible:
- Robot position
- Debris blocks
- target marker
- drone position
This can be simple SVG, canvas, or HTML/CSS.

SYSTEM FAILURE TEST:
The “System Failure Test” mission must demonstrate that the simulation has meaningful state.

When activated:
- One leg should show a warning state
- Telemetry should show motor temperature rising
- Mission log should show warnings
- Robot movement should become slightly unstable
- Warning lights should blink
- A “Rebalance” or “Auto Stabilize” action should appear or become enabled

Add a button:
- Auto Stabilize

When clicked:
- Body returns to stable pose
- Warning decreases
- Leg status returns to normal
- Mission log confirms stabilization

ANIMATION REQUIREMENTS:
Implement smooth animations for:
- walking cycle
- body height changes
- mast extension
- sensor head rotation
- lidar scan sweep
- search light activation
- claw open/close
- debris grabbing
- drone launch/orbit/recall
- system warning blinking
- mission preset transitions

Use requestAnimationFrame or the animation system of the chosen 3D library.

TECHNICAL REQUIREMENTS:
Use:
- HTML
- CSS
- JavaScript
- Three.js or an equivalent browser 3D library

Preferred:
- A single self-contained project
- Clear file structure if multiple files are used
- No build step unless necessary
- Runs by opening index.html or using a simple local server

Code architecture should include:
- Scene setup
- Robot factory / robot builder
- Leg module
- Arm module
- Sensor module
- Drone module
- UI controller
- State manager
- Animation loop
- Mission system
- Telemetry simulator

IMPORTANT:
The robot must be built as a hierarchy of objects so joints rotate correctly.

Example hierarchy:
- robotRoot
  - body
  - leg_FL
    - hipJoint
      - upperLeg
        - kneeJoint
          - lowerLeg
            - ankleJoint
              - foot
  - leg_ML
  - leg_RL
  - leg_FR
  - leg_MR
  - leg_RR
  - armRoot
  - sensorHead
  - mast
  - droneDock

UI QUALITY REQUIREMENTS:
The interface must look polished.

Use:
- Dark background
- Thin borders
- Small technical labels
- Monospace font for telemetry
- Clean sliders
- Highlighted active buttons
- Warning colors for errors
- Compact layout
- Responsive enough for 16:9 recording

The app should look good at 1920x1080.

YOUTUBE DEMO REQUIREMENTS:
The final simulation should have at least 5 “wow moments”:
1. Six-legged walking animation
2. Lidar / thermal scan visualization
3. Robotic claw picking up debris
4. Drone launch and orbit
5. System failure and auto-stabilization

Make these moments clearly visible and easy to trigger with buttons.

Do not hide the impressive features deep in the UI.

ACCEPTANCE CRITERIA:
The project is successful only if:

- The app opens in a browser
- The robot is visible in 3D
- The robot clearly has six legs
- The user can orbit the camera
- Sliders visibly move robot parts
- Walk cycle works
- Sensor effects are visible
- The claw can open and close
- The debris grab demo works
- The drone can launch and return
- Mission presets change the robot state
- Telemetry updates live
- The system failure test creates visible warnings
- Auto stabilize visibly fixes the failure state
- The UI looks like a serious robotics dashboard
- The code is organized and understandable

OUTPUT FORMAT:
Return the complete project code.

If using multiple files, provide:
- index.html
- styles.css
- main.js
- any additional JavaScript modules

Also explain briefly:
- how to run it
- which controls create the main demo moments
- any limitations or simplifications

Do not provide only pseudocode.
Do not provide a partial implementation.
Do not say “this is too complex.”
Build the best complete version possible in one shot.

FINAL NOTE:
Prioritize a working, interactive, visually impressive prototype over perfect robotics physics.
The goal is not scientific accuracy.
The goal is a convincing, clickable, zero-shot robot simulation demo.
````

---

## 14. Photoshop Klon

````text
Build a fully functional, standalone image editor inspired by Photoshop.

The final output must be a single self-contained HTML file that runs locally in the browser without any backend.

Do not use Adobe branding, logos, names, or copyrighted UI assets. Call the app:

"PixelForge Studio"

## Final Deliverable

Create one file:

index.html

The file must include:
- HTML
- CSS
- JavaScript
- All app logic
- No backend
- No build step
- No required external API keys
- No server required

The user should be able to open the file directly in a browser and use the app.

## Core Outcome

The app must feel like a real image editor, not a static demo.

It should support:

1. Canvas-based editing
2. Image import
3. Layers
4. Drawing tools
5. Selection tools
6. Text tool
7. Shape tools
8. Basic filters
9. Undo/redo
10. Export as PNG/JPEG
11. A professional dark UI similar to modern creative tools

## UI Requirements

Create a polished dark interface with:

- Top menu bar
- Left vertical toolbar
- Central canvas workspace
- Right sidebar for:
  - Layers
  - Properties
  - Filters
- Bottom status bar
- Floating canvas area with checkerboard transparency background
- Zoom controls
- Tool-specific settings panel

The UI should look premium, clean, and professional.

Use CSS only. No images required for UI icons unless created with CSS/Unicode/SVG inline.

## Layout

The app layout should contain:

### Top Bar

Include menu buttons:

- File
- Edit
- Image
- Layer
- Select
- Filter
- View
- Help

Under File, support:
- New Project
- Open Image
- Export PNG
- Export JPEG
- Clear Project

### Left Toolbar

Include tools:

- Move Tool
- Brush Tool
- Eraser Tool
- Rectangle Select Tool
- Lasso Select Tool
- Crop Tool
- Text Tool
- Rectangle Shape Tool
- Circle Shape Tool
- Line Tool
- Eyedropper Tool
- Fill Bucket Tool
- Zoom Tool
- Hand/Pan Tool

Each tool should be clickable and visually show active state.

### Center Workspace

The center area must contain:

- Main canvas
- Transparent checkerboard background
- Zoomable workspace
- Pan support
- Canvas boundary shadow
- Rulers optional but nice

### Right Sidebar

Create panels:

#### Layers Panel

Each layer should show:
- Layer name
- Visibility toggle
- Active layer highlight
- Opacity slider
- Blend mode dropdown
- Delete layer button
- Duplicate layer button
- Move layer up/down buttons

Layer support must include:
- Add new layer
- Delete layer
- Rename layer
- Reorder layers
- Hide/show layers
- Change opacity
- Merge visible layers

#### Properties Panel

Show current tool settings.

Brush:
- Size
- Color
- Opacity
- Hardness

Eraser:
- Size
- Opacity

Text:
- Font size
- Font family
- Color
- Bold/italic toggle

Shapes:
- Fill color
- Stroke color
- Stroke width

#### Filters Panel

Add buttons for:

- Grayscale
- Invert
- Sepia
- Brightness
- Contrast
- Blur
- Sharpen
- Pixelate
- Noise
- Vignette

Filters should apply to the active layer only.

## Functional Requirements

### 1. New Project

User can create a new blank project.

Default:
- Width: 1280
- Height: 720
- Transparent background

Allow custom size through a modal.

### 2. Image Import

User can upload an image from local disk.

The image should:
- Be placed on a new layer
- Fit inside the canvas while preserving aspect ratio
- Be editable afterwards

### 3. Layers

Implement real layer compositing.

Each layer should internally be its own canvas or image buffer.

The final visible image should be composed onto the main display canvas.

Required layer properties:

```js
{
  id: string,
  name: string,
  canvas: HTMLCanvasElement,
  ctx: CanvasRenderingContext2D,
  visible: boolean,
  opacity: number,
  blendMode: string,
  x: number,
  y: number,
  locked: boolean
}
```
````

---

## 15. Interaktiver 3D-digitaler Zwilling der Erde

```text
Baue einen vollständig interaktiven 3D-digitalen Zwilling der Erde mit folgenden Funktionen:

Nutzer sollen nahtlos vom Weltraum bis hinunter zu einzelnen Stadtstraßen zoomen können.

Wenn ich mit der Maus über ein Land fahre, soll die Ländergrenze hervorgehoben werden und ein Popup erscheinen, das Statistiken wie Fläche, Bevölkerung und BIP anzeigt.

Zeige einen realistischen Planeten Erde mit Schaltern für atmosphärische Wolkendecke, Flugverkehr und Tag/Nacht. Der Nachtmodus soll Stadtlichter anzeigen.

Verwende kostenlose öffentlich verfügbare Assets, Modelle und Layer, falls nötig. Stelle sicher, dass es effizient in einem normalen Webbrowser lädt.
```


---

## 16. Dragomon Monster-Catching-RPG

```text
Erstelle ein spielbares Monster-Catching-RPG namens „Dragomon“. Das Spiel soll von klassischen Monster-Sammel-Abenteuern und energiegeladenen Shōnen-Kampfkunst-Animes inspiriert sein, aber komplett eigene Charaktere, Kreaturen, Namen, Designs und Welten verwenden.

Spieler sollen eine offene Welt erkunden, wilde Kreaturen in hohem Gras finden, sie fangen, trainieren und in rundenbasierten Kämpfen einsetzen können. Es soll Trainer geben, gegen die man kämpft, ein Levelsystem, Fähigkeiten, Entwicklungen, Items, Heilzentren, verschiedene Gebiete, Quests und ein Ziel, bei dem man stärker wird und die besten Dragomon-Trainer herausfordert.

Der Stil soll dynamisch, farbenfroh und actionreich sein: mit Energie-Auren, Martial-Arts-inspirierten Angriffen, humorvollen Charakteren und dramatischen Kampfeffekten. Keine geschützten Figuren, Namen, Logos oder Designs aus bestehenden Franchises verwenden.
```

---

## 17. Auditierter selbstverbessernder Trading-Research-Agent

Ein umfangreicher Master-Prompt für einen Coding Agent, der ein auditierbares, selbstverbesserndes Trading-Forschungssystem aufbaut, testet, im Paper-Modus bereitstellt und an einen lokalen Operator übergibt. Der Prompt enthält harte Sicherheitsgrenzen, Strategie-Recherche, Backtesting, externe Beobachtung, Railway-Deployment und eine ausdrücklich gesperrte Live-Phase.

[Vollständigen deutschen Prompt öffnen](prompts/17-auditierter-selbstverbessernder-trading-research-agent.md)
