# G.U.A.R.D (Gas, Utility, Air, and Respiratory Detection System)
 - Be reminded that this is intended for a school project. Therefore, everything you see within the provided data may differ, as components would be changed and vary.
---

 ### Project Overview:

- This prototype, named **G.U.A.R.D. (Gas, Utility, Air, and Respiratory Detection System)**, is a wearable safety device that combines the functionality of a digital watch with an environmental monitoring system. Its primary purpose is to monitor combustible gases, carbon monoxide (CO), air quality, temperature, humidity, and respiratory levels, providing users with real-time environmental and health-related information in a compact and portable form.

   #### Who is this project intended for?

     - This project is primarily designed for mineral workers and other individuals who work in hazardous environments. By continuously monitoring environmental conditions and respiratory indicators, **G.U.A.R.D.** helps users assess their surroundings, identify potential hazards at an early stage, and make informed decisions that can reduce the risk of accidents and exposure to dangerous conditions.

   #### What application areas is this project intended to serve?

     - **G.U.A.R.D.** is intended for use in mining operations, factories, industrial facilities, construction sites, warehouses, and other hazardous workplaces where    monitoring air quality, detecting harmful gases, and maintaining environmental awareness are essential for worker safety.

 ### HardWare Overview:
  #### Electronics:
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
            <td><strong>MAX30105</strong></td>
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

#### Function:
<table>
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
</table>
<table>
    <tr>
        <td>
<strong>MQ-7</strong>
- A semiconductor gas sensor specifically designed to detect <strong>carbon monoxide (CO)</strong>. It uses a heated tin dioxide (SnO₂) sensing element whose electrical resistance changes when exposed to carbon monoxide. These changes are converted into an electrical signal that can be read by a microcontroller to monitor CO concentration and provide early warnings of potentially dangerous carbon monoxide levels.
        </td>
         <td align="center" width="280">
            <img src="https://github.com/user-attachments/assets/09e58c86-2501-47d1-b56d-2e340519e270"
                width="250"
                alt="MQ-7 Sensor">
        </td>
    </tr>
</table>
<table>
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
</table>
<table>
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
</table>
<table>
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

 

    
