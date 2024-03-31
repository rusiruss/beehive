# Setting up Arduino IDE for ESP8266 NodeMCU

## Prerequisites

Before you begin, make sure you have the following:

- Arduino IDE installed on your computer. You can download it from the [Arduino website](https://www.arduino.cc/en/software).
- ESP8266 NodeMCU board.
- USB cable to connect the NodeMCU board to your computer.

## Steps

Follow these steps to set up the Arduino IDE for programming the ESP8266 NodeMCU:

1. **Open Arduino IDE**: Launch the Arduino IDE on your computer.

2. **Adding ESP8266 Board Manager URL**:
   - Go to `File` > `Preferences` in the Arduino IDE.
   - In the `Additional Board Manager URLs` field, add the following URL:
     ```
     http://arduino.esp8266.com/stable/package_esp8266com_index.json
     ```
   - Click `OK` to close the Preferences window.

3. **Installing ESP8266 Board Package**:
   - Go to `Tools` > `Board` > `Boards Manager...`.
   - Search for `esp8266` and install the package named (Recommended Version 2.7.3)`esp8266 by ESP8266 Community`.
   - Once the installation is complete, close the Boards Manager window.

4. **Selecting ESP8266 Board**:
   - Go to `Tools` > `Board`.
   - From the list, select `Generic ESP8266 Module)`.

5. **Setting Port**:
   - Go to `Tools` > `Port`.
   - Select the port to which your NodeMCU board is connected. It will typically be something like `COMX` on Windows or `/dev/cu...` on macOS.

6. **Testing the Setup**:
   - To test if everything is set up correctly, you can try uploading a sample sketch.
   - Go to `File` > `Examples` > `ESP8266` > `Blink`.
   - This will open a new sketch that blinks an LED connected to GPIO pin D0 (pin 16).
   - Click on the `Upload` button (right arrow icon) to compile and upload the sketch to your NodeMCU board.
   - Once the upload is complete, you should see the LED on your NodeMCU board blinking.

7. **Customizing Flash Size (Optional)**:
   - By default, the flash size is set to 4M (1M SPIFFS). If you need a different flash size, you can change it from `Tools` > `Flash Size`.

## Conclusion

You have successfully set up the Arduino IDE to work with the ESP8266 NodeMCU board. You can now start building IoT projects and experimenting with the vast capabilities of the NodeMCU platform. 

❤︎ Happy coding! 
