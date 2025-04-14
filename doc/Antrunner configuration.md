
# AntRunner

AntRunner is a portable antenna rotator designed and manufactured by Muse Lab. This project is open source and available at: [GitHub Repository](https://github.com/wuxx/AntRunner).

## AntRunner with Hamlib

AntRunner can be controlled using Hamlib.

- Ensure Hamlib is installed on the Raspberry Pi (refer to the Hamlib installation script).
- Connect AntRunner to the Raspberry Pi via a USB port.
- The AntRunner USB connection appears as a serial port. You can identify the serial port by running: `ls /dev/tty*`.

### Controlling AntRunner via Command Line

With Hamlib, you can use the **rotctl** command to control the rotator:

```bash
rotctl -m 2401 -r /dev/ttyUSB0
```

