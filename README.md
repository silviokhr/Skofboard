# Split Ergonomic Wireless Gasket-Mounted Keyboard

<div align="center">
  <img src="./Images/render.jpeg" alt="Split Ergonomic Keyboard" style="border-radius: 12px; max-width: 100%; box-shadow: 0 4px 8px rgba(0,0,0,0.2);">
</div>

## Features

- **Ergonomic split design** — reduces wrist strain and promotes a more neutral typing position
- **Ortholinear layout**     — aligns keys in a grid, reducing finger travel distance with 3 dedicated thumb buttons
- **Gasket-mounted PCB**     — provides a dampened sound profile and soft keystroke feel
- **Magnetic closure**       — enables quick assembly and disassembly without tools
- **Reversible PCB design**  — single PCB works for both left and right halves
- **Hot-swappable switches** — easily swap or customize switches without soldering
- **ZMK firmware support**   — fully customizable keymap via ZMK Studio
- **Wireless connectivity**  — powered by the nice!nano v2.0 microcontroller

---

## Default Keymap
The default keymap is currently a placeholder and varies by region. To customize your keyboard, access the **studio_unlock** key on the left half at **column 1, row 2** to enter configuration mode in ZMK Studio.

---

## Case

All case parts are CNC machined. Material selection significantly impacts sound profile. Rigid aluminum base dampens resonance while polycarbonate top provides acoustic transparency. Rounded internal surfaces minimize harsh reflections for refined keystroke sound. (STL files are included for 3D-printed case variants.) 

### Case Materials
| Part | Material | Surface Finish |
|------|----------|--------|
| Top casing | Polycarbonate (PC) | Blue-tinted vapor polishing | 
| Bottom casing | Aluminum 6061 | Bead blasting + anodizing |

---

## Internal Components  

### Magnets

Magnet cutouts are intentionally oversized to ensure proper fit during assembly.

| Type | Material | Diameter | Thickness | Cutout Diameter | Cutout Depth | Qty per Half | 
|------|----------|-----------|-----------------|--------------|--------------|--------------|
| Corner disc magnet| Neodymium | 4 mm | 3 mm | 4.1 mm | 3 mm | 8 |
| Edge disc magnet | Neodymium | 2 mm | 3 mm | 2.1 mm | 3 mm | 16 |

### Gasket-Foam

Poron foam provides dampening and spacing for the gasket mounting system.

| Type | Dimensions (L × W × H) | Qty per Half |
|------|--------|---------|
| Large foam strip | 4.5 × 7 × 2 mm | 6 |
| Small foam strip | 4.5 × 4 × 2 mm | 2 |

### Rubber Feet

Feet provide elevation and grip on desk surfaces.
* **Protrusion:** Minimum 0.1 mm above case bottom for optimal grip

| Component | Diameter | Thickness | Cutout Diameter | Cutout Depth | Qty per Half |
|-----------|-----------|--------------|--------------|--------------|--------------|
| Rubber foot | 8 mm | 1.6 mm | 8 mm |  1.5 mm | 4 |

### Microcontroller

| Component | Qty per Half |
|-----------|--------------|
| nice!nano v2.0 | 1 |

### Battery

The battery cutout on the top plate is shared with the battery connector jack, limiting usable space. Choose batteries within these **optimal dimensions**:
- **Height:** 50 mm
- **Width:** 20 mm  
- **Depth:** 30 mm

⚠️ **Constraints:** Taller batteries are possible, but wider or longer batteries are not recommended and may not fit reliably.

| Component | Specification | Qty per Half |
|-----------|---------------|--------------|
| Battery | 3.7V LiPo, 250 mAh, model 502030, 2P-PH connector | 1 |
| Battery connector | S2B-PH-K-S(LF)(SN) | 1 |

### Power Switch

| Component | Part Number | Qty per Half |
|-----------|-------------|--------------|
| Power switch | MSK12C02 | 1 |

**Type:** SMD slide switch
**Function:** Disconnects battery from microcontroller

### Hotswap Sockets

| Component | Type | Qty per Half |
|-----------|-------------|--------------|
| Hotswap Socket| Kailh MX-format | 30 |

### Switches (Keyswitches)

| Component | Type | Qty per Half |
|-----------|------|--------------|
| Keyswitch | MX-format (any compatible switch) | 30 |

**Mounting:** Hot-swappable PCB sockets

### Diodes

Protects against reverse polarity and back-EMF from switches

| Component | Part Number | Package | Qty per Half |
|-----------|-------------|---------|--------------|
| Protection diode | 1N4148W | SOD-123 | 30 |



---

## Complete Bill of Materials (BOM)

| Qty (per half) | Component | Type |
|---|-----------|------|
| 8 | Corner magnet | Neodymium disc, ⌀4mm × 3mm |
| 16 | Edge magnet | Neodymium disc, ⌀2mm × 3mm |
| 6 | Large gasket foam | Poron, 4.5 × 7 × 2mm |
| 2 | Small gasket foam | Poron, 4.5 × 4 × 2mm |
| 4 | Rubber feet | Natural rubber, ⌀8 × 1.6mm |
| 1 | Microcontroller | nice!nano v2.0 |
| 1 | Battery | 3.7V LiPo 250mAh 502030 |
| 1 | Battery connector | S2B-PH-K-S(LF)(SN) |
| 1 | Power switch | MSK12C02 |
| 30 | Keyswitch | MX-format |
| 30 | Diode | 1N4148W |
| 30 | Hotswap Socket | MX-format |

---

## PCB Specifications

- **Layer count:** 2-layer
- **Material:** FR-4, 1.6 mm thickness
- **Copper weight:** 1 oz
- **Surface finish:** LeadFree HASL

**Design Note:** 
The PCB switchplate (SkofTopPlate.kicad_pcb) is 1.6mm FR4 (standard manufacturing thickness). Standard MX switches are designed for 1.5mm plates. Due to this 0.1mm difference, switches fit securely but may feel slightly tight.

---

## Credits

This project uses open-source hardware footprints licensed under MIT and CC-BY-NC-SA 4.0 by Marco Massarelli (@ceoloide) and contributors.