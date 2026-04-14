# 3D Gaussian Splatting in Autonomous Driving: A Survey of Applications and Directions

This repository is the official implementation and resource collection for the paper **"3D Gaussian Splatting in Autonomous Driving: A Survey of Applications and Directions"**, submitted to **IEEE Transactions on Intelligent Transportation Systems**.



We aim to systematically outline the key contributions and latest advancements of 3D Gaussian Splatting (3DGS) in autonomous driving. This project will be continuously updated to track frontier research.

## 📝 Abstract

With the rapid development of autonomous driving technology, the understanding and interaction of the driving environment, as a core component, has increasingly higher requirements for real-time performance and accuracy. **3D Gaussian Splatting (3DGS)**, as an efficient 3D scene reconstruction method, features real-time rendering, high-fidelity reconstruction, and flexible editing capabilities. It can significantly enhance the accuracy of perception, planning, and decision-making, and is gradually replacing implicit reconstruction methods represented by Neural Radiance Fields (NeRF), demonstrating broad application potential in the field of autonomous driving. This paper systematically outlines the key contributions and latest advancements of 3DGS in autonomous driving. We first revisit the background of 3DGS, including point-based explicit representations and NeRF, and then introduce its core principles. Subsequently, we categorize and discuss four major application areas of 3DGS in autonomous driving: **scene reconstruction, scene editing, Simultaneous Localization and Mapping (SLAM)**, and **autonomous driving simulation**. Finally, we analyze the challenges faced by 3DGS in autonomous driving applications and explore future research directions, including **structural optimization, integration with other foundation models, Space-Air-Ground Integration, Vehicle-Road-Cloud Integration**, and \*\*quantum computing. This paper aims to provide comprehensive guidance for researchers, fostering further innovation and application of 3DGS in autonomous driving.

## 🗂️ Applications Taxonomy

Based on our survey, we categorize 3DGS applications in autonomous driving into the following structure. We will update the paper list under these categories.

### 1\. Scene Reconstruction

* **Static Scene Reconstruction**: High-fidelity environmental models for HD maps.
* **Dynamic Scene Reconstruction**: Modeling moving objects (vehicles, pedestrians).
* **Large-Scale Urban Scene Reconstruction**: City-level 3D maps with memory-efficient strategies.

### 2\. Scene Editing

* **Rich and Flexible Editing**: Object removal, replacement, insertion.
* **Multimodal Fusion**: Joint editing of images and LiDAR point clouds.

### 3\. Simultaneous Localization and Mapping (SLAM)

* **LiDAR Integration**: Fusing LiDAR depth for robust initialization and tracking.
* **Low-cost Sensor Fusion SLAM**: RGB or RGBD-based low-cost sensor methods
* **Complex Outdoor Scenes**: Handling unbounded environments.

### 4\. Autonomous Driving Simulation

* **3D Asset Generation and Insertion**: Enhancing asset realism via diffusion models.
* **Physical Simulation**: Integrating kinematic and mechanical properties.
* **Sensor Simulation Testing**: Adversarial attacks and sensor modeling.
* **Autonomous Driving Simulator**: Bridging the sim-to-real gap.

## 🚀 Future Research Directions

We also track the latest works related to the future directions proposed in our survey:

### 1\. Structural Optimization

* **Sparse Data Reconstruction**
* **Memory-Efficient 3DGS**
* **Real-Time 3DGS**
* **Photo-realistic 3DGS**

### 2\. Integration with Foundation Models

* **Segment Anything Model**
* **Large Language Model**
* **Diffusion Model**

### 3\. 3D Perception and Semantic Occupancy

### 4. Space-Air-Ground Integration

### 5. Vehicle-Road-Cloud Integration

### 6. Quantum Computing

