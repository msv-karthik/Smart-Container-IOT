# Smart-Container-IOT

## Introduction

The **Smart Container** is an innovative IoT device designed to improve kitchen and inventory management. It helps monitor the quantity of items stored within containers and alerts users when supplies are running low. Additionally, it features an **expiration date tracking system** that sends notifications both visually (via LED indicators) and digitally (through an app) when the expiration date approaches. This solution addresses common issues such as **over-purchasing**, **food waste**, and the inconvenience of manually tracking stock levels, providing timely alerts and notifications to help users stay informed.

## Key Features

- **Expiry Notification**: Notifies users when the expiration date of a product is approaching.
- **Quantity Detection**: Automatically detects the amount of items left in the container.
- **Container Identification**: Provides an easy way to identify and locate specific containers.

## Components Used

The system utilizes the following components:

### 1. **Node MCU ESP8266**
- A low-cost, Wi-Fi-enabled microcontroller that connects and controls the IoT devices in the system.
  
### 2. **Ultrasonic Sensor**
- Measures the distance to an object using ultrasonic waves, ideal for detecting the quantity of contents in a container.

### 3. **LED**
- Light-emitting diodes used for visual indicators, including expiry notifications and container identification.

### 4. **LCD (Liquid Crystal Display)**
- Used to display information such as sensor readings, status messages, and expiration warnings.

### 5. **Breadboard**
- A reusable platform for prototyping and testing electronic circuits without soldering.

### 6. **Buck Converter**
- A DC-DC converter that steps down the voltage to efficiently power the components in the circuit.

## Functionality

The Smart Container IoT system provides three main functionalities:

### 1. **Expiry Notification**

#### Overview:
Managing the expiry dates of consumables is crucial for safety and quality. Often, items are forgotten until it’s too late, leading to wastage or use of expired goods. The Smart Container provides a seamless solution to monitor and alert users about approaching expiry dates.

#### How it works:
- Users input the expiry date of the content into the app.
- The app compares the entered expiry date with the current date and triggers notifications as the expiry date approaches.
- **Visual Indication**:
  - **Green Light**: 10 days before expiry.
  - **Yellow Light**: 5 days before expiry.
  - **Red Light**: On the day of expiry.
  
#### Benefits:
- Helps prevent usage of expired items.
- Provides visual reminders for timely usage.

### 2. **Quantity Detection**

#### Overview:
Tracking the quantity of items in a container is essential to ensure you never run out of supplies. Manual checks can be cumbersome and prone to errors. The Smart Container automates this process, ensuring the contents are always properly monitored.

#### How it works:
- An ultrasonic sensor measures the remaining quantity of the content.
- The sensor sends data to the app.
- The app notifies the user when the content level is low and needs refilling.
  
#### Benefits:
- Ensures that the container is always adequately filled.
- Prevents running out of essential items unexpectedly.

### 3. **Container Identification**

#### Overview:
In environments with multiple similar containers, identifying the correct one can be a challenge. This often leads to confusion and inefficiency in locating and accessing the right items. The Smart Container offers a convenient solution to this problem.

#### How it works:
- The app includes a feature to identify a specific container.
- When triggered, an LED on the corresponding container lights up.
- This makes it easy for the user to locate the required container.

#### Benefits:
- Simplifies the process of locating the correct container.
- Reduces time spent searching for specific items.

## System Architecture

The Smart Container system consists of the following components:

- **Node MCU ESP8266**: The microcontroller that connects all the sensors and LEDs, and communicates with the mobile app via Wi-Fi.
- **Ultrasonic Sensor**: Measures the content levels and sends data to the Node MCU for processing.
- **LEDs**: Provide visual notifications to the user based on expiry status and container identification.
- **LCD Screen**: Displays the status, including expiry warnings and quantity readings.
- **Mobile App**: A companion app for user interaction where expiry dates, container identification, and other information are managed.

## How to Use

1. **Set Up the Hardware**:
   - Connect the ultrasonic sensor, Node MCU, LED lights, and LCD to the breadboard and power the system.
   - Ensure the system is connected to Wi-Fi for communication with the app.

2. **Download the App**:
   - Install the Smart Container mobile app on your smartphone.
   - Register and log in to the app.

3. **Enter Expiry Dates**:
   - Input the expiry dates for each item stored in the container.
   - The app will notify you as the expiry date approaches, triggering visual alerts via the LEDs.

4. **Monitor Quantity Levels**:
   - The ultrasonic sensor will continuously monitor the quantity of contents in the container.
   - The app will notify you when the quantity is low and needs refilling.

5. **Locate Containers**:
   - When you need to find a specific container, use the app to trigger the LED light on the corresponding container.

