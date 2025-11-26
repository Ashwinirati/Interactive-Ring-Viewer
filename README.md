💍 Interactive Jewellery 3D Ring Viewer

This project is a web-based 3D jewellery showcase built using A-Frame (WebGL). Users can click on any of the three rings to bring it up for inspection, rotate it, and then close it to return it back to the box.

🎯 Features

3 interactive 3D ring models

Click to focus (ring moves up and scales larger)

Drag to rotate (while focused)

Click Close to return

Smooth animations

Only one ring can be active at a time

Responsive for mouse and touch

Realistic lighting and material reflections (PBR-style)

🛠 Technologies Used

A-Frame

JavaScript

GLB 3D Models

WebGL

PBR lighting with dynamic lights

🧱 Project Structure
index.html
assets/
  ring1.glb
  ring2.glb
  ring3.glb
README.md

🧩 Key Components
ring-focus-multi

Handles the logic for bringing a clicked ring forward and scaling it.

close-ring-global

Detects the Close button click and returns the ring back to the box.

drag-rotate

Enables ring rotation via mouse/touch drag, only when focused.

🧠 Interaction Logic (High-Level Explanation)

When a ring is clicked:

It emits focusring

Moves up and forward

Enlarges

Enables rotation

Shows Close button

When Close is clicked:

Emits unfocusring

Moves ring back to its slot

Hides Close button

Resets rotation

💡 Rendering & Lighting

The scene uses:

renderer="colorManagement: true; physicallyCorrectLights: true"


Lighting setup:

Ambient light

Directional light

Two point lights

This enhances metallic reflections and adds realistic highlights to the rings.

🧪 Edge Handling

activeRing & busy prevent multiple rings from being focused at once

Drag rotation only works when focused

Animation events control interaction timing

📦 How to Run

Put project folder inside a local web server

Start server (for example using VS Code Live Server)

Open in browser:

http://127.0.0.1:5500/index.html


👤 Developed by

Ashwini Rati
BCA Student