![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg)

### Wokwi
https://wokwi.com/projects/347140425276981843

Customizable UART Transmitter (inspired by @maehw)

Supports ASCII characters from 0x40 (@) to 0x5F (_), including capital letters from the latin alphabet.

**How to use**

Example Sending 'A'
1. Set the Arduino serial baud rate `Serial.begin(<baud rate>);` in the *.ino file to 300
2. Set the Wokwi clock frequency `"attrs": { "frequency": "300" }` in the diagram.json to 300 as well
3. Set SW7 to OFF ("Load")
4. Set SW2 to ON and SW3-6 to OFF
5. Set SW7 to ON ("TX")
6. Set SW8 to ON ("Output Enable")

If there's no output from the Wokwi Arduino serial monitor, try toggling SW7 OFF and ON again.

Congratulations! You should now see the letter being output in the Wokwi Arduino Serial monitor at the bottom of the simulation.

Note that garbage characters may be printed upon initialization.
| SW      | Function| 
|---------|---------|
| 1       | N/A     | 
| 2       | Bit 0   | 
| 3       | Bit 1   |
| 4       | Bit 2   | 
| 5       | Bit 3   | 
| 6       | Bit 4   |
| 7       | Load/TX | 
| 8       | Out. En.| 
