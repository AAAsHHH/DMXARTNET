# FAQ & Troubleshooting

Common issues and solutions for DMXnetART.

## Device does not power on

- Check supply voltage (must be within **5–24 VDC**).  
- Verify polarity on the power connector.  
- Try a different power supply or cable.

## Wi‑Fi connection fails

- Ensure SSID and password are correct.  
- Check that the network is 2.4 GHz if your hardware doesn’t support 5 GHz.  
- Verify signal strength at the device location.  
- Try a static IP configuration if DHCP is unreliable.

## Art‑Net not discovered by software

- Confirm the PC/controller is on the **same subnet** as the converter.  
- Check firewall settings; allow Art‑Net (UDP 6454).  
- Manually enter the device IP in your software if auto-discovery fails.  
- Verify subnet/universe settings match on both sides.

## DMX output seems wrong or flickers

- Check DMX wiring and pinout.  
- Ensure you have a proper **DMX terminator** at the end of the chain.  
- Reduce cable length or avoid running DMX next to high-current cables.  
- Test with a single fixture to isolate bad cables or devices.

## Firmware update fails

- Ensure you’re using the correct binary for your hardware revision.  
- Re-enter bootloader mode correctly.  
- Try a different USB cable or serial adapter.  
- Check serial output for error messages if available.

If your issue isn’t listed here, open a ticket on the GitHub repository with:

- Firmware version  
- Hardware revision  
- Short description of the problem  
- Any relevant logs or photos