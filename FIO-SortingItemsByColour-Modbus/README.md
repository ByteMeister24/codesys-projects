# FIO-SortingItemsByColour-Modbus

## Factory I/O Information

- Base scene: `Sorting Station`
- Brief description: The station sorts items by color (green and blue) using a vision sensor.
- Control protocol: Modbus (Factory I/O communication is handled via Modbus).
- Official scene details: https://docs.factoryio.com/manual/scenes/sorting-station/

### Scene Modifications

This scene is modified from the original scene provided in the Factory I/O library:

- The stop blade between the entry and exit conveyor is removed.
- A capacitive sensor is added to track items leaving the entry conveyor.
- A diffuse sensor is added at the end of the line for error detection.
- If an item reaches the end sensor, an error is raised.
- Stacklights are added to indicate the current operational state of the sorting station.

### Operation Mode

The current project provides two operation modes for scene control: manual and automatic.

- Manual mode is selected by default.
- In manual mode, press the start button to start the machine.
- Turn the knob to select automatic mode if you want the machine to start automatically through the SoftPLC.

## Demo

![Sorting station running demo](running_demo.gif)
![Sorting station fault injection demo](fault_injection_demo.gif)
