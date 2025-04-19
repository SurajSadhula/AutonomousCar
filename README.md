# Autonomous Car

## Project Overview
In this project, we build an **Autonomous RC Car** using supervised learning of a neural network with a single hidden layer. The system utilizes a remote-controlled car equipped with a **Raspberry Pi** and a **Raspberry Pi camera module**.

- In **training mode**, the camera module captures images to train the neural network.  
- In **autonomous mode**, the trained model uses real-time camera input to predict the car's movements and direction.

---

## Hardware Components
- **Robo Car Chassis**
- **Arduino Uno**
- **Lithium-ion Batteries**
- **Power Bank**
- **L298N H-Bridge Motor Driver**
- **Raspberry Pi Model 3B+**
- **Pi Camera**
- **Servo Motors (Pan-Tilt Module)**

---

## Project Description
The autonomous car is built on a **four-wheel Robo Car chassis** with the following layers:

1. **Base Layer**:  
   - Fitted with 5–12V DC motors connected via the **L298N H-Bridge Motor Driver**.  
   - Powered by **4 lithium polymer batteries** (3.7V each, connected in series for a 12V supply).  

2. **Middle Layer**:  
   - Houses the motor driver and **power bank**, which powers the Raspberry Pi.  
   - Separate power sources are used to prevent short circuits and manage load efficiently.

3. **Top Layer**:  
   - Includes the **Raspberry Pi Model 3B+** and the **Raspberry Pi Camera Module**.  
   - The camera sends data to an external PC for image processing over Wi-Fi.  
   - Processed instructions are sent back to the Raspberry Pi to control the car's movements.  

The **Arduino Uno** receives these instructions and signals the motor driver to execute them.

---

## Components Description
### Robo Car Chassis
- Versatile chassis with mounting options for sensors, motors, and control modules.  
- Supports various robot applications like obstacle avoidance, line following, and remote-controlled systems.

### Arduino Uno
- Open-source microcontroller board based on the ATmega328P, equipped with digital and analog I/O pins for interfacing with additional components.

### Lithium-ion Batteries
- Rechargeable batteries with high capacity (2800mAh) and efficient power delivery.

### L298N H-Bridge Motor Driver
- High-voltage, high-current motor driver to control DC motors.  
- Receives TTL logic signals for operating motors or solenoids.

### Raspberry Pi 3 Model B+
- A compact computer with a 64-bit quad-core processor, dual-band Wi-Fi, and high-speed Ethernet.  
- Ideal for real-time data processing and integration with the Pi camera.

### Pi Camera Module
- Lightweight camera module compatible with Raspberry Pi.  
- Facilitates image processing for tasks like machine learning, surveillance, and robotics.

### Servo Motors (Pan-Tilt Module)
- Dual-axis movement allows camera or sensor panning and tilting.  
- Controlled via PPM pulses for precise adjustments.
