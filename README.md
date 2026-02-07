# Luca's Engineering Portfolio

Welcome to my GitHub portfolio!  
Here, I showcase my work in **Embedded Systems** and different **Robotics**, completed during university and personal projects.

---
#  Embedded Projects
ARM Cortex-M | Bare-Metal | RTOS | Driver Development | Debugging  
[Embedded_Projects Repository](https://github.com/BrenzingerLuca/Embedded-Projects)

---
#  Autonomous Driving Project (University Project)
![ROS](https://img.shields.io/badge/ros2-%2322314E.svg?style=for-the-badge&logo=ros&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)

This repository contains the documentation and source code for our **autonomous driving system**, developed as part of a university course on **Introduction to ROS** during the summer term of 2025.

Our team engineered a comprehensive solution for self-driving within a simulated urban environment. The primary objective was to build a robust system capable of **real-time navigation, traffic light compliance, and collision avoidance** using **ROS (Robot Operating System)** and a **Unity-based simulator**.

## Key Learnings & Project Highlights

This project provided invaluable hands-on experience and a deep dive into advanced robotics and AI concepts:

*   **ROS (Robot Operating System):** Gained a strong understanding of ROS architecture, including node communication, topics, services, and the orchestration of complex robotic systems via launch files.
*   **Autonomous Driving Concepts:** Practical application of fundamental algorithms for perception in a simulated environment.
*   **Sensor Data Fusion:** Developed skills in processing, aligning, and fusing data from depth images and cameras to construct a comprehensive environmental model.
*   **Machine Learning for Perception:** Acquired practical experience in **fine-tuning and deploying YOLOv8 networks** for real-time object detection (specifically cars and traffic lights) in simulated scenarios.
*   **Git & Version Control:** Mastered collaborative codebase management using Git, including efficient handling of **large binary files with Git Large File Storage (Git LFS)** and maintaining a clean, effective project history.
*   **Team Collaboration:** Successfully navigated the complexities of agile team development, clearly defining responsibilities, and seamlessly integrating individual software modules into a cohesive system.

## My Contribution (Luca Brenzinger)

As a core team member, my primary responsibilities and contributions focused on critical areas of the system, demonstrating expertise in both development and optimization:

*   **Perception Module (Lead):** I led the design and implementation of key components within the perception pipeline. This included developing the `static_tf_ins_to_cameras` node for precise sensor frame transformations and configuring the `pointcloud.launch` file for robust 3D point cloud generation.
*   **YOLOv8 Network Fine-Tuning & Data Augmentation:** I made significant contributions to the fine-tuning of the **YOLOv8 object detection model**. My work involved setting up and executing **data augmentation strategies** to enhance model generalization and training the network on custom simulation data for accurate car and traffic light detection.
*   **Object Detector Node Development:** I actively developed and refined the `object_detector` node, which continuously processes incoming images to identify objects of interest, publishing their bounding box coordinates and class labels for downstream modules.
*   **3D Car Position Estimator Node:** My involvement extended to the `car_position_estimator` node, where I contributed to estimating 3D world positions of detected cars through depth-based triangulation and visualizing these results in RViz.
*   **Documentation:** I contributed to the comprehensive project documentation, providing detailed explanations of key modules and their functionalities to ensure clarity and maintainability.

---
#  PI-Bot: Distributed 3-DOF Robotic Arm (Personal Project)
![alt text](https://img.shields.io/badge/ros2-%2322314E.svg?style=for-the-badge&logo=ros&logoColor=white)
![alt text](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![alt text](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![alt text](https://img.shields.io/badge/-Raspberry%20Pi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)
![alt text](https://img.shields.io/badge/Qt-%2341CD52.svg?style=for-the-badge&logo=Qt&logoColor=white)

This repository contains the full source code and hardware configuration for the PI-Bot, a custom-built 3-DOF robotic arm. Developed as an end-to-end solo project, it demonstrates the integration of distributed software systems, hardware control, and a hybrid robot control system.
The system is built on a distributed ROS2 architecture, where a workstation handles high-level motion planning and a Raspberry Pi 4 manages the low-level hardware abstraction layer.

## System Demo

## Technical Highlights & Implementation

This project covers the entire robotics stack, from mechanical coordination to high-level software orchestration:

*   **Distributed ROS2 Architecture:** Engineered a multi-node system where computation is split between a **PC (running MoveIt2 & GUI)** and a **Raspberry Pi 4 (Servo/ADC nodes)**, communicating seamlessly via **ROS2 Topics and SSH**.
*   **Hybrid Control System:** Developed two distinct operational modes:
    *   **GUI-Control:** Asynchronous trajectory execution using **MoveIt2 and PySide6**.
    *   **Hardware-in-the-Loop (HIL):** Real-time manipulation via **analog potentiometers**, allowing the user to "teach" the robot movements.
*   **Custom GUI (PI-Bot Control Center):** Designed and implemented a professional dashboard using **PySide6 (Qt)**. Key features include a **Sequence Recorder** to store/execute movement patterns and **real-time state synchronization** to prevent hardware jumps.
*   **Low-Level Hardware Interfacing:** Developed custom nodes for the **MCP3008 ADC (I2C)** and **PCA9685 PWM (I2C)** to bridge the gap between analog sensors and the digital ROS2 environment.
*   **Kinematics & Digital Twin:** Created a precise **URDF model** and configured the **TF-tree** for real-time visualization in **RViz**, ensuring the digital twin perfectly reflects the physical state of the 3-DOF arm.
*   **Motion Planning:** Integrated the **MoveIt2 framework** for **inverse kinematics (IK)** and collision-free path planning, utilizing custom service interfaces for **cartesian positioning**.


## Skills & Tools
- **Languages:** C++, Python, bash, 
- **Robotics:** ROS2, sensor integration, MoveIt2, URDF
