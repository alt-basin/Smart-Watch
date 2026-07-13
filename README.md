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
            <th>Component</th>
            <th>Primary Function</th>
            <th>Detectable Parameters</th>
            <th>Main Purpose in G.U.A.R.D.</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>TGS2611</strong></td>
            <td>Combustible Gas Detection</td>
            <td>Methane (CH₄), Natural Gas</td>
            <td>Detects combustible gas leaks to provide early warning against fire and explosion hazards in industrial environments.</td>
        </tr>
        <tr>
            <td><strong>ZE07-CO</strong></td>
            <td>Carbon Monoxide Detection</td>
            <td>Carbon Monoxide (CO)</td>
            <td>Continuously monitors carbon monoxide concentration and alerts the user when dangerous CO levels are detected.</td>
        </tr>
        <tr>
            <td><strong>ENS160 + AHT21</strong></td>
            <td>Air Quality Monitoring</td>
            <td>TVOC, eCO₂, AQI, Temperature, Humidity</td>
            <td>Measures indoor air quality, volatile organic compounds, temperature, and humidity to help identify unhealthy environmental conditions.</td>
        </tr>
        <tr>
            <td><strong>MAX30102</strong></td>
            <td>Health Monitoring</td>
            <td>Heart Rate (BPM), Blood Oxygen Saturation (SpO₂), Pulse Signal</td>
            <td>Monitors the user's vital signs to assess physiological condition and detect potential health risks caused by hazardous gases.</td>
        </tr>
        <tr>
            <td><strong>Mini DS3231 RTC</strong></td>
            <td>Real-Time Clock</td>
            <td>Time, Date</td>
            <td>Maintains accurate timekeeping for displaying the current time, timestamping sensor readings, and preserving time during power interruptions using its backup battery.</td>
        </tr>
    </tbody>
</table>

*Sensor Function:*


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

<img width="567" height="728" alt="Screenshot 2026-07-13 210535" src="https://github.com/user-attachments/assets/eb3cc2ca-a93f-46ca-a34b-07f00ae555fc" />
  
- im too lazy to say the connections.



    
