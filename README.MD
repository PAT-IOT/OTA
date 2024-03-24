# IoT Controller Firmware Update via Web Interface

This firmware enables Over-The-Air (OTA) updates for an IoT controller using a web interface. It allows you to upload firmware files to the controller without the need for physical access.

## Features

- **Web Interface**: Provides a simple web interface for uploading firmware files.
- **Authentication**: Implements a basic authentication mechanism for accessing the update page.
- **OTA Update**: Enables Over-The-Air updates for the IoT controller firmware.

## Setup Instructions

To use this firmware for your IoT controller, follow these steps:

1. **Requirements**:
   - ESP32 board compatible with the Arduino framework.
   - WiFi network credentials.

2. **Installation**:
   - Clone or download this repository to your local machine.

3. **Configuration**:
   - Open the `OTA_Controller.ino` file in the Arduino IDE or any compatible editor.
   - Modify the `ssid` and `password` variables to match your WiFi network credentials.
   - Optionally, you can change the `host` variable to set a custom hostname for the device.

4. **Upload Firmware**:
   - Connect your ESP32 board to your computer.
   - Compile and upload the firmware to your ESP32 board.

5. **Usage**:
   - Once the firmware is uploaded, the ESP32 will create an access point with the configured SSID.
   - Connect your computer or smartphone to this access point.
   - Open a web browser and navigate to `http://Novaday.local` (replace `Novaday` with the configured hostname).
   - You will be prompted to enter a username and password. The default credentials are `admin` for both username and password.
   - After successful authentication, you can upload firmware files using the provided interface.

6. **OTA Update**:
   - Select the firmware file using the "Choose file..." button.
   - Click the "Update" button to initiate the firmware update process.
   - Monitor the progress bar to track the update process.
   - Once the update is complete, the device will automatically reboot with the new firmware.

## Important Notes

- Ensure that your firmware files are compatible with the ESP32 platform and follow the required format.
- It's recommended to test the firmware update process in a controlled environment before deploying it in production.
- Always secure your device by changing the default credentials and implementing additional security measures as needed.

