# Firmware

This page covers firmware installation, configuration, and updates for DMXnetART.

## Supported firmware

- Current version: **v1.2** (Art‑Net → DMX, 1–3 universes, Wi‑Fi)  
- Source code: (link to your repo or a dedicated firmware repo)

## Flashing the firmware

Typical flow for ESP32-based hardware:

1. Put the device in **bootloader mode** (hold BOOT button while powering on, or use GPIO strap).  
2. Connect via USB/serial to your PC.  
3. Use your preferred tool (e.g. `esptool`, Arduino IDE, PlatformIO, VS Code) to flash the binary.  
4. Reset the device.

Provide exact commands or IDE settings if you want users to build from source.

## Initial configuration

After first flash:

- The device may start in **configuration AP mode**.  
- Connect to the AP and open the configuration page (usually at `192.168.4.1` or similar).  
- Set:
  - Wi‑Fi SSID and password  
  - Art‑Net node name  
  - Universe count and mapping  
  - Any other options (e.g. static IP, DMX fade curves)

Save and reboot.

## Updating firmware

To update:

1. Download the latest firmware binary.  
2. Flash it over the existing firmware using the same method as initial flashing.  
3. Configuration may be preserved depending on your storage design (SPIFFS/LittleFS vs. full erase).

Document whether config is kept or reset on update.