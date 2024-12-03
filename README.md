ESP8266 Data Logger with Google Sheets Integration

This project uses an **ESP8266** microcontroller to log sensor data and send it to a **Google Sheets** document via Google Apps Script.

Features
- Connects to a Wi-Fi network.
- Reads sensor data through the UART interface in the format `light1,light2,light3`.
- Sends the data to Google Sheets using an HTTPS GET request.
- Retrieves the current time using NTP (Network Time Protocol).
- Provides a visual indicator using an LED connected to pin `D1`.
- Automatically reconnects to Wi-Fi if disconnected.

Prerequisites
1. **ESP8266 Board**: Install the required board support in the Arduino IDE.
2. **Google Apps Script**: Configure a script to handle the data and link it to your Google Sheets.
3. **Wi-Fi Credentials**: Update the `ssid` and `password` in the code.
4. **GAS ID**: Replace `GAS_ID` in the code with your Google Apps Script ID.

Usage
1. Upload the code to the ESP8266.
2. Connect the ESP8266 to the specified Wi-Fi network.
3. Send data through the serial interface in the format `light1,light2,light3`.
4. View the logged data in your Google Sheets document.

The project can be used, for example, to use the data sent to the sheets to simulate the rotation of light sources.
