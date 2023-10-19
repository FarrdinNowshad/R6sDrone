# Wi-Fi Camera and Car Control

This project combines a Wi-Fi camera and a car control system using an ESP32 microcontroller. The system allows you to remotely view the camera feed and control the movement of a car.

## Prerequisites
- Arduino IDE installed
- ESPAsyncWebServer library installed
- AsyncTCP library installed
- ESP32 board selected in Arduino IDE
- Camera module connected to the ESP32
- Motor driver and motors connected to the specified pins
- HTML, CSS, and JavaScript knowledge for customizing the web interface

## Hardware Setup
1. Connect the camera module to the specified pins on your ESP32.
2. Connect the motors and motor driver to the specified pins for the car control system.
3. Adjust the motorPins and camera-related constants in the code based on your hardware setup.

## Configuration
1. Set your Wi-Fi credentials in the code.
   ```cpp
   const char* ssid     = "Your_WiFi_SSID";
   const char* password = "Your_WiFi_Password";
   ```

## Running the Code
1. Upload the code to your ESP32 board using the Arduino IDE.
2. Open the Serial Monitor to view the ESP32's IP address.
3. Connect to the Wi-Fi network created by the ESP32.
4. Open a web browser and enter the IP address to access the control interface.
5. Use the interface to view the camera feed, control the car's movement, adjust speed, and control the light.

## Web Interface
- The web interface provides arrows for controlling the car's movement (UP, DOWN, LEFT, RIGHT).
- Sliders allow adjusting the car's speed and the intensity of an external light source.
- The camera feed is displayed in real-time on the interface.

## Troubleshooting
- If the camera feed is not displayed, check the camera connections and initialization in the code.
- Ensure that the motor and motor driver connections match the specified pins in the code.
- Check the Serial Monitor for any error messages.

## Acknowledgments
- This project uses the ESPAsyncWebServer library for handling HTTP requests and websockets.
- The camera module is initialized using the esp_camera library.
- Motor control is achieved using PWM signals through the LEDC library.

Feel free to customize and enhance the project according to your needs!
```
