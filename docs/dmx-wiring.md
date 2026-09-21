# DMX Wiring

This page covers proper DMX cabling, termination, and addressing for use with DMXnetART.

## DMX basics

- DMX512 uses **RS‑485** differential signaling.  
- One universe = up to **512 channels**.  
- Devices are daisy-chained from **DMX OUT** on the converter.

## Cabling

- Use **shielded twisted pair** DMX cable where possible.  
- Standard connectors: **3‑pin or 5‑pin XLR** (match your converter).  
- Avoid using regular audio cables for long runs or critical setups.

## Wiring example (3‑pin XLR)

- Pin 1: GND (shield)  
- Pin 2: DATA−  
- Pin 3: DATA+

Connect:

`DMXnetART DMX OUT → Fixture 1 IN → Fixture 1 OUT → Fixture 2 IN → … → Last fixture`

## Termination

- For long chains or many fixtures, add a **DMX terminator** at the last device.  
- A proper terminator is a 120 Ω resistor between DATA+ and DATA−.  
- Some fixtures have built-in termination that can be enabled.

## Addressing fixtures

- Each fixture has a **start address** (1–512 per universe).  
- Assign addresses so channels don’t overlap.  
- Example:
  - Moving head uses 16 channels → start at 1, next fixture at 17, etc.

Combine this with your Art‑Net universe mapping to plan your show.