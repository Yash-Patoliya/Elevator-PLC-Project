**Elevator (Lift) Control System Simulation Using Siemens TIA Portal and SCL**

The **Elevator Control System** is a comprehensive simulation project developed using **Siemens TIA Portal** with **Structured Control Language (SCL)** to model real-world elevator behavior. The primary goal of the project was to implement a fully functional lift system that can respond to user requests, move between floors, and control door operations, while incorporating safety and interlock logic.

The system manages **floor requests** from both cabin buttons and external buttons, storing them in dedicated request flags for each floor. It dynamically selects the **target floor** based on pending requests and current elevator position. The motor control logic ensures the elevator moves in the correct direction, stops when the target is reached, and adjusts speed depending on the distance to the target floor. A **movement simulation** assumes 5 seconds per floor, updating the elevator’s virtual position and activating floor-specific sensors to track current floor status.

**Door operations** are fully automated with timers, ensuring doors open for a fixed duration at each stop. Safety features include interlocks to prevent elevator movement when doors are open, mutual exclusion logic to avoid conflicting door signals, and the ability to manually open or close doors via cabin buttons. The system also simulates realistic operational constraints, such as speed reduction when approaching the next floor and resetting cabin and hall buttons after serving requests.

This project emphasizes **modularity and scalability**, making it easy to extend for additional floors or integrate new features like priority requests or emergency stop functionality. The SCL code is organized with clear comments, logical structure, and the use of timers, conditional statements, and boolean logic to simulate realistic industrial control behavior.

💡 Feel free to use this code as a learning resource or a base for your own projects. You can adapt, expand, and edit it as per your imagination to simulate more complex elevator systems or other industrial automation applications.
