🌱 SMART WATER IRRIGATION SYSTEM

🔧 COMPONENTS USED

1. ESP8266 Microcontroller
Acts as the main controller for the system
Reads soil moisture values
Controls the motor driver and pump
Can be used for Wi-Fi/IoT monitoring (optional)

2. Motor Driver (L298N / L293D / Relay Driver)
Used to safely control the water pump motor
Provides necessary current/voltage to the pump
Protects ESP8266 from high current load

3. Ultrasonic Sensor (HC-SR04)
Measures water tank level or reservoir water depth
Helps prevent pump from running when tank is empty
Improves system safety and water management

4. Water Pump
Pumps water to the plants automatically
Controlled via the motor driver based on soil moisture readings

5. DC Motor
Used for additional mechanical movement (if required)
Can be controlled by the motor driver

7. Soil Moisture Sensor
Measures the moisture content in the soil
Sends data to ESP8266 to decide when the pump should turn ON or OFF

8. Two (2) Switches
Switch 1: Manual Pump ON/OFF control
Switch 2: Mode selector (Manual / Automatic)
Allows user interaction even without Wi-Fi

9. Resistor (1 or more)
Used for LED current limiting or pull-up/pull-down functions
Protects components from overcurrent

10. Two (2) Solar Panels (5V)
Provide renewable energy to charge the rechargeable battery
Power the system during sunlight
Eco-friendly and reduces dependency on external power

11. Rechargeable Battery (Lithium/Lead Acid/18650)
Stores energy from the solar panels
Powers the ESP8266, sensors, and pump when sunlight is not available
Ensures uninterrupted operation

12. LED Indicator
Shows system status such as:
Power ON
Charging status
Pump ON/OFF
Wi-Fi connection

⭐ ABOUT THE PROJECT

The Smart Water Irrigation System is an innovative and eco-friendly automation project designed to simplify plant watering, conserve water, and make irrigation efficient with the help of technology. This system uses sensors, solar power, microcontrollers, and automated water flow control to ensure plants receive the right amount of water at the right time. It is built as a collaborative team effort with clear roles assigned to each member, highlighting excellent teamwork and technical coordination.

The main goal of this project is to create a system that automatically waters plants based on real-time soil moisture conditions. When the soil becomes dry, the pump automatically turns ON and supplies water to the plants. When the soil moisture reaches a healthy level, the pump turns OFF. This eliminates the need for manual watering, reduces water wastage, and supports sustainable farming practices.

To achieve this, several electronic components are integrated. The ESP8266 microcontroller acts as the brain of the system. It reads values from the soil moisture sensor, processes data, and controls the motor driver and pump. The ESP8266 also has built-in Wi-Fi, which can be used for IoT functionalities like monitoring soil moisture online or checking pump status remotely (optional).

A motor driver (like L293D or L298N) is used to control the water pump and DC motor. This driver protects the microcontroller from high current and allows safe switching of the pump. The water pump ensures water is supplied to the plants whenever the system detects dryness. A DC motor is also available for additional movement, depending on future expansion of the project.

A very important component is the soil moisture sensor, which determines how much water is present in the soil. If the sensor detects low moisture, the controller activates the pump. If the sensor detects high moisture, the pump stops automatically. This creates a smart closed-loop solution for plant irrigation.

The system also uses an ultrasonic sensor (HC-SR04) to check the water level in the tank. If the tank is empty, the ultrasonic sensor prevents the pump from running, protecting the motor from damage and saving energy. This increases the reliability and lifespan of the system.

To make the project environmentally friendly, two 5V solar panels charge a rechargeable battery, which powers the entire system. This makes the irrigation system independent of external power sources and suitable for farms, gardens, and remote areas where electricity supply may be limited. Solar charging ensures that even during power cuts or nighttime, stored battery power runs the system smoothly.

Two physical switches are included. One switch can be used for manually turning the pump ON/OFF, while the second switch can be used to change the working mode between manual mode and automatic mode. A resistor is used for current control, especially for LED safety and input protection. A single LED is included to provide basic indication—for example, pump status, power status, or Wi-Fi connectivity.

Along with the hardware and logic, this project showcases excellent teamwork. Each member contributed uniquely to the system’s success.

🧑‍🤝‍🧑 Team Roles & Special Credits

🧠 Team Leadership
Captain: Bruvan 
Vice-Captain: Aarush

🧠 Planning & System Architecture
Bruvan – Project layout planning, workflow strategy, component selection, power system planning, and feature integration.

⚡ Circuit Wiring & Electrical Design
Aarush – Designed and executed the circuit wiring, relay and motor driver connections, sensor wiring, LED indicators, and ensured safe and correct electrical layout.

👨‍💻 Coding & Programming
Vishwa – Developed the ESP8266 code, soil moisture logic, ultrasonic integration, pump control automation, and overall system programming.

🔧 Hardware Setup & Assembly
Adeen – Assembled all hardware components, mounted sensors, installed pump and motor driver, and ensured a stable physical setup.

🔋 Solar Charging + ESP8266 Monitoring Circuit

This circuit demonstrates a basic solar-powered battery charging system with ESP8266-based monitoring.
A solar panel is used to generate power, which flows through a blocking diode to safely charge a 9V battery without allowing reverse current at night.

To monitor the battery voltage, an ESP8266 (such as NodeMCU) senses the battery level through a voltage divider that steps the 9V down to a safe input range for the ADC pin.
An indicator LED is added to show charging status.

The ESP8266 can further upload the battery status to cloud platforms like Blynk, Firebase, or a simple web server — enabling IoT-based solar monitorin

🔁 How the Circuit Works

Solar Panel → Battery
The solar panel charges the 9V battery. The diode prevents reverse discharge.

Battery → ESP8266 (Monitoring Only)
The voltage divider reduces the battery voltage to safe ADC levels (~0–3.3V).
ESP8266 reads this value through A0 pin.

LED Indicator
The LED turns ON when charging (panel voltage present).

IoT Monitoring (Optional)
ESP8266 can publish battery voltage to Blynk, MQTT, or a webpage.

Circuit Diagram


![Circuit Diagram](https://raw.githubusercontent.com/<username>/<repo>/main/circuit.png)


