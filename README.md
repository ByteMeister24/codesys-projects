# CODESYS IEC 61131-3 Projects

This repository contains CODESYS projects implemented for Factory I/O scenes.
The contained projects are programmed using Structured Text (ST). For more info, see: https://www.plcacademy.com/structured-text-tutorial/

## Development Environment

- CODESYS version: `CODESYS V3.5 SP21 Patch 3+`
- Compiler version: `3.5.21.30` (`compiler="3.5.21.30"`)

## Factory I/O References

- Each project folder contains a `scene` folder with the Factory I/O scene file and the I/O mapping.
- Open the scene file in Factory I/O and control the simulation through CODESYS SoftPLC.
- Factory I/O scenes manual: https://docs.factoryio.com/manual/scenes/
- CODESYS + Factory I/O tutorials: https://docs.factoryio.com/tutorials/codesys/

## Troubleshooting

### Device Description Missing

If you see errors like `Device not installed to the system` or missing device descriptions:

- This is commonly caused by a CODESYS/version mismatch between the project and your local installation.
- In the device tree, right-click the device with the missing/unknown marker and select **Update Device**.
- Choose the equivalent target/device version that matches your installed CODESYS version.
- If errors remain, open **Library Manager** and download missing libraries.
- Check library placeholders and resolve any unresolved/missing versions (typically by selecting the latest compatible version).

Reference discussion: https://www.reddit.com/r/PLC/comments/1k390yr/codesys_error/
