# G.U.A.R.D (Gas, Utility, Air, and Respiratory Detection System)
 - Be reminded that this is intended for a school project. Therefore, everything you see within the provided data may differ, as components would be changed and vary.
---

 ### Project Overview:

- This prototype, named **G.U.A.R.D. (Gas, Utility, Air, and Respiratory Detection System)**, is a wearable safety device that combines the functionality of a digital watch with an environmental monitoring system. Its primary purpose is to monitor combustible gases, carbon monoxide (CO), air quality, temperature, humidity, and respiratory levels, providing users with real-time environmental and health-related information in a compact and portable form.

   #### Who is this project intended for?

     - This project is primarily designed for mineral workers and other individuals who work in hazardous environments. By continuously monitoring environmental conditions and respiratory indicators, **G.U.A.R.D.** helps users assess their surroundings, identify potential hazards at an early stage, and make informed decisions that can reduce the risk of accidents and exposure to dangerous conditions.

   #### What application areas is this project intended to serve?

     - **G.U.A.R.D.** is intended for use in mining operations, factories, industrial facilities, construction sites, warehouses, and other hazardous workplaces where    monitoring air quality, detecting harmful gases, and maintaining environmental awareness are essential for worker safety.

---

 ### HardWare Overview:
  #### Electronics:
  *Sensors:*
  <table border="1" cellpadding="10" cellspacing="0" style="border-collapse: collapse; width: 100%; font-family: Arial, sans-serif;">
    <thead>
        <tr style="background-color: #1a1a2e; color: white;">
            <th>Sensor</th>
            <th>Primary Detection</th>
            <th>Detectable Parameters</th>
            <th>Main Purpose in G.U.A.R.D.</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>MQ-2</strong></td>
            <td>Combustible Gas Detection</td>
            <td>LPG, Propane, Methane, Hydrogen, Smoke, and other flammable gases</td>
            <td>Detects combustible gas leaks and smoke to help prevent fires and explosions.</td>
        </tr>
        <tr>
            <td><strong>MQ-7</strong></td>
            <td>Carbon Monoxide (CO) Detection</td>
            <td>Carbon Monoxide (CO)</td>
            <td>Monitors carbon monoxide levels to help protect users from CO poisoning in hazardous environments.</td>
        </tr>
        <tr>
            <td><strong>MQ-135</strong></td>
            <td>Air Quality Monitoring</td>
            <td>Ammonia (NH₃), Nitrogen Oxides (NOₓ), Benzene, Alcohol, Smoke, and other volatile compounds</td>
            <td>Monitors overall air quality and detects harmful gases that may indicate unsafe environmental conditions.</td>
        </tr>
        <tr>
            <td><strong>MAX30102</strong></td>
            <td>Health Monitoring</td>
            <td>Heart Rate (BPM), Pulse Signal, Estimated Respiratory Rate</td>
            <td>Monitors the user's physiological condition and provides health-related information that may indicate fatigue, stress, or respiratory issues.</td>
        </tr>
        <tr>
            <td><strong>DHT11</strong></td>
            <td>Environmental Monitoring</td>
            <td>Temperature and Humidity</td>
            <td>Measures ambient temperature and humidity to provide additional environmental data and improve situational awareness.</td>
        </tr>
    </tbody>
</table>

*Sensor Function:*
<table border="1" cellpadding="10" cellspacing="0" style="border-collapse: collapse; width: 100%;">
    <tr>
        <td>
<strong>MQ-2</strong>

- A semiconductor gas sensor that detects combustible gases and smoke. It uses a heated <strong>tin dioxide (SnO₂)</strong> sensing element whose electrical resistance changes when exposed to flammable gases such as LPG, methane, propane, hydrogen, and smoke. These changes are converted into an electrical signal that can be read by a microcontroller to monitor gas concentration and provide early warnings of <strong>potential hazards.</strong>
        </td>
        <td width="280" align="center">
            <img src="https://github.com/user-attachments/assets/267966ba-e691-44c7-b545-7115decc8394"
                 width="250"
                 alt="MQ-2 Sensor">
        </td>
    </tr>
    <tr>
        <td>
