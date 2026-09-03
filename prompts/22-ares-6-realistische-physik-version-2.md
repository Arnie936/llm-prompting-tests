# ARES-6 Disaster Rescue Spider Robot — Realistische Physik (Version 2)

```text
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
- realistic physics and collision-aware robotics behavior

REALISTIC PHYSICS REQUIREMENT (VERSION 2):
This version must not treat the robot as a purely visual demo. It must use a physics-aware interaction model for the robot, its limbs, and the environment.

Mandatory physics behavior:
- Robot limbs must not collide with or pass through each other.
- Robot limbs must not pass through the robot body, sensor mast, claw, drone dock, or other robot parts.
- The robot must not walk, slide, teleport, or animate through walls, debris, floors, columns, survivors, shelves, rocks, crates, collapsed beams, or any other environmental object.
- Feet must respect ground contact and obstacle contact. A planted foot should stay planted until a valid step target is chosen.
- Leg movement must use collision checks, reach limits, joint limits, and safe step placement instead of only decorative keyframe animation.
- The body must respond plausibly to support points, slopes, debris, and blocked paths.
- If the robot attempts an impossible movement, the system should visibly prevent it, reroute, stop, stumble, rebalance, or show a warning instead of clipping through geometry.
- Debris, objects, and the claw must interact through collision-aware grabbing and placement. No object should visually phase through the claw, robot, or world.
- The drone must launch, orbit, and return without passing through the robot or surrounding obstacles.
- Use bounding boxes, bounding spheres, raycasting, capsule/cylinder approximations, inverse kinematics constraints, or a browser physics engine such as Rapier, Cannon-es, or Ammo.js if useful.
- The simulation does not need industrial-grade robotics accuracy, but it must be physically believable and explicitly collision-safe.

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
Prioritize a working, interactive, visually impressive prototype that also enforces real collision-aware physics.
The goal is not a fake visual-only demo.
The goal is a convincing, clickable, zero-shot robot simulation where ARES-6 physically interacts with itself and its environment: no limb clipping, no walking through objects, and no pass-through motion.
```
