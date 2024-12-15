[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/KSk4F6vj)

# 1.Changes throughout the project

## Target Market & Demographics

Initial Phase:  
Focus: Primarily large event organizers for reducing maintenance costs and ensuring restroom cleanliness.
Geographical Focus: North America and Europe due to high demand and regulatory environments.
Market Size Estimation: General global mobile restroom market projected to reach over $15 billion by 2027.  

Changes Throughout the Project:  
Detailed Breakdown: Provided a more granular market size analysis segmented by region and industry (e.g., events, construction, municipal).  
Differentiation Strategies: Clearly articulated how the product stands out from competitors, particularly through advanced IoT integration and smart monitoring features.  

## Security, Hardware, & Software Requirements

Initial Phase:  
Security:  
Basic requirements for data privacy, integrity, tampering prevention, and secure storage.  
Hardware:  
Utilization of Nordic Thingy:91 for GPS tracking, user volume monitoring via Hall effect sensors, and air quality detection via gas sensors.  
Software:  
Managed GPS tracking, user-triggered alerts, and data transmission to the cloud via LTE-M/NB-IoT.  

Changes Throughout the Project:  
Security: Implemented end-to-end encryption for data in transit and at rest.  
Upgraded Hardware Specifications: use nRF 9160dk instead of Nordic Thingy:91 (for the Memfault cellular ).
Advanced Software Features: use nRF cloud to show the location of the device.

## Product Function & Components

Initial Phase:  
Primary Functions:  
GPS tracking of portable toilets.  
User volume monitoring via Hall effect sensors.  
Air quality detection via gas sensors.  
Core Components:  
Nordic Thingy:91, Hall effect sensors, gas sensors.  

Changes Throughout the Project:  
The product features have hardly changed.  
Core Components: nRF 9160dk, bme680(as gas sensor), button(instead of Hall effect sensors)  

## Power & Cost Budgeting

Bulk Purchasing Discounts: Negotiated bulk purchasing agreements for components, reducing per-unit costs.  
Component Substitutions: Identified alternative suppliers or component models offering similar functionality at lower costs without compromising quality.  
Prototype to Production Scaling: Adjusted cost estimates to account for economies of scale as production moves from prototype to mass manufacturing.  

# 2. What parts of the project were successful

Detailed Software Requirements Specification  

Why It's a Success:  

1.Real-Time Monitoring and Alerts: Implementing real-time GNSS tracking and alert systems ensures that maintenance staff can respond promptly to issues, enhancing operational efficiency.
Power Monitoring: Monitoring battery status and sending low-power alerts adds a layer of reliability, ensuring that the system remains functional when needed.

2.System Administrators and Maintenance Staff: Clearly defining user roles ensures that the software meets the specific needs of different stakeholders, facilitating ease of use and effective management.  

3.LTE-M/NB-IoT Connectivity: Utilizing reliable and low-power communication technologies ensures that your system can maintain continuous connectivity with minimal energy consumption.  

# 3. What parts of your project didn’t go well

Technical Integration and Hardware Challenges  

Issues Faced:  

Sensor Reliability: Certain sensors (e.g., bme680) may have exhibited inconsistent performance in real-world conditions.  
Hardware Durability: The hardware components, including the nRF 9160dk, may have faced durability issues when deployed in outdoor environments.  

Reasons:  
Environmental Factors: Exposure to extreme weather conditions, dust, and moisture could have affected sensor performance and hardware longevity.  
Integration Complexities: Integrating multiple sensors and ensuring seamless communication between them and the central unit might have led to unforeseen technical challenges.  

# 4.If you had to do it again, how might you change your development approach given the finite time and money resources?

## 4.1 Streamline Market Research and Targeting

Primary Users: Concentrate on segments with immediate and high demand, such as large event organizers and rental companies, which can provide early revenue streams.

## 4.2 Optimize Hardware and Technology Choices

Choose sensors with established performance records and community support to ensure reliability and ease of integration.

## 4.3 Prioritize Security and Compliance Strategically

Ensure secure data transmission using standard encryption protocols without overcomplicating the architecture.

## 4.4 Simplify User Interface and Experience

Focus on displaying only the most critical information and functionalities in the user interface to reduce complexity.

# 5. Would you change your system design after this development cycle?

## 5.1 Wireless Communication Protocol

Initial Choice: LTE-M/NB-IoT  

Pros:  

Wide Coverage: LTE-M and NB-IoT offer extensive coverage, making them suitable for outdoor deployments where mobile restrooms are frequently moved.  
Low Power Consumption: Both protocols are designed for low power usage, extending the battery life of IoT devices.  
Scalability: They support a large number of devices, facilitating the management of multiple restroom units.  

Cons:  

Latency: These protocols may introduce higher latency compared to alternatives like LoRaWAN, which could impact real-time data transmission.  
Cost: LTE-M/NB-IoT can be more expensive in terms of data plans, especially for deployments with a large number of devices sending frequent updates.  
Dependency on Cellular Networks: Reliance on existing cellular infrastructure may limit deployment in remote areas with poor network coverage.  

Recommended Changes:  

Wi-Fi 6 or 6E. Pros: Higher data rates and lower latency, beneficial for real-time monitoring and high-density deployments. Cons: Higher power consumption and reliance on local Wi-Fi infrastructure.

## 5.2 Sensors and Actuators

Recommended Changes: Infrared (IR) Sensors or Ultrasonic Sensors: For more reliable and accurate user occupancy detection, reducing dependency on door movements which may not always correlate with actual usage.

## 5.3 Target Market Alignment

Challenges Faced:  
Slower Adoption Rates: Potential customers were hesitant to adopt the new technology without sufficient education and proven benefits.  
Market Misalignment: Some segments may have different priorities or requirements that were not fully addressed by the initial product design.  

Recommended Changes:  
Additional User Segments: Include smaller event organizers, temporary installations for disaster relief, outdoor recreational facilities, and private businesses (e.g., food trucks, pop-up shops).  
Geographical Diversification: Consider expanding focus to regions with growing infrastructure projects or frequent events, such as Latin America and Southeast Asia.

## 5.4 Images of our MVP Device  

1. Get the Device's Location
![Get Location](./images/Location2.png)
![Get Location](./images/Location.png)

2. Measuring the Air Quality
![Air Quality](./images/AirQuality.png)

3. Simulate Door Openings
![Door](./images/DoorOpenings.png)

4. Upload to Memfault
![Door](./images/Memfault.png)

## 5.5 A video of the Core Product Function  

[Core Product Function](https://drive.google.com/file/d/11ecXrXUUzbfoC3DiXIjPaw3_1XLnYxOT/view?usp=sharing)

Note: The functionalities demonstrated in the video include:  

- Retrieving the device's location (longitude and latitude).
- Measuring the air quality inside the restroom.
- Recording the number of door openings in the restroom.
- Uploading all this data to Memfault.  
