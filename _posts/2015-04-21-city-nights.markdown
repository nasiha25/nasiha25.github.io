---
title:  "a simple circuit to draw in kicad."
subtitle: " making a blueprint for your PCB"
author: "Npv"
avatar: "https://png.pngtree.com/png-vector/20241123/ourmid/pngtree-magical-book-world-illustration-png-image_14551987.png"
image: "http://t1.gstatic.com/images?q=tbn:ANd9GcSE2nmUPARpIqQty8ClspP-x1oAmB9O71BL8xsn5jp4-S19zL1SJ2lk_2aEfZVnIOSy8oeEmfM7"
date:   2015-04-21 12:12:12
---

###  single LED circuit
For a simple KiCad project, a single LED circuit is an excellent starting point. This circuit introduces the core KiCad workflow—creating a schematic, assigning footprints, and designing a basic PCB layout—with minimal components. 

### Components needed:
1 x Resistor (R)
1 x LED (D)
1 x Voltage source (VDC)
1 x Ground symbol (GND).

![KiCad Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTLq_i7n6jnYAde6foaEchHFzb_eFDN6dUGXw&s)

*Note: In KiCad, you would use a `VCC` power symbol and a `GND` ground symbol to represent the connections rather than drawing the lines to a battery symbol.*

### Step-by-step guide in KiCad

#### 1. Create a new project
*   Launch KiCad and click **File > New Project**.
*   Give your project a name and save it in a new folder.

#### 2. Draw the schematic in the Schematic Editor (Eeschema)
*   From the main project window, double-click the `.kicad_sch` file to open the Schematic Editor.
*   **Add components:** Click the **Place Symbol** button on the right toolbar or press **A**.
    *   Find and place a resistor. Search for `R` or `resistor`.
    *   Find and place an LED. Search for `LED`.
    *   Find and place a power symbol. Search for `5V` or `VCC`.
    *   Find and place a ground symbol. Search for `GND`.
*   **Move and rotate components:**
    *   Hover over a component and press **M** to move it.
    *   Hover over a component and press **R** to rotate it.
*   **Connect components with wires:** Click the **Place Wire** button or press **W**.
    *   Click on the pins of the components to connect them in series.
*   **Edit component values:**
    *   Hover over the resistor and press **E** or **V** to change its value. For a typical red LED, a 470 Ω resistor with a 5V source is a common choice.
    *   You can also edit the values of the LED and power symbols for documentation purposes.
*   **Annotate the schematic:** Click **Tools > Annotate Schematic**. This assigns unique designators (e.g., `R1`, `D1`) to all components.
*   **Run the Electrical Rules Check (ERC):** Click **Tools > Electrical Rules Checker** and run the check to catch any basic errors.

#### 3. Assign footprints
*   Click **Tools > Assign Footprints** from the Schematic Editor.
*   In the footprint assignment window, select the appropriate physical packages for each component.
    *   **Resistor:** Select a footprint from the `Resistor_THT` library (for through-hole) or `Resistor_SMD` (for surface mount).
    *   **LED:** Select a footprint from the `LED_THT` library for a standard LED package.
    *   The power and ground symbols do not require a physical footprint.
