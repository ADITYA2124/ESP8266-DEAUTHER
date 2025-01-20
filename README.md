# ESP8266 Deauther Project

This project is an ESP8266-based Wi-Fi deauthentication tool that sends deauth packets to disconnect devices from a Wi-Fi network. It uses an SH1106 OLED display to show real-time network status and other relevant information. The tool is controlled through a simple web interface and allows the user to perform network testing.

## Features

- Sends deauthentication packets to disconnect devices from a Wi-Fi network.
- Displays network status and details on an SH1106 OLED display.
- Web interface for controlling the deauth process.
- Allows targeting specific Wi-Fi networks.

## Requirements

- ESP8266 (NodeMCU or similar)
- SH1106 OLED Display
- Arduino IDE
- Required libraries:
  - `ESP8266WiFi`
  - `Adafruit_SH1106`
  
## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/ADITYA2124/ESP8266-DEAUTHER.git
    ```

2. **Set up Arduino IDE:**

    - Install the ESP8266 board support via the Board Manager.
    - Install the required libraries:
      - `ESP8266WiFi`
      - `Adafruit_SH1106` (for the OLED display)

3. **Configure the Code:**

    - Open the `.ino` file in the Arduino IDE.
    - Modify the Wi-Fi credentials in the code:

    ```cpp
    const char* ssid = "your-SSID";        // Enter your Wi-Fi SSID
    const char* password = "your-password"; // Enter your Wi-Fi password
    ```

4. **Upload the Code:**

    - Select the correct board (ESP8266) and port.
    - Upload the code to your ESP8266 using the Arduino IDE.

## Usage

1. **Connect your ESP8266:**

    - Ensure the ESP8266 is properly connected to the computer via USB.
    - Ensure the SH1106 OLED display is connected to the ESP8266 using I2C.

2. **Run the code:**

    - Open the serial monitor to view connection status.
    - The ESP8266 will attempt to connect to your Wi-Fi network.
    - Once connected, it will display a message on the OLED display.

3. **Access the Web Interface:**

    - Once the ESP8266 is connected to Wi-Fi, it will display the IP address in the serial monitor.
    - Open a web browser and enter the IP address to access the web interface.

4. **Send Deauth Packets:**

    - Use the web interface to select the target network and start sending deauth packets.
    - The OLED display will show real-time status of the deauth process.

5. **Stop the Script:**

    - Press `Ctrl+C` to stop the script if running in serial monitor or terminal.

## Files

- `ESP8266_Deauther.ino`: The main Arduino sketch for the deauth tool.

## Images and Circuit Diagram

![Circuit Diagram](https://github.com/user-attachments/assets/e53d0b5f-ab0d-4196-922b-4998fb65332d)
*Circuit Diagram*

![Actual Circuit](https://github.com/user-attachments/assets/0ab8f963-eb87-4181-a4a4-52469086d400)
*Actual Circuit Preview*


## Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
