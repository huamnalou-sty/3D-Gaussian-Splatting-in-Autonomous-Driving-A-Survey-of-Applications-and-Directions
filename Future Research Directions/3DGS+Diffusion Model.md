**\[20]. L3DG: Latent 3D Gaussian Diffusion (SIGGRAPH Asia 2024)**

* 🧑‍🎓 **Author**：Barbara Roessle, Norman Müller, Lorenzo Porzi, Samuel Rota Bulò, Peter Kontschieder, Angela Dai, Matthias Nießner
* 🔗 **Link**：\[[arXiv:2410.13530](https://arxiv.org/abs/2410.13530)]
* 🤔 **Challenge**：Directly generating large-scale 3D scenes in pixel space or raw parameter space is computationally expensive, limiting generation resolution and scene scale.
* 📖 **Introduction**：L3DG proposes a latent 3D Gaussian diffusion model. It compresses 3D Gaussians into a compact latent space via a VQ-VAE and trains a diffusion model within that space. This approach significantly reduces generation complexity, making the generation of large-scale (Room-scale) 3D scenes possible.



**\[19]. LangSplat: 3D Language Gaussian Splatting (CVPR 2024)**

* 🧑‍🎓 **Author**：Minghan Qin, Wanhua Li, Jiawei Zhou, Haoqian Wang, Hanspeter Pfister
* 🔗 **Link**：\[[arXiv:2312.16084](https://arxiv.org/abs/2312.16084)]
* 🤔 **Challenge**：Precise open-vocabulary queries in 3D space are usually inefficient and consume large amounts of memory; existing NeRF-based methods (like LERF) have slow rendering speeds and ambiguous queries.
* 📖 **Introduction**：LangSplat integrates language features (CLIP embeddings) into 3D Gaussians. It uses a scene-specific autoencoder to compress language features, avoiding high memory costs, and achieves rendering speeds 199 times faster than LERF, supporting precise semantic queries and localization in 3D scenes.



**\[18]. GaussianCube: Structured Gaussian Splatting using Optimal Transport for 3D Generative Modeling (NeurIPS 2024)**

* 🧑‍🎓 **Author**：Bowen Zhang, Yiji Cheng, Jiaolong Yang, Chunyu Wang, Feng Zhao, Yansong Tang, Dong Chen, Baining Guo
* 🔗 **Link**：\[[arXiv:2403.19655](https://arxiv.org/abs/2403.19655v2)]
* 🤔 **Challenge**：3D Gaussians are unstructured data, making it difficult to directly apply standard 3D convolutional networks (like 3D U-Net) for diffusion generation.
* 📖 **Introduction**：GaussianCube rearranges and voxelizes discrete 3D Gaussians into a structured grid representation (GaussianCube) using an Optimal Transport algorithm. This enables the use of efficient 3D U-Nets for diffusion modeling, achieving high-quality 3D generation with significantly fewer parameters.



**\[17]. GALA3D: Towards Text-to-3D Complex Scene Generation via Layout-guided Generative Gaussian Splatting (ICML 2024)**

* 🧑‍🎓 **Author**：Xiaoyu Zhou, Xingjian Ran, Yajiao Xiong, Jinlin He, Zhiwei Lin, Yongtao Wang, Deqing Sun, Ming-Hsuan Yang
* 🔗 **Link**：\[[arXiv:2402.07207](https://arxiv.org/abs/2402.07207)]
* 🤔 **Challenge**：Generating complex 3D scenes (containing multiple objects and specific layouts) from text is very difficult; existing text-to-3D methods usually only handle single objects and struggle to control the overall structure and object interactions.
* 📖 **Introduction**：GALA3D first utilizes a Large Language Model (LLM) to generate a scene layout, then introduces a layout-guided Gaussian representation. Through a compositional optimization mechanism and conditional diffusion models, it generates complex 3D scenes with consistent geometry, texture, and scale while maintaining high fidelity for individual objects.



**\[16]. DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation (ICLR 2024)**

* 🧑‍🎓 **Author**：Jiaxiang Tang, Jiawei Ren, Hang Zhou, Ziwei Liu, Gang Zeng
* 🔗 **Link**：\[[arXiv:2309.16653](https://arxiv.org/abs/2309.16653)]
* 🤔 **Challenge**：NeRF-based generation methods (like DreamFusion) have long optimization times and difficulty extracting high-quality meshes; existing methods struggle to balance generation efficiency and quality.
* 📖 **Introduction**：DreamGaussian designs a generative 3D Gaussian Splatting framework paired with mesh extraction and UV space texture refinement. Leveraging the progressive densification property of Gaussians to accelerate convergence, it generates high-quality textured 3D meshes from a single image in just about 2 minutes.



**\[15]. VFusion3D: Learning Scalable 3D Generative Models from Video Diffusion Models (ECCV 2024)**

* 🧑‍🎓 **Author**：Junlin Han, Filippos Kokkinos, Philip Torr
* 🔗 **Link**：\[[arXiv:2403.12034](https://arxiv.org/abs/2403.12034)]
* 🤔 **Challenge**：Developing scalable 3D generative models is limited by the scarcity of high-quality 3D data, while existing 2D data lacks 3D information.
* 📖 **Introduction**：VFusion3D proposes using video diffusion models as "multi-view data generators" to create large-scale synthetic multi-view data. A feed-forward 3D generative model trained on this data demonstrates excellent scalability and generation quality, marking a significant step towards 3D foundation models.



**\[14]. Generative Sparse-view Gaussian Splatting (CVPR 2025)**

* 🧑‍🎓 **Author**：Hanyang Kong, Xingyi Yang, Xinchao Wang
* 🔗 **Link**：\[[https://openaccess.thecvf.com/content/CVPR2025/papers/Kong\_Generative\_Sparse-View\_Gaussian\_Splatting\_CVPR\_2025\_paper.pdf](https://openaccess.thecvf.com/content/CVPR2025/papers/Kong_Generative_Sparse-View_Gaussian_Splatting_CVPR_2025_paper.pdf)]
* 🤔 **Challenge**：Reconstructing 3D scenes from extremely sparse views is an ill-posed problem due to the lack of observational information, leading to inaccurate geometric inference and artifacts.
* 📖 **Introduction**：GS-GS introduces a generative pipeline that uses pre-trained image diffusion models to "hallucinate" images for unseen views (Pseudo-views). Through an iterative optimization strategy, it enforces consistency between generated views and semantic correspondence, significantly enhancing the reconstruction quality of 3D/4D Gaussian Splatting under sparse views.



**\[13]. DirectTriGS: Triplane-based Gaussian Splatting Field Representation for 3D Generation (CVPR 2025)**

* 🧑‍🎓 **Author**：Xiaoliang Ju, Hongsheng Li
* 🔗 **Link**：\[[arXiv:2503.06900](https://arxiv.org/abs/2503.06900)]
* 🤔 **Challenge**：Directly generating discrete point cloud data for 3D Gaussians is very difficult because they are unstructured, whereas traditional generative models excel at processing continuous data.
* 📖 **Introduction**：DirectTriGS proposes using a Triplane representation to encode 3D Gaussians into an image-like continuous field. By using a TriRenderer for differentiable rendering supervision, combined with a Variational Autoencoder (VAE) and a Latent Diffusion Model, it achieves direct, high-quality generation of 3D Gaussian objects.



**\[12]. GaussianDreamer: Fast Generation from Text to 3D Gaussians by Bridging 2D and 3D Diffusion Models (CVPR 2024)**

* 🧑‍🎓 **Author**：Taoran Yi, Jiemin Fang, Junjie Wang, Guanjun Wu, Lingxi Xie, Xiaopeng Zhang, Wenyu Liu, Qi Tian, Xinggang Wang
* 🔗 **Link**：\[[arXiv:2310.08529](https://arxiv.org/abs/2310.08529)]
* 🤔 **Challenge**：3D diffusion models possess geometric consistency but lack texture details, whereas 2D diffusion models are rich in detail but lack 3D consistency. Combining the advantages of both for fast generation is a difficult problem.
* 📖 **Introduction**：GaussianDreamer bridges 2D and 3D diffusion models. It first utilizes the geometric priors from a 3D diffusion model to initialize 3D Gaussian point clouds, and then employs Score Distillation Sampling (SDS) to leverage a 2D diffusion model for enriching geometric and texture details. This method achieves high-quality text-to-3D generation in 15 minutes.



**\[11]. LGM: Large Multi-View Gaussian Model for High-Resolution 3D Content Creation (ECCV 2024)**

* 🧑‍🎓 **Author**：Jiaxiang Tang, Zhaoxi Chen, Xiaokang Chen, Tengfei Wang, Gang Zeng, Ziwei Liu
* 🔗 **Link**：\[[arXiv:2402.05054](https://arxiv.org/abs/2402.05054)]
* 🤔 **Challenge**：Existing 3D generation methods struggle to balance generation speed and high-resolution details; optimization-based methods are too slow, while feed-forward methods often result in low resolution.
* 📖 **Introduction**：LGM is a novel framework that generates high-resolution 3D Gaussian Primitives directly from multi-view images or text via an asymmetric U-Net backbone. By training on data generated by multi-view diffusion models, it can produce high-quality 512-resolution 3D objects in approximately 5 seconds, significantly improving efficiency and quality.



**\[10]. 3DGS-Enhancer: Enhancing Unbounded 3D Gaussian Splatting with View-consistent 2D Diffusion Priors (NeurIPS 2024)**

* 🧑‍🎓 **Author**：Xi Liu, Chaoyi Zhou, Siyu Huang
* 🔗 **Link**：\[[arXiv:2410.16266](https://arxiv.org/abs/2410.16266)]
* 🤔 **Challenge**：In unbounded scenes with sparse input views, standard 3DGS often fails to render consistent novel views due to the lack of spatial information.
* 📖 **Introduction**：3DGS-Enhancer reformulates the 3D view consistency problem as a video temporal consistency task. It uses a video diffusion model to enhance the latent features of rendered views, ensuring they are consistent, and then uses these enhanced views to fine-tune the 3DGS model.



**\[9]. DiffGS: Functional Gaussian Splatting Diffusion**

* 🧑‍🎓 **Author**：Junsheng Zhou, Weiqi Zhang, Yu-Shen Liu
* 🔗 **Link**：\[[arXiv:2410.19657](https://arxiv.org/abs/2410.19657)]
* 🤔 **Challenge**：Directly generating 3D Gaussian Splatting representations is difficult because they are discrete and unstructured data, unlike continuous meshes or voxel grids.
* 📖 **Introduction**：DiffGS disentangles the discrete 3DGS representation into continuous functions (Gaussian Probability, Color, and Transform functions). It then trains a Latent Diffusion Model (LDM) on these functions to efficiently generate high-fidelity 3D Gaussian primitives.



**\[8]. SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior (WACV 2025)**

* 🧑‍🎓 **Author**：Zhongrui Yu, Haoran Wang, Jinze Yang, Hanzhang Wang, Zeke Xie, Yunfeng Cai, Jiale Cao, Zhong Ji, Mingming Sun
* 🔗 **Link**：\[[arXiv:2403.20079](https://arxiv.org/abs/2403.20079)]
* 🤔 **Challenge**：Synthesizing novel street views is difficult because vehicle-captured training data is sparse and constrained to a specific path, causing blurring and artifacts when viewing from new angles.
* 📖 **Introduction**：SGD integrates a diffusion model with 3D Gaussian Splatting. It utilizes adjacent frames and LiDAR depth to fine-tune a diffusion model, which then acts as a prior to guide the 3DGS training, providing supervision for unseen views and improving rendering quality.



**\[7]. Deceptive-NeRF/3DGS: Diffusion-Generated Pseudo-Observations for High-Quality Sparse-View Reconstruction (ECCV 2024)**

* 🧑‍🎓 **Author**：Xinhang Liu, Jiaben Chen, Shiu-Hong Kao, Yu-Wing Tai,  and Chi-Keung Tang
* 🔗 **Link**：\[[arXiv:2305.15171](https://arxiv.org/abs/2305.15171)]
* 🤔 **Challenge**：Sparse-view reconstruction often fails due to a lack of observations, leading to overfitting and artifacts in novel views.
* 📖 **Introduction**：This method proposes a "deceptive" diffusion model that takes noisy renderings from a sparse reconstruction and enhances them into high-quality "pseudo-observations." These generated views are then used to supervise the NeRF or 3DGS model, effectively densifying the training data.



**\[6]. HuGDiffusion: Generalizable Single-Image Human Rendering via 3D Gaussian Diffusion**

* 🧑‍🎓 **Author**：Yingzhi Tang, Qijian Zhang, Junhui Hou
* 🔗 **Link**：\[[arXiv:2501.15008](https://arxiv.org/abs/2501.15008)]
* 🤔 **Challenge**：Rendering detailed 3D humans from a single image is challenging due to self-occlusions and the difficulty of inferring invisible parts or 3D structure from 2D pixel data alone.
* 📖 **Introduction**：HuGDiffusion treats single-view human rendering as a conditional generation task. It uses a diffusion-based framework conditioned on human-centric priors to generate 3D Gaussian attributes (position, color, etc.), significantly outperforming regression-based baselines.



**\[5]. DiffSplat: Repurposing Image Diffusion Models for Scalable Gaussian Splat Generation**

* 🧑‍🎓 **Author**：Chenguo Lin, Panwang Pan, Bangbang Yang, Zeming Li, Yadong Mu
* 🔗 **Link**：\[[arXiv:2501.16764](https://arxiv.org/abs/2501.16764)]
* 🤔 **Challenge**：Existing 3D generative models struggle to effectively utilize web-scale 2D priors from image diffusion models while simultaneously maintaining 3D consistency and scalability.
* 📖 **Introduction**：DiffSplat is a 3D generative framework that directly generates 3D Gaussian splats by fine-tuning large-scale text-to-image diffusion models. It uses a lightweight reconstruction model for bootstrapping and introduces a 3D rendering loss to ensure coherence across arbitrary views.



**\[4]. RGE-GS: Reward-Guided Expansive Driving Scene Reconstruction via Diffusion Priors**

* 🧑‍🎓 **Author**：Sicong Du, Jiarun Liu, Qifeng Chen, Hao-Xiang Chen, Tai-Jiang Mu, Sheng Yang
* 🔗 **Link**：\[[arXiv:2506.22800](https://arxiv.org/abs/2506.22800)]
* 🤔 **Challenge**：Reconstructing expansive driving scenes using diffusion priors often leads to inconsistencies where the generated areas do not align well with the reconstructed geometry, causing artifacts in the expanded regions.
* 📖 **Introduction**：RGE-GS employs a reward-guided framework that evaluates the confidence of diffusion-generated priors before integrating them. It prioritizes consistently generated patterns to ensure spatial stability and high quality during the expansive reconstruction of driving scenes.



**\[3]. X-Scene: Large-Scale Driving Scene Generation with High Fidelity and Flexible Controllability**

* 🧑‍🎓 **Author**：Yu Yang, Alan Liang, Jianbiao Mei, Yukai Ma, Yong Liu, Gim Hee Lee
* 🔗 **Link**：\[[arXiv:2506.13558](https://arxiv.org/abs/2506.13558)]
* 🤔 **Challenge**：Generating large-scale driving scenes requires balancing high geometric/visual fidelity with flexible controllability (e.g., specific layouts vs. user intentions), which is difficult to achieve in a unified framework.
* 📖 **Introduction**：X-Scene is a framework for large-scale driving scene generation that supports multi-granular control. It sequentially generates 3D semantic occupancy and multi-view videos, ensuring alignment across modalities and allowing control via both low-level layouts and LLM-enriched text prompts.



**\[2]. VideoScene: Distilling Video Diffusion Model to Generate 3D Scenes in One Step (CVPR 2025)**

* 🧑‍🎓 **Author**： Hanyang Wang,Fangfu Liu,Jiawei Chi, Yueqi Duan
* 🔗 **Link**：\[[https://openaccess.thecvf.com/content/CVPR2025/papers/Wang\_VideoScene\_Distilling\_Video\_Diffusion\_Model\_to\_Generate\_3D\_Scenes\_in\_CVPR\_2025\_paper.pdf](https://openaccess.thecvf.com/content/CVPR2025/papers/Wang_VideoScene_Distilling_Video_Diffusion_Model_to_Generate_3D_Scenes_in_CVPR_2025_paper.pdf)]
* 🤔 **Challenge**：Traditional methods for generating 3D scenes from video diffusion priors require multi-step inference, which is slow and prone to accumulating inconsistencies, leading to artifacts and structural misalignment.
* 📖 **Introduction**：VideoScene distills a video diffusion model into a consistent 3D scene generator. It utilizes a "3D-Aware Leap Flow Distillation" strategy to generate 3D-consistent scenes from sparse views in a single step, significantly improving efficiency and fidelity.



**\[1]. 4Real: Towards Photorealistic 4D Scene Generation via Video Diffusion Models (NeurIPS 2024)**

* 🧑‍🎓 **Author**：Heng Yu, Chaoyang Wang, Peiye Zhuang, Willi Menapace, Aliaksandr Siarohin, Junli Cao, Laszlo A Jeni, Sergey Tulyakov, Hsin-Ying Lee
* 🔗 **Link**：\[[arXiv:2406.07472](https://arxiv.org/abs/2406.07472)]
* 🤔 **Challenge**：Generating dynamic 4D scenes from text or video is difficult due to the lack of diverse 4D data, and existing methods often struggle to maintain both photorealism and temporal consistency when handling complex real-world motions.
* 📖 **Introduction**：4Real introduces a pipeline that leverages the priors of video diffusion models to supervise Deformable 3D Gaussian Splatting (D-3DGS). By creating "freeze-time" videos and employing Score Distillation Sampling (SDS), it generates high-fidelity, spatiotemporally consistent 4D scenes from text prompts.
