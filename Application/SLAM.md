**\[22]. Transforming Omnidirectional RGB-LiDAR data into 3D Gaussian Splatting**

* 🧑‍🎓 **Author**：Semin Bae, Hansol Lim, Jongseong Brad Choi
* 🔗 **Link**：\[[arXiv:2603.06061](https://arxiv.org/abs/2603.06061)]
* 🤔 **Challenge**：Multi-sensor data (RGB and LiDAR) is often underutilized in 3DGS due to non-linear distortions in omnidirectional cameras and the lack of automated cross-modal alignment pipelines.
* 📖 **Introduction**：The paper establishes a robust modality-bridging workflow that synchronizes LiDAR point clouds with omnidirectional RGB streams for 3DGS initialization. It introduces a PRISM-based color-stratified downsampling strategy to optimize Gaussian density, enabling high-fidelity digital twin construction from routine autonomous vehicle logs.



**\[21]. FeatureSLAM: Feature-enriched 3D gaussian splatting SLAM in real time**

* 🧑‍🎓 **Author**：Christopher Thirgood, Oscar Mendez, Erin Ling, Jon Storey, Simon Hadfield
* 🔗 **Link**：\[[arXiv:2601.05738](https://arxiv.org/abs/2601.05738)]
* 🤔 **Challenge**：Traditional SLAM systems provide only geometric or photometric maps, lacking the deep semantic understanding required for open-set interaction and complex downstream tasks.
* 📖 **Introduction**：FeatureSLAM unifies camera tracking with feature-enriched mapping by integrating dense feature rasterization aligned with foundation models (e.g., DINOv2) into the 3DGS pipeline. It enables real-time open-set semantic segmentation and feature-guided GICP tracking, which improves localization accuracy beyond simple RGB-D supervision.



**\[20]. RGS-SLAM: Robust Gaussian Splatting SLAM with One-Shot Dense Initialization**

* 🧑‍🎓 **Author**：Wei-Tse Cheng, Yen-Jen Chiou, Yuan-Fu Yang
* 🔗 **Link**：\[[arXiv:2601.00705](https://arxiv.org/abs/2501.05242)]
* 🤔 **Challenge**：Standard 3DGS-SLAM relies on residual-driven densification, which causes non-stationary optimization objectives, slow convergence, and tracking instability in low-texture regions.
* 📖 **Introduction**：This paper proposes a one-shot dense initialization method using Dense Feature Matching (DFM) to triangulate a complete Gaussian set before optimization begins. This approach replaces incremental densification, leading to 20% faster convergence and 30% reduction in pose drift while maintaining high real-time throughput of up to 925 FPS.



**\[19]. SEGS-SLAM: Structure-enhanced 3D Gaussian Splatting SLAM with Appearance Embedding (ICCV/2025)**

* 🧑‍🎓 **Author**：Tianci Wen, Zhiang Liu, Yongchun Fang
* 🔗 **Link**：\[[arXiv:2501.05242](https://arxiv.org/abs/2501.05242)]
* 🤔 **Challenge**：Existing 3DGS-SLAM methods often fail to capture fine-grained underlying structures, leading to structural inconsistencies and visual artifacts during abrupt appearance or lighting variations.
* 📖 **Introduction**：This work introduces a structure-enhanced mapping framework that leverages highly structured point cloud priors to initialize 3D Gaussians for improved rendering quality. It integrates appearance embeddings to handle environmental lighting changes, achieving a significant 19.86% PSNR improvement over state-of-the-art monocular methods on the TUM RGB-D dataset.



**\[18]. WildGS-SLAM: Monocular Gaussian Splatting SLAM in Dynamic Environments (CVPR 2025)**

* 🧑‍🎓 **Author**：Jianhao Zheng, Zihan Zhu, Valentin Bieri, Marc Pollefeys, Songyou Peng, Iro Armeni
* 🔗 **Link**：\[[arXiv:2504.03886](https://arxiv.org/abs/2504.03886)]
* 🤔 **Challenge**：Monocular 3DGS SLAM systems are highly fragile in dynamic environments; moving objects disrupt the photometric consistency assumption, leading to tracking drift and mapping artifacts. Additionally, handling the inherent depth uncertainty in monocular setups remains a significant difficulty.
* 📖 **Introduction**：WildGS-SLAM proposes a monocular Gaussian SLAM system tailored for dynamic environments. Instead of relying on heavy deep learning networks, it employs a purely geometric approach to handle dynamic objects. By introducing an "uncertainty-aware" tracking and mapping mechanism, the system automatically identifies and filters out dynamic outliers. This enables robust pose estimation and clean static background reconstruction in highly dynamic wild scenes using solely monocular RGB input.



**\[17]. MAGiC-SLAM: Multi-Agent Gaussian Globally Consistent SLAM (CVPR 2025)**

* 🧑‍🎓 **Author**：Vladimir Yugay, Theo Gevers, Martin R. Oswald
* 🔗 **Link**：\[[https://openaccess.thecvf.com/content/CVPR2025/papers/Yugay\_MAGiC-SLAM\_Multi-Agent\_Gaussian\_Globally\_Consistent\_\_SLAM\_CVPR\_2025\_paper.pdf](https://openaccess.thecvf.com/content/CVPR2025/papers/Yugay_MAGiC-SLAM_Multi-Agent_Gaussian_Globally_Consistent__SLAM_CVPR_2025_paper.pdf)]
* 🤔 **Challenge**：Single-agent SLAM is limited in exploration speed and scale; however, achieving global consistency in multi-agent systems is difficult due to trajectory drift, communication bandwidth constraints, and the challenge of merging distinct Gaussian sub-maps without artifacts.
* 📖 **Introduction**：MAGiC-SLAM is a multi-agent SLAM system that enables scalable and globally consistent environment reconstruction. It employs a centralized server architecture where agents send lightweight image features and Gaussian sub-maps. The server performs loop closure detection and pose graph optimization to correct drift, followed by a novel map-merging mechanism that unifies the sub-maps into a single coherent Gaussian representation, enabling real-time collaborative exploration and high-fidelity rendering.



**\[16]. RTG-SLAM: Real-time 3D Reconstruction at Scale Using Gaussian Splatting (SIGGRAPH 2024)**

* 🧑‍🎓 **Author**：Zhexi Peng, Tianjia Shao, Yong Liu, Jingke Zhou, Yin Yang, Jingdong Wang, Kun Zhou
* 🔗 **Link**：\[[arXiv:2404.19706](https://arxiv.org/abs/2404.19706)]
* 🤔 **Challenge**：Applying 3DGS to large-scale real-time SLAM faces bottlenecks in memory usage and optimization speed; standard Gaussians can become redundant (multiple semi-transparent splats representing one surface), leading to "overdraw" and high computational costs.
* 📖 **Introduction**：RTG-SLAM introduces a compact Gaussian representation specifically designed for scalable real-time reconstruction. It enforces a "binary opacity" strategy where Gaussians are encouraged to be either opaque (surface) or transparent, and renders depth differently from color to ensure a single layer fits the surface well. Combined with an efficient on-the-fly optimization scheme that categorizes Gaussians into "stable" and "unstable," it achieves reconstruction speeds twice as fast as NeRF-based methods with half the memory footprint.



**\[15]. SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM (ECCV 2024)**

* 🧑‍🎓 **Author**：Mingrui Li, Shuhong Liu, Heng Zhou, Guohao Zhu, Na Cheng, Tianchen Deng, Hongyu Wang
* 🔗 **Link**：\[[arXiv:2402.03246](https://arxiv.org/abs/2402.03246)]
* 🤔 **Challenge**：Most 3DGS SLAM systems only reconstruct geometry and appearance, lacking semantic understanding; meanwhile, NeRF-based semantic SLAM systems often produce over-smoothed object edges and struggle with real-time performance.
* 📖 **Introduction**：SGS-SLAM is the first semantic dense SLAM framework based on 3D Gaussian Splatting. It incorporates appearance, geometry, and semantic features into a multi-channel optimization process. By using a semantic-guided keyframe selection strategy and a unique semantic feature loss, it achieves high-fidelity reconstruction with precise object-level segmentation, overcoming the limitations of previous neural implicit methods.



**\[14]. CG-SLAM: Efficient Dense RGB-D SLAM in a Consistent Uncertainty-aware 3D Gaussian Field (CVPR 2024)**

* 🧑‍🎓 **Author**：Jiarui Hu, Xianhao Chen, Boyin Feng, Guanglin Li, Liangjing Yang, Hujun Bao, Guofeng Zhang, Zhaopeng Cui
* 🔗 **Link**：\[[arXiv:2403.16095](https://arxiv.org/abs/2403.16095)]
* 🤔 **Challenge**：Naive 3DGS SLAM often suffers from "floaters" (artifacts in unobserved areas), inconsistent geometry, and unbounded memory usage as the map grows indefinitely over time.
* 📖 **Introduction**：CG-SLAM focuses on consistency and efficiency by building an uncertainty-aware 3D Gaussian field. It explicitly models the uncertainty of Gaussians to select informative primitives and prune unstable or redundant ones. Additionally, it employs specific geometric regularization terms to ensure alignment between depth and color rendering, achieving state-of-the-art tracking performance (up to 15 Hz) while maintaining a clean and compact map.



**\[13]. Gaussian Splatting SLAM (CVPR 2024)**

* 🧑‍🎓 **Author**：Hidenobu Matsuki, Riku Murai, Paul H.J. Kelly, Andrew J. Davison
* 🔗 **Link**：\[[arXiv:2312.06741](https://arxiv.org/abs/2312.06741)]
* 🤔 **Challenge**：Monocular SLAM is the hardest setup due to scale ambiguity and lack of depth; applying 3DGS directly is difficult because it typically requires accurate poses from offline Structure-from-Motion (SfM) to converge.
* 📖 **Introduction**：Often referred to as "MonoGS," this is the first system to apply 3D Gaussian Splatting to monocular SLAM. It formulates camera tracking via direct optimization against the 3D Gaussians and introduces geometric verification to handle ambiguities in incremental reconstruction. The system unifies tracking, mapping, and rendering into a single Gaussian representation, enabling live 3fps operation and high-fidelity reconstruction from a single camera without external depth sensors.



**\[12]. SplaTAM: Splat, Track \& Map 3D Gaussians for Dense RGB-D SLAM (CVPR 2024)**

* 🧑‍🎓 **Author**：Nikhil Keetha, Jay Karhade, Krishna Murthy Jatavallabhula, Gengshan Yang, Sebastian Scherer, Deva Ramanan, Jonathon Luiten
* 🔗 **Link**：\[[arXiv:2312.02126](https://arxiv.org/abs/2312.02126)]
* 🤔 **Challenge**：Implicit representations (like NeRF) are difficult to edit, slow to optimize, and lack explicit geometric bounds, while existing dense SLAM methods often struggle to balance speed with high-fidelity reconstruction.
* 📖 **Introduction**：SplaTAM is a foundational RGB-D SLAM system that replaces implicit neural networks with an explicit volumetric representation using 3D Gaussians. It employs a silhouette mask to efficiently capture scene density and utilizes a simple online tracking and mapping system tailored to Gaussians. This approach enables dense optimization and fast rendering (up to 400 FPS), allowing for structured map expansion and superior reconstruction quality compared to prior implicit methods.



**\[11]. EGS-SLAM: RGB-D Gaussian Splatting SLAM with Events**

* 🧑‍🎓 **Author**：Siyu Chen, Shenghai Yuan, Thien-Minh Nguyen, Zhuyu Huang, Chenyang Shi, Jin Jing, Lihua Xie
* 🔗 **Link**：\[[arXiv:2508.07003](https://arxiv.org/abs/2508.07003)]
* 🤔 **Challenge**：Standard RGB-D SLAM fails in high-speed motion scenarios due to motion blur, while event cameras (which have high temporal resolution) are sparse and lack texture, making it difficult to produce photorealistic reconstructions.
* 📖 **Introduction**：EGS-SLAM fuses event data with RGB-D inputs to handle motion blur and fast dynamics. It explicitly models the camera's continuous trajectory during exposure time to deblur images using event data. Simultaneously, it uses a unified Gaussian representation that is optimized by both the deblurred images and the event stream, achieving robust tracking and high-fidelity reconstruction even in severe motion blur conditions.



**\[10]. VPGS-SLAM: Voxel-based Progressive 3D Gaussian SLAM in Large-Scale Scenes**

* 🧑‍🎓 **Author**：Tianchen Deng, Wenhua Wu, Weidong Chen
* 🔗 **Link**：\[[arXiv:2505.18992](https://arxiv.org/abs/2505.18992)]
* 🤔 **Challenge**：Maintaining a globally consistent Gaussian map in large-scale scenes is memory-intensive and prone to tracking failure; existing submap-based methods may suffer from boundary artifacts or slow retrieval speeds.
* 📖 **Introduction**：VPGS-SLAM proposes a voxel-based progressive mapping strategy. It divides the space into voxels, where each voxel manages its own set of Gaussians. As the camera moves, the system progressively activates and deactivates voxels, ensuring constant-time tracking complexity and efficient memory usage. This allows for seamless transitions between submaps and robust performance in extended large-scale trajectories.



**\[9]. Large-Scale Gaussian Splatting SLAM (ICRA 2025)**

* 🧑‍🎓 **Author**：Zhe Xin, Chenyang Wu, Penghui Huang, Yanyong Zhang, Yinian Mao, Guoquan Huang
* 🔗 **Link**：\[[arXiv:2505.09915](https://arxiv.org/abs/2505.09915)]
* 🤔 **Challenge**：Scaling 3DGS SLAM to large environments is difficult due to memory limitations and drift; a single global Gaussian map becomes unmanageable, and standard frame-to-frame tracking drifts significantly over long trajectories.
* 📖 **Introduction**：This paper, termed LSG-SLAM, presents a large-scale stereo visual SLAM system. It divides the scene into continuous "Gaussian Submaps" to manage memory and scale. It introduces a "feature-alignment warping constraint" to improve tracking robustness against appearance similarities and employs a global optimization backend that merges submaps via loop closure, enabling consistent reconstruction of city-scale environments.



**\[8]. HI-SLAM2: Geometry-Aware Gaussian SLAM for Fast Monocular Scene Reconstruction**

* 🧑‍🎓 **Author**：Wei Zhang, Qing Cheng, David Skuddis, Niclas Zeller, Daniel Cremers, Norbert Haala
* 🔗 **Link**：	\[[arXiv:2411.17982](https://arxiv.org/abs/2411.17982)]
* 🤔 **Challenge**：Monocular 3DGS SLAM systems often suffer from scale ambiguity and geometric distortion; purely photometric losses are insufficient to constrain the geometry of the Gaussians, leading to "floaters" and inaccurate surface reconstruction.
* 📖 **Introduction**：HI-SLAM2 introduces a geometry-aware optimization strategy for monocular Gaussian SLAM. It incorporates geometric regularization terms (such as depth consistency and normal alignment) into the Gaussian optimization process. This ensures that the reconstructed map is not only visually pleasing but also geometrically accurate, enabling fast and high-quality scene reconstruction from a single camera.



**\[7]. GSPR: Multimodal Place Recognition Using 3D Gaussian Splatting for Autonomous Driving**

* 🧑‍🎓 **Author**：Zhangshuo Qi, Junyi Ma, Jingyi Xu, Zijie Zhou, Luqi Cheng, Guangming Xiong
* 🔗 **Link**：\[[arXiv:2410.00299](https://arxiv.org/abs/2410.00299)]
* 🤔 **Challenge**：Place recognition in autonomous driving is critical for loop closure but challenging due to viewpoint changes and environmental variations. Existing methods using 2D images or point clouds separately struggle to capture the comprehensive structural and textural information of a scene.
* 📖 **Introduction**：GSPR exploits 3D Gaussian Splatting as a unified scene representation for multimodal place recognition. It constructs a "Multimodal Gaussian Splatting" (MGS) representation combining LiDAR geometry and visual appearance. A custom network with 3D graph convolutions and transformers then extracts global descriptors from these Gaussian scenes, significantly improving place recognition accuracy compared to unimodal approaches.



**\[6]. RGB-Only Gaussian Splatting SLAM for Unbounded Outdoor Scenes (ICRA 2025)**

* 🧑‍🎓 **Author**：Sicheng Yu, Chong Cheng, Yifan Zhou, Xiaojun Yang, Hao Wang
* 🔗 **Link**：\[[arXiv:2502.15633](https://arxiv.org/abs/2502.15633)]
* 🤔 **Challenge**：Most 3DGS-based SLAM systems rely on depth sensors (RGB-D) and fail in unbounded outdoor scenarios where depth is unavailable; estimating accurate depth and scale solely from RGB images for Gaussian initialization is highly unstable.
* 📖 **Introduction**：Also known as OpenGS-SLAM, this method proposes an RGB-only pipeline tailored for unbounded outdoor scenes. It utilizes a "pointmap regression network" to generate consistent geometry across frames for pose estimation and initialization. By integrating this with an end-to-end differentiable rendering pipeline, it simultaneously optimizes camera poses and scene parameters, achieving high-fidelity outdoor mapping without LiDAR or depth sensors.



**\[5]. LiV-GS: LiDAR-Vision Integration for 3D Gaussian Splatting SLAM in Outdoor Environments**

* 🧑‍🎓 **Author**：Xiaolei Lang, Jiajun Lv, Kai Tang, Xingxing Zuo
* 🔗 **Link**：\[[arXiv:2411.12185](https://arxiv.org/abs/2411.12185)]
* 🤔 **Challenge**：Applying 3DGS to large-scale outdoor SLAM is difficult because sparse LiDAR data does not naturally align with the continuous Gaussian representation, and visual-only initialization often fails in open, texture-poor areas.
* 📖 **Introduction**：LiV-GS is an outdoor SLAM system that tightly couples LiDAR and visual data. It adaptively initializes 3D Gaussians from LiDAR measurements to constrain scene geometry and employs a sliding window optimization to refine both the trajectory and the Gaussian map. This integration ensures geometric accuracy from LiDAR and photorealistic appearance from vision, surpassing single-sensor baselines.



**\[4]. LoopSplat: Loop Closure by Registering 3D Gaussian Splats (3DV 2025)**

* 🧑‍🎓 **Author**：Liyuan Zhu, Yue Li, Erik Sandström, Shengyu Huang, Konrad Schindler, Iro Armeni
* 🔗 **Link**：\[[arXiv:2408.10154](https://arxiv.org/abs/2408.10154)]
* 🤔 **Challenge**：Standard Gaussian Splatting SLAM lacks a robust loop closure mechanism; traditional point cloud registration methods (like ICP) are not directly applicable to the splat representation, leading to accumulated drift and inconsistent maps over long trajectories.
* 📖 **Introduction**：LoopSplat introduces a novel loop closure module that registers 3D Gaussian submaps directly. Instead of converting splats to meshes or points, it aligns two Gaussian representations by minimizing a 3D-to-3D registration energy function tailored for splats. This allows the system to correct drift and merge maps globally, ensuring consistent large-scale reconstruction.



**\[3]. Photo-SLAM: Real-Time Simultaneous Localization and Photorealistic Mapping for Monocular, Stereo, and RGB-D Cameras (CVPR 2024)**

* 🧑‍🎓 **Author**：Huajian Huang, Longwei Li, Hui Cheng, Sai-Kit Yeung
* 🔗 **Link**：\[[arXiv:2311.16728](https://arxiv.org/abs/2311.16728)]
* 🤔 **Challenge**：Existing SLAM systems typically struggle to balance localization accuracy with photorealistic mapping quality; purely geometric SLAM lacks visual fidelity, while NeRF-based SLAM is computationally heavy and often fails to run in real-time on embedded devices.
* 📖 **Introduction**：Photo-SLAM presents a modular framework that decouples tracking and mapping by using "Hyper Primitives"—combining explicit geometric features (ORB) for robust localization with a 3D Gaussian map for photorealistic rendering. This hybrid approach enables state-of-the-art rendering quality and real-time performance on varied hardware (from PCs to embedded systems) across monocular, stereo, and RGB-D settings.



**\[2]. GS-SLAM: Dense Visual SLAM with 3D Gaussian Splatting (CVPR 2024)**

* 🧑‍🎓 **Author**：Chi Yan, Delin Qu, Dong Wang, Dan Xu, Zhigang Wang, Bin Zhao, Xuelong Li
* 🔗 **Link**：\[[arXiv:2311.11700](https://arxiv.org/abs/2311.11700)]
* 🤔 **Challenge**：Traditional dense SLAM methods relying on neural implicit representations (like NeRF) suffer from slow rendering speeds and expensive optimization, making them unsuitable for real-time applications that require both accurate mapping and high-fidelity re-rendering.
* 📖 **Introduction**：GS-SLAM is the first RGB-D SLAM system to utilize 3D Gaussian Splatting for both tracking and mapping. It introduces an adaptive expansion strategy to dynamically add or prune Gaussians based on geometric errors and coverage, enabling the system to efficiently reconstruct new scene geometry while maintaining a compact map size and achieving real-time performance.



**\[1]. MM-Gaussian: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes (IROS 2024)**

* 🧑‍🎓 **Author**：Chenyang Wu, Yifan Duan, Xinran Zhang, Yu Sheng, Jianmin Ji, Yanyong Zhang
* 🔗 **Link**：\[[arXiv:2404.04026](https://arxiv.org/abs/2404.04026)]
* 🤔 **Challenge**：In large-scale unbounded scenes, single-modal SLAM often fails; camera-only methods suffer from depth ambiguity, while LiDAR-only methods lack texture and color information, making it difficult to achieve both precise localization and high-fidelity photorealistic reconstruction simultaneously.
* 📖 **Introduction**：MM-Gaussian proposes a multi-modal fusion framework that integrates LiDAR and camera data into a unified 3D Gaussian representation. It utilizes LiDAR point clouds to initialize Gaussians, providing accurate geometry, while optimizing color and texture from images. This tight coupling allows for robust tracking in challenging lighting conditions and enables high-quality real-time rendering of large-scale outdoor environments.

