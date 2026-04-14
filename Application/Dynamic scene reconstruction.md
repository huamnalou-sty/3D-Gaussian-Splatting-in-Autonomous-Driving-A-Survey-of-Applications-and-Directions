**\[26]. Dynamic Gaussian Scene Reconstruction from Unsynchronized Videos (AAAI/2025)**

* 🧑‍🎓 **Author**：Zhixin Xu, Hengyu Zhou, Yuan Liu, Wenhan Xue, Hao Pan, Wenping Wang, Bin Wang
* 🔗 **Link**：\[[arXiv:2511.11175](https://arxiv.org/abs/2511.11175)]
* 🤔 **Challenge**：Most 4DGS frameworks assume input videos are perfectly synchronized, but real-world captures often suffer from temporal misalignment (network latency, manual triggers), causing severe motion blur and artifacts.
* 📖 **Introduction**：This paper proposes a coarse-to-fine optimization framework to estimate and compensate for unknown temporal offsets of each camera during the 4D reconstruction process. By integrating this module into existing 4DGS pipelines, it achieves robust, artifact-free dynamic reconstruction from asynchronous multi-view data.



**\[25]. SpeeDe3DGS: Speedy Deformable 3D Gaussian Splatting with Temporal Pruning and Motion Grouping (CVPR/2026)**

* 🧑‍🎓 **Author**：Allen Tu, Haiyang Ying, Alex Hanson, Yonghan Lee, Tom Goldstein, Matthias Zwicker
* 🔗 **Link**：\[[arXiv:2506.07917](https://arxiv.org/abs/2506.07917)]
* 🤔 **Challenge**：While dynamic extensions of 3DGS achieve high-quality results, the per-Gaussian neural inference required for deformation fields makes these models computationally expensive and memory-intensive for long sequences.
* 📖 **Introduction**：SpeeDe3DGS bridges the efficiency-fidelity gap through three modules: Temporal Sensitivity Pruning (TSP) to remove low-impact Gaussians, Temporal Sensitivity Sampling (TSS), and Motion Grouping. These contributions enable significantly faster training and rendering while maintaining high-fidelity reconstruction of monocular dynamic scenes.



**\[24]. 4DM: 4D Photorealistic Mapping from Monocular Video with 3D Gaussian Splatting**

* 🧑‍🎓 **Author**：Lizhi Bai
* 🔗 **Link**：\[[https://doi.org/10.1117/12.3094288](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/14124/3094288/4DM--4D-photorealistic-mapping-from-monocular-video-with-3D/10.1117/12.3094288.short)]
* 🤔 **Challenge**：Traditional monocular 4D reconstruction struggles with dynamic consistency and redundant sampling in new frames, often failing to maintain high visual fidelity across long sequences.
* 📖 **Introduction**：4DM is a mapping framework that transforms monocular video into 4D scenes using only 2D priors like depth and optical flow. It employs image gradient-based quad-tree sampling to minimize redundancy and K-Nearest Neighbor (KNN) densification for new Gaussian points. The pipeline alternately optimizes camera poses and Gaussian dynamics, achieving significant improvements in visual fidelity on the DAVIS dataset.



**\[23]. GC-4DGS: Geometry-Consistent 4D Gaussian Splatting for Sparse-Input Dynamic View Synthesis**

* 🧑‍🎓 **Author**：Yiwei Li, Jiannong Cao, Penghui Ruan, Divya Saxena, Songye Zhu, Yinfeng Cao
* 🔗 **Link**：\[[arXiv:2511.23044](https://arxiv.org/abs/2511.23044)]
* 🤔 **Challenge**：Dynamic scene reconstruction significantly degrades under sparse-view inputs due to the ill-posed nature of 4D geometric optimization and incoherent learning of temporal geometry.
* 📖 **Introduction**：GC-4DGS infuses geometric consistency into the 4DGS framework by utilizing a global-local depth regularization approach. It distills spatiotemporal-consistent information from monocular depth estimators and Multi-View Stereo (MVS) priors to regularize the 4D volume. The method achieves a substantial 2.62dB PSNR improvement over prior sparse-input baselines while remaining deployable on edge devices.



**\[22]. Diff4Splat: Controllable 4D Scene Generation with Latent Dynamic Reconstruction Models (CVPR/2026)**

* 🧑‍🎓 **Author**：Panwang Pan, Chenguo Lin, Jingjing Zhao, Chenxin Li, Yuchen Lin, Haopeng Li, Honglei Yan, Kairun Wen, Yunlong Lin, Yixuan Yuan, Yadong Mu
* 🔗 **Link**：\[[arXiv:2511.00503](https://arxiv.org/abs/2511.00503)]
* 🤔 **Challenge**：Most 4D reconstruction methods require time-consuming per-scene optimization and lack high-level controllability over motion and appearance. Single-image to 4D generation is often bottlenecked by the gap between 2D video diffusion priors and explicit 3D representations.
* 📖 **Introduction**：Diff4Splat is a feed-forward framework that generates a deformable 3D Gaussian field from a single image and camera trajectory in one forward pass. It leverages a Latent Dynamic Reconstruction Model (LDRM) to bridge video diffusion latents with temporal transformers, enabling real-time interaction (6.7ms rendering) and precise pose control without test-time optimization.



**\[21]. MoE-GS: Mixture of Experts for Dynamic Gaussian Splatting (ICLR/2026)**

* 🧑‍🎓 **Author**：In-Hwan Jin, Hyeongju Mun, Joonsoo Kim, Kugjin Yun, Kyeongbo Kong
* 🔗 **Link**：\[[arXiv:2510.19210](https://arxiv.org/abs/2510.19210)]
* 🤔 **Challenge**：Existing dynamic 3DGS methods often employ a single deformation prior (e.g., global MLP or local displacement), which fails to generalize across diverse motion types within a single scene. This leads to inconsistent reconstruction quality when handling complex, heterogeneous dynamics.
* 📖 **Introduction**：This paper introduces MoE-GS, the first framework to incorporate Mixture-of-Experts (MoE) into dynamic Gaussian splatting. By combining heterogeneous deformation priors through a gating mechanism, the model adaptively selects the most suitable expert for specific motion components. It consistently outperforms state-of-the-art methods on N3V and Technicolor datasets with improved efficiency.



**\[20]. ProDyG: Progressive Dynamic Scene Reconstruction via Gaussian Splatting from Monocular Videos**

* 🧑‍🎓 **Author**：Shi Chen, Erik Sandstrom, Sandro Lombardi, Siyuan Li, Martin R. Oswald
* 🔗 **Link**：\[[arXiv:2509.17864](https://arxiv.org/abs/2509.17864)]
* 🤔 **Challenge**：Achieving truly practical dynamic 3D reconstruction requires online operation, global pose and map consistency, detailed appearance modeling, and the flexibility to handle both RGB and RGB-D inputs. However, existing SLAM methods typically merely remove the dynamic parts or require RGB-D input, while offline methods are not scalable to long video sequences, and current transformer-based feedforward methods lack global consistency and appearance details.
* 📖 **Introduction**：ProDyG introduces a progressive Gaussian Splatting framework for monocular video-based dynamic scene reconstruction, enabling online processing with global consistency. It progressively builds and refines the scene representation, supporting both RGB and RGB-D inputs, and achieves high-fidelity novel view synthesis while maintaining real-time performance in long sequences.



**\[19]. BARD-GS: Blur-Aware Reconstruction of Dynamic Scenes via Gaussian Splatting (CVPR 2025)**

* 🧑‍🎓 **Author**：Yiren Lu, Yunlai Zhou, Disheng Liu, Tuo Liang, Yu Yin
* 🔗 **Link**：\[[arXiv:2503.15835](https://arxiv.org/abs/2503.15835)]
* 🤔 **Challenge**：Motion blur in real-world dynamic scenes captured by handheld monocular cameras poses significant challenges for accurate 3D reconstruction, particularly in distinguishing camera motion blur from object motion blur.
* 📖 **Introduction**：BARD-GS proposes a blur-aware Gaussian Splatting method that explicitly models and deblurs dynamic scenes by integrating motion estimation and adaptive Gaussian deformation. It outperforms prior methods in handling blurred inputs, achieving superior reconstruction quality and rendering fidelity on dynamic benchmarks.



**\[18]. SurgicalGS: Dynamic 3D Gaussian Splatting for Accurate Robotic-Assisted Surgical Scene Reconstruction (MICCAI 2025)**

* 🧑‍🎓 **Author**：Jialei Chen, Xin Zhang, Mobarakol Islam, Francisco Vasconcelos, Danail Stoyanov, Daniel S. Elson, Baoru Huang
* 🔗 **Link**：\[[arXiv:2410.09292](https://arxiv.org/abs/2410.09292)]
* 🤔 **Challenge**：Accurate 3D reconstruction of dynamic surgical scenes from endoscopic video is essential for robotic-assisted surgery, but recent 3D Gaussian Splatting methods suffer from depth compression due to inverse depth loss functions, leading to inaccuracies in deformable tissues.
* 📖 **Introduction**：SurgicalGS enhances dynamic Gaussian Splatting with a novel depth-aware loss and deformation modeling tailored for surgical environments, enabling precise reconstruction of deformable scenes. It achieves higher geometric accuracy and faster rendering compared to baselines, supporting real-time robotic applications.



**\[17]. Motion-Blender Gaussian Splatting for Dynamic Scene Reconstruction**

* 🧑‍🎓 **Author**：Xinyu Zhang, Haonan Chang, Yuhan Liu, Abdeslam Boularias
* 🔗 **Link**：\[[arXiv:2503.09040](https://arxiv.org/abs/2503.09040)]
* 🤔 **Challenge**：Existing dynamic Gaussian Splatting methods struggle with explicit motion representation, leading to inefficiencies in modeling complex non-rigid deformations in robot vision applications.
* 📖 **Introduction**：This work introduces Motion-Blender Gaussian Splatting (MBGS), a framework that uses motion graphs as an explicit and sparse motion representation, propagating link motions to individual Gaussians via dual quaternion skinning with learnable weights. Jointly optimized from videos, it enables high-fidelity dynamic reconstruction with differentiable rendering.



**\[16]. DGNS: Deformable Gaussian Splatting and Dynamic Neural Surface for Monocular Dynamic 3D Reconstruction (ACM MM 2025)**

* 🧑‍🎓 **Author**：Xuesong Li, Jinguang Tong, Jie Hong, Vivien Rolland, Lars Petersson
* 🔗 **Link**：\[[arXiv:2412.03910](https://arxiv.org/abs/2412.03910)]
* 🤔 **Challenge**：Monocular dynamic 3D reconstruction faces challenges in novel-view synthesis and geometry fidelity due to the lack of explicit surface constraints in pure Gaussian representations.
* 📖 **Introduction**：DGNS combines Deformable Gaussian Splatting with Dynamic Neural Surfaces in a hybrid framework, incorporating depth and normal supervision for improved 3D consistency. It excels in dynamic scene reconstruction, outperforming baselines in PSNR and geometric metrics on standard datasets.



**\[15]. Periodic Vibration Gaussian: Dynamic Urban Scene Reconstruction and Real-time Rendering (CVPR 2024)**

* 🧑‍🎓 **Author**：Yurui Chen, Chun Gu, Junzhe Jiang, Xiatian Zhu, Li Zhang
* 🔗 **Link**：\[[arXiv:2311.18561](https://arxiv.org/abs/2311.18561)]
* 🤔 **Challenge**：The modeling challenge for dynamic, large-scale urban scenes lies in their highly complex geometric structures and spatially and temporally unconstrained dynamics. Prior approaches typically employ high-level architectural priors that separate static and dynamic elements, resulting in suboptimal capture of their synergistic interactions.
* 📖 **Introduction**：This paper introduces Periodic Vibration Gaussian (PVG), which builds upon 3DGS by incorporating time-based dynamics driven by periodic vibrations. This innovation enables PVG to elegantly and uniformly represent the characteristics of various objects and elements within dynamic urban scenes.



**\[14]. Speedy-Splat: Fast 3D Gaussian Splatting with Sparse Pixels and Sparse Primitives**

* 🧑‍🎓 **Author**：Alex Hanson, Allen Tu, Geng Lin, Vasu Singla, Matthias Zwicker, Tom Goldstein
* 🔗 **Link**：\[[arXiv:2412.00578](https://arxiv.org/abs/2412.00578)]
* 🤔 **Challenge**：Although recent work on compressing 3D-GS models has achieved some acceleration by reducing the number of parameters, few methods directly target rendering speed.
* 📖 **Introduction**：Speedy-Splat optimizes the rendering pipeline to precisely locate Gaussians within scenes, boosting rendering speed without compromising visual fidelity. Furthermore, it introduces a novel pruning technique integrated into the training pipeline, significantly reducing model size and training time while further accelerating rendering performance.



**\[13]. SplatFlow: Self-Supervised Dynamic Gaussian Splatting in Neural Motion Flow Field for Autonomous Driving (CVPR 2025)**

* 🧑‍🎓 **Author**：Su Sun, Cheng Zhao, Zhuoyang Sun, Yingjie Victor Chen, Mei Chen
* 🔗 **Link**：\[[arXiv:2411.15482](https://arxiv.org/abs/2411.15482)]
* 🤔 **Challenge**：Most existing dynamic Gaussian dispersion methods for complex urban scenes rely on costly, manually labeled, accurate object-level supervision, which limits their scalability in practical applications.
* 📖 **Introduction**：This paper introduces SplatFlow, a self-supervised dynamic Gaussian splatting technique within Neural Motion Flow Fields (NMFF) that learns 4D spatiotemporal representations without tracking 3D bounding boxes. This enables accurate dynamic scene reconstruction and novel view synthesis of RGB/depth/flow.



**\[12]. Das3r: Dynamics-aware gaussian splatting for static scene reconstruction**

* 🧑‍🎓 **Author**：Kai Xu, Tze Ho Elden Tse, Jizong Peng, Angela Yao
* 🔗 **Link**：\[[arXiv:2412.19584](https://arxiv.org/abs/2412.19584)]
* 🤔 **Challenge**：Previous 3DGS dynamic reconstruction methods have encountered difficulties when applied to broader everyday video content involving continuous and numerous dynamic components alongside complex camera movements.
* 📖 **Introduction**：This paper proposes DAS3R for scene segmentation and static background reconstruction from everyday videos. By integrating pre-trained motion masks, modeling static scenes as Gaussian fragments, and performing dynamics-aware optimization, it achieves more accurate background reconstruction results than previous work.



**\[11]. DeSiRe-GS: 4D Street Gaussians for Static-Dynamic Decomposition and Surface Reconstruction for Urban Driving Scenes (CVPR 2025)**

* 🧑‍🎓 **Author**：Chensheng Peng, Chengwei Zhang, Yixiao Wang, Chenfeng Xu, Yichen Xie, Wenzhao Zheng, Kurt Keutzer, Masayoshi Tomizuka, Wei Zhan
* 🔗 **Link**：\[[arXiv:2411.11921](https://arxiv.org/abs/2411.11921)]
* 🤔 **Challenge**：Due to the unbounded nature of outdoor environments, 3DGS faces challenges in reconstruction accuracy and efficiency during dynamic driving scene reconstruction.
* 📖 **Introduction**：This paper proposes DeSiRe-GS, a two-stage optimization pipeline based on dynamic street Gaussians. In the first stage, a two-dimensional motion mask is extracted, as the observed three-dimensional Gaussian distribution inherently can only reconstruct static regions in dynamic environments. These extracted 2D motion priors are then differentially mapped into Gaussian space using the efficient formula of the second-stage dynamic Gaussian. Combined with introduced geometric regularization, this approach resolves overfitting issues caused by data sparsity in autonomous driving while reconstructing physically plausible Gaussians.



**\[10]. Mini-Splatting: Representing Scenes with a Constrained Number of Gaussians**

* 🧑‍🎓 **Author**：Guangchi Fang, Bing Wang
* 🔗 **Link**：\[[arXiv:2403.14166v3](https://arxiv.org/abs/2403.14166v3)]
* 🤔 **Challenge**：Using a finite number of Gaussian representations to effectively model scenes
* 📖 **Introduction**：This paper introduces strategies for densification including blur split and depth reinitialization, and simplification through intersection preserving and sampling. These techniques reorganize the spatial positions of the Gaussians, resulting in significant improvements across various datasets and benchmarks in terms of rendering quality, resource consumption, and storage compression.



**\[9]. Street Gaussians: Modeling Dynamic Urban Scenes with Gaussian Splatting (ECCV 2024)**

* 🧑‍🎓 **Author**：Yunzhi Yan, Haotong Lin, Chenxu Zhou, Weijie Wang, Haiyang Sun, Kun Zhan, Xianpeng Lang, Xiaowei Zhou, Sida Peng
* 🔗 **Link**：\[[arXiv:2401.01339](https://arxiv.org/abs/2401.01339)]
* 🤔 Challenge：3DGS exhibits slow training and rendering speeds when modeling dynamic urban streets in autonomous driving scenarios.
* 📖 **Introduction**：The dynamic urban scenes of Street Gaussians are represented as a set of point clouds equipped with semantic logic and 3D Gaussians, each of which is associated with either a foreground vehicle or the background. To model the dynamics of foreground objects, each object point cloud is optimized using an optimizable tracking pose and a 4D spherical harmonic model for dynamic appearance. Street Gaussians enable scene editing operations and rendering at 135 FPS (1066 x 1600 resolution) within half an hour after training.



**\[8]. 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering (CVPR 2024)**

* 🧑‍🎓 **Author**：Guanjun Wu, Taoran Yi, Jiemin Fang, Lingxi Xie, Xiaopeng Zhang, Wei Wei, Wenyu Liu, Qi Tian, Xinggang Wang
* 🔗 **Link**：\[[arXiv:2310.08528](https://arxiv.org/abs/2310.08528)]
* 🤔 **Challenge**：3DGS accurately models complex motion, which is often difficult to achieve efficiently.
* 📖 **Introduction**：This paper proposes 4D Gaussian Splatting (4D-GS) as a holistic representation of dynamic scenes, rather than applying 3D-GS to each individual frame. In 4D-GS, a novel explicit representation is proposed that simultaneously incorporates 3D Gaussian and 4D neurovoxels.



**\[7]. AutoSplat: Constrained Gaussian Splatting for Autonomous Driving Scene Reconstruction**

* 🧑‍🎓 **Author**：Mustafa Khan, Hamidreza Fazlali, Dhruv Sharma, Tongtong Cao, Dongfeng Bai, Yuan Ren, Bingbing Liu
* 🔗 **Link**：\[[arXiv:2407.02598](https://arxiv.org/abs/2407.02598)]
* 🤔 **Challenge**：3DGS faces challenges in simulating driving scenarios due to complex backgrounds, dynamic objects, and sparse views.
* 📖 **Introduction**：This paper proposes AutoSplat to achieve highly realistic reconstruction of autonomous driving scenes. It decomposes the background and imposes geometric constraints on its road and sky regions to enable multi-view consistent rasterization. It uses 3D templates to initialize foreground Gaussians and combines reflection Gaussian consistency constraints to reconstruct invisible parts from symmetric visible views. It captures the dynamic visual features of foreground objects by estimating time-dependent residual spherical harmonics. AutoSplat outperforms state-of-the-art methods in scene reconstruction and novel view synthesis across various driving scenarios.



**\[6]. VDG: Vision-Only Dynamic Gaussian for Driving Simulation**

* 🧑‍🎓 **Author**：Hao Li, Jingfeng Li, Dingwen Zhang, Chenming Wu, Jieqi Shi, Chen Zhao, Haocheng Feng, Errui Ding, Jingdong Wang, Junwei Han
* 🔗 **Link**：\[[arXiv:2406.18198](https://arxiv.org/abs/2406.18198)]
* 🤔 **Challenge**：Previous works heavily relied on precomputed pose and motion structure (SfM) algorithms or expensive sensors with Gaussian initialization.
* 📖 **Introduction**：This paper promotes pose and depth initialization as well as static-dynamic decomposition by integrating self-supervised VO into our pose-free dynamic Gaussian method (VDG) for the first time. In addition, compared with pose-free dynamic view synthesis methods, VDG can process only RGB image inputs and construct dynamic scenes at a faster speed and with a larger scene.



**\[5]. S3Gaussian: Self-Supervised Street Gaussians for Autonomous Driving (CVPR 2024)**

* 🧑‍🎓 **Author**：Nan Huang, Xiaobao Wei, Wenzhao Zheng, Pengju An, Ming Lu, Wei Zhan, Masayoshi Tomizuka, Kurt Keutzer, Shanghang Zhang
* 🔗 **Link**：\[[arXiv:2405.20323](https://arxiv.org/abs/2405.20323)]
* 🤔 **Challenge**：Most previous street 3DGS methods require tracked 3D vehicle bounding boxes to decompose the static and dynamic elements for effective reconstruction, limiting their applications for in-the-wild scenarios.
* 📖 **Introduction**：This paper proposes a self-supervised street Gaussian (S3Gaussian) method that decomposes dynamic and static elements from 4D consistency. S3Gaussian demonstrates the ability to decompose static and dynamic scenes and achieves optimal performance without using 3D annotations.



**\[4]. DrivingGaussian: Composite Gaussian Splatting for Surrounding Dynamic Autonomous Driving Scenes (CVPR 2024)**

* 🧑‍🎓 **Author**：Xiaoyu Zhou, Zhiwei Lin, Xiaojun Shan, Yongtao Wang, Deqing Sun, Ming-Hsuan Yang
* 🔗 **Link**：\[[arXiv:2312.07920](https://arxiv.org/abs/2312.07920)]
* 🤔 **Challenge**：Previous works focused on individual dynamic objects and were unable to handle complex driving scenarios involving static-dynamic composite areas and multiple high-speed moving objects.
* 📖 **Introduction**：DrivingGaussian uses composite dynamic Gaussian maps to process multiple moving objects, independently reconstructing each object and restoring its accurate position and occlusion relationships in the scene. DrivingGaussian outperforms existing methods in dynamic driving scene reconstruction and can achieve realistic surround synthesis with high fidelity and multi-camera consistency.



**\[3]. HUGS: Holistic Urban 3D Scene Understanding via Gaussian Splatting**

* 🧑‍🎓 **Author**：Hongyu Zhou, Jiahao Shao, Lu Xu, Dongfeng Bai, Weichao Qiu, Bingbing Liu, Yue Wang, Andreas Geiger, Yiyi Liao
* 🔗 **Link**：\[[arXiv:2403.12722](https://arxiv.org/abs/2403.12722)]
* 🤔 **Challenge**：Previous works have typically focused on specific aspects of understanding urban scenes based on RGB images, requiring additional inputs such as LiDAR scans or manually annotated 3D bounding boxes.
* 📖 **Introduction**：This paper introduces a new pipeline for understanding urban scenes using 3D Gaussian splatting, which can render new viewpoints in real time, generate high-precision 2D and 3D semantic information, and reconstruct dynamic scenes, even in scenes with high noise in 3D bounding box detection.



**\[2]. Motion-aware 3D Gaussian Splatting  for Efficient Dynamic Scene Reconstruction**

* 🧑‍🎓 **Author**：Zhiyang Guo, Wengang Zhou, Li Li, Min Wang, Houqiang Li
* 🔗 **Link**：\[[arXiv:2403.11447](https://arxiv.org/abs/2403.11447)]
* 🤔 **Challenge**：Previous works have primarily focused on extending static 3DGS to time-varying representations, neglecting the rich motion information carried by two-dimensional observations. This approach suffers from performance degradation and model redundancy issues.
* 📖 **Introduction**：A novel motion-aware enhancement framework for dynamic scene reconstruction is proposed, which extracts useful motion cues from optical flow to improve different paradigms of dynamic 3DGS. Compared with the baselines, our method shows significant superiority in both rendering quality and efficiency.



**\[1]. Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis**

* 🧑‍🎓 **Author**：Jonathon Luiten, Georgios Kopanas, Bastian Leibe, Deva Ramanan
* 🔗 **Link**：\[[arXiv:2308.09713](https://arxiv.org/abs/2308.09713)]
* 🤔 **Challenge**：Extend 3DGS from modeling static scenes only to dynamic scenes.
* 📖 **Introduction**：Dynamic 3D Gaussians solve the task of dynamic scene view synthesis and six degrees of freedom (6-DOF) tracking of all dense scene elements, while supporting a wide range of downstream applications, including first-person view synthesis, dynamic scene synthesis, and 4D video editing.

