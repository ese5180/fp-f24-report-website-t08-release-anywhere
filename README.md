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
Clear Software Functionality:  

Real-Time Monitoring and Alerts: Implementing real-time GPS tracking and alert systems ensures that maintenance staff can respond promptly to issues, enhancing operational efficiency.
Power Monitoring: Monitoring battery status and sending low-power alerts adds a layer of reliability, ensuring that the system remains functional when needed.
User-Centric Design:  

System Administrators and Maintenance Staff: Clearly defining user roles ensures that the software meets the specific needs of different stakeholders, facilitating ease of use and effective management.  
Scalable and Secure Communication:  

LTE-M/NB-IoT Connectivity: Utilizing reliable and low-power communication technologies ensures that your system can maintain continuous connectivity with minimal energy consumption.  
Secure Data Transmission: Emphasizing secure data transmission protocols protects against potential breaches, maintaining the integrity and confidentiality of your system's data.  