<strong>MQ-7</strong>

- A semiconductor gas sensor specifically designed to detect <strong>carbon monoxide (CO)</strong>. It uses a heated <strong>tin dioxide (SnO₂)</strong> sensing element whose electrical resistance changes when exposed to carbon monoxide. These changes are converted into an electrical signal that can be read by a microcontroller to monitor CO concentration and provide early warnings of potentially dangerous carbon monoxide levels.
        </td>
        <td width="280" align="center">
            <img src="https://github.com/user-attachments/assets/09e58c86-2501-47d1-b56d-2e340519e270"
                 width="250"
                 alt="MQ-7 Sensor">
        </td>
    </tr>
    <tr>
        <td>
<strong>MQ-137</strong>

- A semiconductor gas sensor specifically designed to detect <strong>ammonia (NH₃)</strong>. It uses a heated <strong>tin dioxide (SnO₂)</strong> sensing element whose electrical resistance changes when exposed to ammonia gas. These changes are converted into an electrical signal that can be read by a microcontroller to monitor ammonia concentration and provide early warnings of potentially hazardous conditions.
        </td>
        <td width="280" align="center">
            <img width="250"
                 src="https://github.com/user-attachments/assets/b34b21a6-3fe8-4115-bd6e-39586fbdfb1c"
                 alt="MQ-137 Sensor" />
        </td>
    </tr>
    <tr>
        <td>
<strong>MAX30102</strong>

- A biometric sensor designed to measure <strong>heart rate (BPM)</strong> and <strong>blood oxygen saturation (SpO₂)</strong>. It uses red and infrared LEDs along with a photodetector to measure changes in blood flow beneath the skin. These optical signals are processed by a microcontroller to monitor the wearer's physiological condition and provide real-time health information.
        </td>
        <td width="280" align="center">
            <img width="250"
                 src="https://github.com/user-attachments/assets/e363d19c-1896-4f6f-8975-e53f097238be"
                 alt="MAX30102 Sensor" />
        </td>
    </tr>
    <tr>
        <td>
<strong>DHT11</strong>

- A digital temperature and humidity sensor that measures the ambient temperature and relative humidity of the surrounding environment. It uses a capacitive humidity sensor and a thermistor to collect data, then transmits the measurements as a digital signal to a microcontroller. This allows the system to monitor environmental conditions and provide additional information for workplace safety.
        </td>
        <td width="280" align="center">
            <img width="250"
                 src="https://github.com/user-attachments/assets/07dd2d53-9298-465c-88bb-b0b991cb68b0"
                 alt="DHT11 Sensor" />
        </td>
    </tr>
</table>

 *Power supply and control components:*
<table border="1" cellpadding="10" cellspacing="0" style="border-collapse: collapse; width: 100%; font-family: Arial, sans-serif;">
    <thead>
        <tr style="background-color: #1a1a2e; color: white;">
            <th>Component</th>
            <th>Primary Function</th>
            <th>Key Features</th>
            <th>Main Purpose in G.U.A.R.D.</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>ESP32-C3-DEVKITM-1</strong></td>
            <td>Microcontroller Unit (MCU)</td>
            <td>32-bit RISC-V processor, Wi-Fi, Bluetooth Low Energy (BLE), GPIO, SPI, I²C, UART, ADC, 4 MB Flash</td>
            <td>Serves as the main controller of the system by collecting sensor data, processing information, controlling peripherals, and managing communication between all hardware components.</td>
        </tr>
        <tr>
            <td><strong>Adafruit 2.0 Color IPS TFT Display</strong></td>
            <td>Visual Display</td>
            <td>320×240 IPS LCD, full-color graphics, SPI interface, wide viewing angles</td>
            <td>Displays real-time sensor readings, battery status, system alerts, menus, and other information for the user.</td>
        </tr>
        <tr>
            <td><strong>MINI560</strong></td>
            <td>Power Regulation</td>
            <td>High-efficiency DC-DC buck converter, stable 5 V output, compact design</td>
            <td>Converts battery voltage into a stable power supply for the ESP32-C3 and other electronic components while maximizing power efficiency.</td>
        </tr>
        <tr>
            <td><strong>TP4056</strong></td>
            <td>Battery Charging</td>
            <td>Single-cell Li-ion/Li-Po charging, CC/CV charging, overcharge protection (protected versions)</td>
            <td>Safely charges the rechargeable lithium battery and manages the charging process for reliable portable operation.</td>
        </tr>
    </tbody>
