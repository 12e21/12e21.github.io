---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a third year undergraduate student from [School of Cyber Security](https://wlkjaqxy.nwpu.edu.cn/), [Northwestern Polytechnical University](https://www.nwpu.edu.cn/).
My research interest includes 3D Vsion, Embodied AI, Robotics.

I am very fortunate to be advised by [Prof. Jiaqi Yang](https://yangjiaqihomepage.github.io/) of [ASGO Lab](https://asgo.nwpu.edu.cn/) from School of Computer Science, Northwestern Polytechnical University.

You can find my CV here: [Bingqian Wu's Curriculum Vitae](../assets/Curriculum_Vitae.pdf)

[Email](mailto:2496813401@qq.com) / [Github](https://github.com/12e21) / [Wechat](../images/wechat.jpg)

## Experience
- 2022.09-present, Undergraduate, School of Cyber Security, Northwestern Polytechnic University, Xi’an, Shaanxi Province, China.
- 2022.10-present, Drone Software Team Leader, Northwestern Polytechnic University V5++ robotics team
- 2023.11-present, Research Intern, advised by [Prof. Jiaqi Yang](https://yangjiaqihomepage.github.io/) ,ASGO-3DV Lab at Northwestern Polytechnic University

## Awards
- 2022-2023 Second Class Scholarship for Outstanding Students of Northwestern Polytechnical University
- 2023-2024 First Class Scholarship for Outstanding Students of Northwestern Polytechnical University
- 2023-2024 Xiaomi Scholarship

## Competitions
- First Prize in the Robot Mission Challenge (Micro UAV) of the 25th China Robot and Artificial Intelligence Competition
- Second Prize in the 2023 China Robot Competition and ROBOCUP Robot World Cup China Drone Challenge
- First Prize in the Robot Mission Challenge (Micro UAV) of the 26th China Robot and Artificial Intelligence Competition
- Second Prize in the 2024 China Robot Competition and ROBOCUP Robot World Cup China Drone Challenge

## Projects
### 1. MMreifne
During my research internship at the **ASGO Laboratory** of Northwestern Polytechnical University, I focused on advancing **3D object detection**. Here, I independently designed and implemented the **MMrefine framework**, which significantly enhanced the performance of 3D object detection. This framework employs a multi-branch and multi-stage refinement approach to address issues related to uneven point cloud distribution and incomplete point clouds. 

The effectiveness of MMrefine was demonstrated through significant improvements on the **KITTI dataset**, one of the most renowned benchmarks for evaluating autonomous driving technologies. The research findings have been submitted for publication in the esteemed **IEEE Robotics and Automation Letters (RAL)** journal, highlighting the innovative nature and impact of this work.

Here is the [code](https://github.com/12e21/MMrefine).

![MMrefine_pipeline](./images/projects/MMrefine_pipeline.png)

### 2. Drone-Based Parcel Delivery Project

In the **Drone-Based Parcel Delivery** project, I took the lead in developing the software strategies essential for the drone's autonomous operations. Utilizing **ROS (Robot Operating System)** alongside the **MAVROS PX4** interface, I implemented key functionalities including autonomous flight, path planning, and obstacle avoidance mechanisms. These capabilities were crucial for ensuring the drone could navigate efficiently and safely to its destination.

Furthermore, I was responsible for designing and implementing **mission strategy functions**, which enabled the drone to successfully execute parcel delivery tasks. This involved not only reaching the target location accurately but also managing the release of the parcel at the designated drop-off point. The successful completion of these missions demonstrated the effectiveness of the developed strategies in real-world applications.

Since the code is for a competition, I cannot publish the code.

![uav_deliver](./images/projects/uav_deliver.png)

### 3. Multi-Drone Simulation for Target Tracking Project

As the **Project Leader** in the **Multi-Drone Simulation for Target Tracking** project, I designed and implemented a comprehensive multi-drone cooperative target tracking framework. This framework integrates several advanced technologies to achieve effective, precise, and sustainable target tracking.

- **Navigation and Obstacle Avoidance**: Utilizing **MoveBase** along with **2D LiDAR** sensors for navigation and obstacle avoidance, ensuring safe and efficient drone movement.
- **Target Detection**: Employing **YOLOv8** for real-time object detection, providing accurate identification of targets within the operational area.
- **Visual Servoing**: Implementing visual servoing through gimbal cameras and image Jacobian matrices for proportional control, allowing drones to maintain focus on the moving targets.
- **Coordinate Transformation**: Applying **Direct Linear Transformation (DLT)** to transform target coordinates from the 2D camera frame to the 3D world coordinate system, enhancing the accuracy of target localization.

This integrated approach enabled the drones to perform robust and precise target tracking, demonstrating significant advancements in autonomous drone operations. The successful implementation of this framework highlights its potential for various applications, including surveillance, search and rescue missions, and more.

Since the code is for a competition, I cannot publish the code.

![uav_track](./images/projects/uav_track.png)

### 4. LLM-Controlled Drone Project

In the **LLM-Controlled Drone** project, I designed a **state machine-based task execution system** that translates natural language commands into actionable drone operations. This innovative approach leverages a **task command set** and integrates with large language models (LLMs) via **LangChain** to bridge the gap between human instructions and drone actions.

#### Key Features:
- **State Machine Design**: A robust state machine was developed to manage different stages of drone tasks, ensuring smooth transitions and reliable execution.
- **Task Command Set**: A predefined set of commands was created to cover various drone operations, enabling precise control over the drone's activities.
- **Integration with LLMs**: By interfacing with LLM APIs through **LangChain**, the system can interpret complex natural language inputs and convert them into executable drone actions.
- **Control System**: The overall architecture facilitates a seamless flow from **natural language input** to **LLM processing** and finally to **drone action execution**, making the drone operation intuitive and user-friendly.

This system significantly enhances the usability and flexibility of drones by allowing users to control them through simple, conversational commands rather than requiring technical expertise. It opens up new possibilities for applications such as automated inspections, surveillance, and delivery services.

Here is the [code](https://github.com/12e21/llm_interface).

![uav_llm](./images/projects/uav_llm.png)
