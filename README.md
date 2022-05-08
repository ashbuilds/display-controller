# Display controller
Display controller PCB800099 with firmware and flasher using Arduino Uno


## Connection

### Arduino ###

Compile the RTD266xArduino sketch with the Arduino IDE and download it onto your Arduino. You can close the Arduino IDE afterwards.

#### Connecting ####

The communication between display and Arduino is done via I�C which is accessible on the VGA and HDMI ports of RTD266x. Connect SCL, SDA and GND with the corresponding Arduino pins.

For an Arduino Uno and an VGA connector, this would be:

| Pin name | Arduino Uno | VGA pinout |
| --- | --- |------------|
| SCL | A5 | 15         |
| SDA | A4 | 8, 7, 6    |
| GND | GND | 17         |

There are no additional pull-ups required, they are already on the RTD266x PCB.

Connect the display and Arduino as mentioned above. Power on the display first, then the Arduino.

A flashing user LED on the Arduino indicates a problem with the connection. Reset the Arduino to try again and use the GUI tool to read the error info.