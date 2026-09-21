# Art‑Net Configuration

This page explains how to configure Art‑Net on the DMXnetART converter and in common lighting software.

## Art‑Net basics (brief)

- Art‑Net transports DMX data over IP networks.  
- Each **universe** = 512 DMX channels.  
- Devices are addressed by:
  - **IP address**  
  - **Subnet** and **universe ID** (in Art‑Net terms)

DMXnetART supports **1–3 universes**.

## Device configuration

In the firmware config (web UI, serial, or config file):

- **Node name**: Human-readable name (e.g. `DMXnetART-01`).  
- **Subnet**: Usually 0–15 depending on your network design.  
- **Universes**:
  - Universe 0 → DMX channels 1–512  
  - Universe 1 → channels 513–1024  
  - Universe 2 → channels 1025–1536  

Map these to physical DMX outputs according to your hardware design.

## Example: QLC+

1. Open **Edit → Preferences → Plugins → ArtNet**.  
2. Enable Art‑Net and set the correct interface (your Wi‑Fi network).  
3. Add an Art‑Net node; it should discover `DMXnetART-01`.  
4. Assign universes and patch fixtures.  

## Example: Resolume / other software

- Enable Art‑Net output.  
- Set subnet/universe to match the converter.  
- Ensure the software is on the same IP subnet as the device.

## Tips

- Keep subnet/universe mapping consistent across all nodes.  
- Use static IPs or DHCP reservations for reliable operation in shows.  
- For multi-node setups, document each node’s IP, subnet, and universe mapping.