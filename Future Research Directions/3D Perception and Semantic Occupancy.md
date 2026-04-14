**\[3]. GaussianFormer3D: Multi-modal Gaussian-based Semantic Occupancy Prediction with 3D Deformable Attention**

* 🧑‍🎓 **Author**：Lingjun Zhao, Sizhe Wei, James Hays, Lu Gan
* 🔗 **Link**：\[[arXiv:2505.10685](https://arxiv.org/abs/2505.10685)]
* 🤔 **Challenge**：Fusing multi-modal data for 3D occupancy is often inefficient, and standard 3DGS-based perception lacks the ability to adaptively capture localized semantic features across different sensors.
* 📖 **Introduction**：The authors propose a multi-modal perception framework that utilizes 3D deformable attention to adaptively aggregate features from cameras and LiDAR into Gaussian primitives. By treating 3D Gaussians as unified kernels for both geometry and semantics, the model enables robust semantic occupancy prediction and enhanced multi-view consistency in challenging weather and lighting conditions.



**\[2]. GaussianFormer-2: Probabilistic Gaussian Superposition for Efficient 3D Occupancy Prediction (CVPR/2025)**

* 🧑‍🎓 **Author**：Yuanhui Huang, Amonnut Thammatadatrakoon, Wenzhao Zheng, Yunpeng Zhang, Dalong Du, Jiwen Lu
* 🔗 **Link**：\[[arXiv:2412.04384](https://arxiv.org/abs/2412.04384)]
* 🤔 **Challenge**：Traditional voxel-based occupancy methods suffer from heavy computational costs, while existing Gaussian-based methods struggle to accurately represent complex spatial probability distributions in sparse-view driving scenarios.
* 📖 **Introduction**：This paper introduces a probabilistic Gaussian superposition mechanism that models 3D occupancy as a summation of Gaussian probability density functions. By shifting the perception task from dense voxel grids to a sparse set of learnable Gaussian queries, the framework achieves high-fidelity 3D occupancy prediction with significantly reduced memory footprint and faster inference speed.



**\[1]. GaussianFormer: Scene as Gaussians for Vision-Based 3D Semantic Occupancy Prediction (ECCV/2024)**

* 🧑‍🎓 **Author**：Yuanhui Huang, Wenzhao Zheng, Yunpeng Zhang, Jie Zhou, Jiwen Lu
* 🔗 **Link**：\[[arXiv:2405.17429](https://arxiv.org/abs/2405.17429)]
* 🤔 **Challenge**：Cross-view spatial alignment in 3DGS is often suboptimal when relying solely on SfM points, especially in sparse-view driving scenarios.
* 📖 **Introduction**：This paper proposes a Transformer-based architecture that treats 3D Gaussians as learnable queries within a perception pipeline. By attending to multi-camera features, the "Gaussian-Former" refines the spatial distribution of primitives, enhancing 3D object detection and panoptic segmentation performance.

