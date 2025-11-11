# Luca's Engineering Portfolio

Welcome to my GitHub portfolio!  
Here, I showcase my work in **Embedded Systems** and **Robotics**, completed during university and personal projects.

---

# 🔹 Embedded Projects
ARM Cortex-M | Bare-Metal | RTOS | Driver Development | Debugging  
[Embedded_Projects Repository](https://github.com/BrenzingerLuca/Embedded-Projects)

- Bare-Metal LED Blink – Startup code, GPIO register access
- Fault Handler Debugger – HardFault analysis, UART debugging
- GPIO & SPI Driver – Custom peripheral drivers
- I2C Temperature Logger – Sensor reading, UART output
- RTOS Demo – FreeRTOS tasks, timers, UART
- Trace Logger – Software tracing, analysis with OpenOCD
- GDB Automation Script – Register dumps, debugger scripts

---
#🔹 Team23_I2ROS_2025: Autonomous Driving System (University Project)

This repository contains the documentation and source code for our **autonomous driving system**, developed as part of a university course on **Introduction to ROS** during the summer term of 2025.

Our team engineered a comprehensive solution for self-driving within a simulated urban environment. The primary objective was to build a robust system capable of **real-time navigation, traffic light compliance, and collision avoidance** using **ROS (Robot Operating System)** and a **Unity-based simulator**.

## Key Learnings & Project Highlights

This project provided invaluable hands-on experience and a deep dive into advanced robotics and AI concepts:

*   **ROS (Robot Operating System):** Gained a strong understanding of ROS architecture, including node communication, topics, services, and the orchestration of complex robotic systems via launch files.
*   **Autonomous Driving Concepts:** Practical application of fundamental algorithms for perception, path planning, trajectory generation, and vehicle control in a simulated environment.
*   **Sensor Data Fusion:** Developed skills in processing, aligning, and fusing data from various sensors (e.g., depth images, cameras) to construct a comprehensive environmental model.
*   **Machine Learning for Perception:** Acquired practical experience in **fine-tuning and deploying YOLOv8 networks** for real-time object detection (specifically cars and traffic lights) in simulated scenarios.
*   **Simulation & Testing:** Utilized a **Unity-based simulator** for iterative development, rigorous testing, and robust validation of autonomous driving functionalities.
*   **Git & Version Control:** Mastered collaborative codebase management using Git, including efficient handling of **large binary files with Git Large File Storage (Git LFS)** and maintaining a clean, effective project history.
*   **Team Collaboration:** Successfully navigated the complexities of agile team development, clearly defining responsibilities, and seamlessly integrating individual software modules into a cohesive system.

## My Contribution (Luca Brenzinger)

As a core team member, my primary responsibilities and contributions focused on critical areas of the system, demonstrating expertise in both development and optimization:

*   **Perception Module (Lead):** I led the design and implementation of key components within the perception pipeline. This included developing the `static_tf_ins_to_cameras` node for precise sensor frame transformations and configuring the `pointcloud.launch` file for robust 3D point cloud generation.
*   **YOLOv8 Network Fine-Tuning & Data Augmentation:** I made significant contributions to the fine-tuning of the **YOLOv8 object detection model**. My work involved setting up and executing **data augmentation strategies** to enhance model generalization and training the network on custom simulation data for accurate car and traffic light detection.
*   **Object Detector Node Development:** I actively developed and refined the `object_detector` node, which continuously processes incoming images to identify objects of interest, publishing their bounding box coordinates and class labels for downstream modules.
*   **3D Car Position Estimator Node:** My involvement extended to the `car_position_estimator` node, where I contributed to estimating 3D world positions of detected cars through depth-based triangulation and visualizing these results in RViz.
*   **System Integration & Debugging:** Beyond specific module development, I played a crucial role in integrating various system components, debugging complex interactions within the ROS graph, and ensuring the overall stability and performance of the autonomous system.
*   **Documentation:** I contributed to the comprehensive project documentation, providing detailed explanations of key modules and their functionalities to ensure clarity and maintainability.

## 📌 Skills & Tools
- **Languages:** C, C++, Python
- **Embedded:** ARM Cortex-M, STM32, Bare-Metal, HAL, RTOS
- **Robotics:** ROS2, sensor integration, PID, motor control
- **Debugging:** OpenOCD, GDB, Logic Analyzer, Trace Analysis
