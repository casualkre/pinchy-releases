---
title: "CAD: parts to print and boards to order"
description: "A **CAD** item in the Reef is either a **3D part** (to 3D print, or to send to another CAD program) or a **circuit board** (to order from a board maker like PCBWay or JLCPCB). Make one with **New → CAD** in a space, or just ask: Pinchy, your agents and krill make them with the same tools you see."
keywords: "cad, 3d, 3d print, 3d printing, printer, stl, 3mf, step, freecad, kicad, pcb, circuit board, board, electronics, gerber, gerbers, pcbway, jlcpcb, order a board, bom, pick and place, assembly, solder, enclosure, case, box, part, design a part, route, autoroute, footprint, mounting holes"
permalink: /cad/
---
# CAD: parts to print and boards to order

A **CAD** item in the Reef is either a **3D part** (to 3D print, or to send to another CAD program) or a **circuit board** (to order from a board maker like PCBWay or JLCPCB). Make one with **New → CAD** in a space, or just ask: Pinchy, your agents and krill make them with the same tools you see.

## What to ask for
- "Design a tiny board: a USB-C socket, a 330 Ω resistor and a green LED, about 25 × 15 mm with two mounting holes. Build it so I can order it."
- "Make a 3D-printable case for that board: 1.5 mm walls, rounded corners, a slot for the plug."
- "Make the wall 2 mm and build it again."

## A 3D part
- On the left: **Parameters** (numbers you tune, like `wall` or `width`) and **Shapes** (boxes, cylinders, spheres, rings, extrusions, turned profiles). A **Cut** takes the other shapes out of the first one: that is how holes, slots and hollows are made.
- Any size can be a number or a parameter: `w`, `wall*2`, `(w - 4)/2`. Change a parameter and every shape that uses it follows.
- Drag the 3D view to turn it, scroll to zoom, right-drag to move. The buttons below it show it from the front, the top and the side.
- **Build** makes an **STL** and a **3MF** for your printer (3MF keeps the colours), and a **STEP** for other CAD programs when FreeCAD is installed. A printing guide (settings, how much filament) is written as a document in the same space.

## A circuit board
- **Parts** are placed by their real KiCad footprint names (Pinchy looks them up for you); **Nets** say which pins are wired together.
- **Route** draws the copper tracks on both sides by itself, with vias where it needs to change side. You can move parts and route again. If something doesn't fit, it says which connection and why.
- **Check** finds unconnected pins, parts off the board, overlaps.
- **Build** (with KiCad installed) runs KiCad's own design check, fills the ground copper, and makes everything the board maker asks for in one zip: Gerbers and drill files, the parts list (BOM) and the pick-and-place file for their assembly service. You also get a STEP model and a 3D picture of the board with its parts (the **3D (KiCad)** tab).
- An **assembly guide** lands in the same space: what to order, what to solder first, a picture of where each part goes, and which parts have a direction.

## KiCad and FreeCAD
Both are free. Without them you still get the pictures, routing, checks, STL/3MF, the parts list and a KiCad project. KiCad adds the fab files and its design check; FreeCAD adds STEP files and rounded edges on any shape. The chip at the top of a CAD item says what is missing; click it to install (about 1 GB, only when you click). On the away server they are installed by hand.

## On the phone
A CAD item shows its picture and size. To change it, ask a krill from the item.

## Settings
- Settings → Safety & data → Backup & move: CAD items and their built files are part of a backup, like every space.
- Settings → Agents & automation → Away server: CAD items sync with your away server, and krill there can design and route; fab files need KiCad installed on that server.

## Not yet
Schematic drawings, boards with more than two copper layers, and very dense boards (the router tells you what didn't fit).

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
