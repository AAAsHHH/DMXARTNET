# Hardware

This section describes the hardware design and connections of the DMXnetART converter.

## Enclosure

- Compact housing designed for integration into lighting rigs or control desks.  
- Dimensions: **200 × 40 × 20 mm**  
- Weight: **~150 g**

## Connectors

### Power input

- Voltage: **5–24 VDC**  
- Connector type: (barrel jack / terminal block – specify your actual design)  
- Polarity: (center-positive / terminal labeling – specify)

### DMX output

- Standard: **DMX512 / RS‑485**  
- Connector: **3‑pin or 5‑pin XLR** (specify which you use)  
- Pinout (example for 3‑pin):

  - Pin 1: GND  
  - Pin 2: DATA− (cold)  
  - Pin 3: DATA+ (hot)

Adjust this to your actual schematic.

### Network

- **Wi‑Fi** (internal antenna)  
- No Ethernet port on this version; Art‑Net is transported over Wi‑Fi only.

## Internal hardware (optional section)

If you want to share details for advanced users:

- MCU: (e.g. ESP32 variant)  
- DMX driver: (e.g. MAX485 / SN75176 or dedicated DMX chip)  
- Power regulation: (LDO / buck, input range, etc.)

This helps users who might modify or repair the unit.