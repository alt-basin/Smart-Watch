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
            <td><strong>DHT22</strong></td>
            <td>Environmental Monitoring</td>
            <td>Temperature and Humidity</td>
            <td>Measures ambient temperature and humidity to provide additional environmental data and improve situational awareness.</td>
        </tr>
    </tbody>
</table>


    
