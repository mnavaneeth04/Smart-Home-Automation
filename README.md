🔌 **Smart Home Automation using ESP32 and Firebase**
This repository contains the code and circuit information for a smart home automation system that uses Bluetooth-based user detection and Firebase cloud integration. The system is designed to personalize appliance control (fan and light) based on the presence of authorized users.

📝** Description**
The smart home automation system is built using the ESP32 microcontroller, which features built-in Bluetooth and Wi-Fi capabilities. It detects nearby users by scanning for their smartphone’s Bluetooth MAC address. Once a recognized user is detected, their personalized preferences are retrieved from Firebase Realtime Database, and the system controls connected devices accordingly. The project uses two LEDs (representing light and fan status) and a DC motor (acting as a fan) controlled via an L298N motor driver.

The code is written using the Arduino programming language (C/C++) and is compatible with the Arduino IDE.

🧰** Hardware Requirements**
To build and run the smart home automation system, you will need the following components:

ESP32 DevKit board

L298N Motor Driver

DC Motor (1)

LEDs (2)

220Ω Resistors (2)

Breadboard and jumper wires

Power source (e.g., USB or battery for motor)

⚙️ **Installation**
Connect the components according to the circuit diagram provided in the repository.

Clone or download this repository to your local machine.

Open the Arduino IDE and load the main .ino file.

Enter your Wi-Fi credentials and Firebase database details in the code.

Upload the code to the ESP32 board.

🚀 **Usage**
Power on the ESP32 and ensure it connects to Wi-Fi and Firebase.

The ESP32 will begin scanning for nearby Bluetooth devices.

If a recognized MAC address is found, the system retrieves user preferences from Firebase.

Based on the data, the LEDs and DC motor are activated accordingly.

Devices turn OFF automatically when no authorized user is nearby.

🔒 **Security & Efficiency**
The system activates appliances only when necessary, contributing to improved energy efficiency. For added security, MAC address validation is implemented, with future upgrades planned for encryption and access control.

🤝 **Contributing**
Contributions are welcome! Feel free to fork the repository and submit a pull request if you have improvements, bug fixes, or new features to suggest.

🙏 **Acknowledgements**
ESP32 and Firebase documentation

Open-source community projects related to smart home systems

Arduino IDE for development tools
