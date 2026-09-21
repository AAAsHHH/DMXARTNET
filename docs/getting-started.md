# Getting Started

This guide walks you through the first-time setup of your DMXnetART converter.

## What’s in the box

- DMXnetART converter (v1.2)  
- Power cable or terminal block (depending on version)  
- Any included mounting hardware or labels

## Step 1 – Power the device

The converter accepts **5–24 VDC**.

- Use a suitable DC supply within this range.  
- Observe polarity on the power connector.  
- On power-up, the status LED should indicate power and boot.

## Step 2 – Connect to Wi‑Fi

On first boot, the device either:

- Creates its own **configuration AP**, or  
- Connects to a previously configured Wi‑Fi network.

Check the firmware documentation for:

- Default SSID / password (if using AP mode)  
- How to enter station mode and set your network credentials

Once connected, note the device’s IP address (via your router, serial output, or OLED/LED indication, depending on your design).

## Step 3 – Configure Art‑Net

Using the configuration interface (web UI, serial, or config file):

1. Set **Art‑Net node name** (e.g. `DMXnetART-01`).  
2. Choose number of universes (1–3).  
3. Assign **subnet** and **universe IDs** to match your lighting software.  
4. Save and reboot if required.

## Step 4 – Connect DMX fixtures

- Connect a standard DMX cable from the converter’s **DMX OUT** to your first fixture.  
- Daisy-chain fixtures as usual.  
- Add a **DMX terminator** at the end of the line if needed.

## Step 5 – Test with lighting software

In your lighting control software:

1. Enable **Art‑Net** output.  
2. Set the correct **subnet** and **universe**.  
3. Point Art‑Net output to the converter’s IP (or let it auto-discover).  
4. Patch fixtures and test channels.

You should now see DMX values on your fixtures controlled via Art‑Net over Wi‑Fi.