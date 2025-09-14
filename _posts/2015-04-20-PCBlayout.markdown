---
title:  "Design the PCB layout"
subtitle: "your manufacturable blueprint"
author: "Npv"
avatar: "https://png.pngtree.com/png-vector/20241123/ourmid/pngtree-magical-book-world-illustration-png-image_14551987.png"
image: "https://as2.ftcdn.net/v2/jpg/16/00/96/27/1000_F_1600962790_POzvDH9jX007aEjx8K2bvK1q0uN6JdQw.jpg"
date:   2015-04-20 12:12:12
---



#### 1. Design the PCB layout in the PCB Editor (Pcbnew)
*   From the main project window, double-click the `.kicad_pcb` file to open the PCB Editor.
*   **Update the PCB from the schematic:** Click **Tools > Update PCB from Schematic**. Your components will appear on the workspace.
*   **Place components:** Drag the components to your desired layout. Arrange them to simplify the wiring.
![KiCad Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQNDbQ6z31t0TSca9JuB4wq0FopN2i6Ptuyzg&s)
*   **Draw the board outline:**
    *   Select the `Edge.Cuts` layer from the layer manager on the right side of the screen.
    *   Use the **Add graphic line** tool to draw a box around your components.
*   **Draw tracks (routing):**
    *   Click the **Route tracks** tool or press **W**.
    *   Follow the "ratsnest" (thin white lines) to connect the component pins.
*   **3D viewer (optional):** To see a 3D model of your finished board, click **View > 3D Viewer**.