</table>

*Power supply and control components Function:*
<table border="1" cellpadding="10" cellspacing="0" style="border-collapse: collapse; width: 100%;">
    <tr>
        <td>

<strong>ESP32-C3-DEVKITM-1</strong>

- A compact development board based on the ESP32-C3 microcontroller, featuring a 32-bit RISC-V processor with integrated Wi-Fi and Bluetooth® Low Energy (BLE). It serves as the main controller of the G.U.A.R.D. system by collecting data from the sensors, processing the information, controlling peripheral devices such as the display, and managing communication between all connected components.
    </td>
        <td width="280" align="center">
        <img width="250"
             src="https://github.com/user-attachments/assets/646ccf67-1ee2-47ce-adff-56535f8bd790"
             alt="ESP32-C3-DEVKITM-1" />
        </td>
    </tr>
    <tr>
        <td>
<strong>Adafruit 2.0" 320×240 Color IPS TFT Display</strong>

- A 2.0-inch full-color IPS TFT display with a resolution of 320×240 pixels, designed to provide a bright, sharp, and easy-to-read graphical interface. It communicates with the ESP32-C3 through the SPI interface, enabling fast and efficient data transfer. In the G.U.A.R.D. system, the display presents real-time gas concentration, heart rate, blood oxygen level (SpO₂), ambient temperature, humidity, battery status, and system notifications. Its IPS technology provides wide viewing angles and accurate color reproduction, ensuring that critical information remains clearly visible under different viewing conditions.

  (had to make it smaller the image)
    </td>
         <td width="280" align="center">
         <img width="250"
              height="250"
              src="https://github.com/user-attachments/assets/45c601e4-bc0c-4781-8585-5d0cab17e56d"
              alt="Adafruit 2.0&quot; 320×240 Color IPS TFT Display" />
        </td>
    </tr>
    <tr>
        <td>
<strong>MINI560</strong>

- A compact, high-efficiency DC-DC buck (step-down) voltage converter designed to provide a stable power supply for electronic systems. It converts a higher input voltage from the rechargeable battery into a regulated output voltage suitable for powering the ESP32-C3, display, and other components. Its high conversion efficiency minimizes power loss, reduces heat generation, and helps extend the operating time of the G.U.A.R.D. system.
    </td>
        <td width="280" align="center">
        <img width="250"
             src="https://github.com/user-attachments/assets/e459525f-19c8-4561-8280-aa1aac8de0c2"
             alt="MINI560 DC-DC Buck Converter" />
        </td>
    </tr>
    <tr>
       <td>
<strong>TP4056</strong>

- A lithium-ion/lithium-polymer battery charging module designed for safely charging a single-cell rechargeable battery using a constant-current/constant-voltage (CC/CV) charging method. It manages the charging process by regulating the charging current and voltage while preventing overcharging. In the G.U.A.R.D. system, the TP4056 enables convenient USB charging of the battery, ensuring reliable and safe power management for portable operation.
    </td>
        <td width="280" align="center">
        <img width="250"
             src="https://github.com/user-attachments/assets/b980c2cd-4af7-4691-b7c8-22fbce7793a7"
             alt="TP4056 Battery Charging Module" />
    </td>
</tr>
</table>

**SCHEMATIC:**

  <img width="1007" height="737" alt="Screenshot 2026-07-10 175056" src="https://github.com/user-attachments/assets/8ea345c5-a3d6-4d8f-b1fc-2ff30036b934" />

- im too lazy to say the connections, please excuse me.



    
