# Smart Agriculture System

## Introduction

The Smart Agriculture System is an IoT-based project designed to automate and optimize farming. It uses NodeMCU and Arduino microcontrollers paired with various sensors to monitor soil moisture, temperature, and humidity in real-time. Based on this sensor data, the system automatically controls irrigation, helping farmers save water, reduce manual work, and improve crop growth.

## Project Objectives

* 
**Automate Irrigation:** Streamline the watering process.


* 
**Real-Time Monitoring:** Track environmental conditions constantly.


* 
**Resource Optimization:** Optimize water usage efficiently.


* 
**Reduce Dependency:** Lower human effort and manual intervention.



## Hardware Components

The project is built using the following components:

* **NodeMCU:** Fetches API data, specifically weather forecasts.
* **Arduino UNO:** Acts as the main controller for the sensors and the water pump.
* **Soil Moisture Sensor:** Detects the dryness of the soil.
* **DHT11 Sensor:** Reads ambient temperature and humidity.
* **LDR Sensor:** Measures sunlight intensity.
* **Servo Motor:** Controls a shade mechanism based on sunlight levels.
* **Relay Module & Water Pump:** Manages the irrigation flow.
* **LCD (I2C):** Displays real-time temperature and moisture readings.

## System Working Logic

The system operates using a coordinated logic flow between the microcontrollers and cloud data:

1. The **NodeMCU** fetches the current weather forecast using the OpenWeatherMap API.


2. If the probability of rain is greater than 50%, the NodeMCU sends a warning signal to the **Arduino**.


3. The **Arduino** then evaluates multiple real-time conditions:
* Is the soil dry? 


* Is the temperature high and humidity low? 


* Is rain predicted soon? 


4. Based on these combined parameters, the Arduino automatically turns the water pump ON or OFF.



## Key Features

* 
**Automated Irrigation:** The water pump activates automatically when soil moisture falls below a set threshold.


* 
**Real-Time Environmental Monitoring:** The system continuously measures soil moisture, temperature, and humidity using its sensors.


* 
**Energy Efficient:** The system operates only when necessary, reducing both power and water consumption.


* 
**User-Defined Thresholds:** Moisture levels can be easily configured to suit different types of crops and varying soil conditions.



## Benefits

Implementing this system provides several core advantages:

* Conserves water resources.
* Saves valuable time for farmers.
* Protects crops from harsh weather.
* Leverages the smart use of IoT and automation.
* Promotes sustainable farming practices.

## Conclusion

The Smart Agriculture System successfully uses IoT to automate irrigation and monitor farming conditions in real-time. It is a low-cost, scalable solution that helps save water, reduce manual effort, and improve crop health, thereby promoting smarter and more sustainable farming practices.
