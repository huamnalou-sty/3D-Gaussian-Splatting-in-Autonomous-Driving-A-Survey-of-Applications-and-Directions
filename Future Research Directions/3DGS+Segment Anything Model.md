**\[8]. Segment then Splat: Unified 3D Open-Vocabulary Segmentation via Gaussian Splatting**

* 🧑‍🎓 **Author**：Yiren Lu, Yunlai Zhou, Yiran Qiao, Chaoda Song, Tuo Liang, Jing Ma, Huan Wang, Yu Yin
* 🔗 **Link**：\[[arXiv:2503.22204](https://arxiv.org/abs/2503.22204)]
* 🤔 **Challenge**：Most existing methods follow a "reconstruction then segmentation" paradigm (relying on 2D pixel-level parsing), which leads to multi-view inconsistencies, poor 3D object retrieval, and significant struggles with dynamic scenes due to motion modeling complexities.
* 📖 **Introduction**：This paper proposes Segment then Splat, which reverses the traditional pipeline. It divides Gaussians into distinct object sets before reconstruction commences. By doing so, the scene is naturally segmented into individual objects upon reconstruction completion. This design eliminates both geometric and semantic ambiguities (common in dynamic scenes) and accelerates optimization by removing the need to learn a separate language field.



**\[7]. OpenInsGaussian: Open-vocabulary Instance Gaussian Segmentation with Context-aware Cross-view Fusion (ICCVW 2025)**

* 🧑‍🎓 **Author**：Tianyu Huang, Runnan Chen, Dongting Hu, Fengming Huang, Mingming Gong, Tongliang Liu
* 🔗 **Link**：\[[arXiv:2510.18253](https://arxiv.org/abs/2510.18253)]
* 🤔 **Challenge**：Recent semantic 3DGS approaches often rely on projecting 2D semantic features (from foundation models) onto 3D scenes, which frequently leads to alignment errors, incompleteness, and loss of context when fusing features from multiple views.
* 📖 **Introduction**：To address this, the authors propose OpenInsGaussian, a framework featuring two key modules: "Context-Aware Feature Extraction" which augments SAM masks with rich semantic context, and "Attention-Driven Feature Aggregation" which selectively fuses multi-view features to mitigate alignment errors. This method achieves state-of-the-art results in open-vocabulary 3D Gaussian segmentation by ensuring robust cross-view fusion.



**\[6]. OpenSplat3D: Open-Vocabulary 3D Instance Segmentation using Gaussian Splatting (CVPRW 2025)**

* 🧑‍🎓 **Author**：Jens Piekenbrinck, Christian Schmidt, Alexander Hermans, Narunas Vaskevicius, Timm Linder, Bastian Leibe
* 🔗 **Link**：\[[arXiv:2506.07697](https://arxiv.org/abs/2506.07697)]
* 🤔 **Challenge**：Standard 3DGS offers high-quality rendering but lacks fine-grained scene understanding; relying on manual labeling for instance segmentation is impractical, and existing methods often struggle to associate semantic information effectively with individual Gaussians.
* 📖 **Introduction**：This paper introduces OpenSplat3D, an approach for open-vocabulary 3D instance segmentation without manual labeling. It leverages "feature-splatting" to associate semantic info with Gaussians and incorporates SAM instance masks with a contrastive loss formulation to guide instance features. By utilizing language embeddings from vision-language models, it enables the system to identify and segment arbitrary objects in 3D scenes based on natural language descriptions.



**\[5]. PanoGS: Gaussian-based Panoptic Segmentation for 3D Open Vocabulary Scene Understanding (CVPR 2025)**

* 🧑‍🎓 **Author**：Hongjia Zhai, Hai Li, Zhenzhe Li, Xiaokun Pan, Yijia He, Guofeng Zhang
* 🔗 **Link**：\[[arXiv:2503.18107](https://arxiv.org/abs/2503.18107)]
* 🤔 **Challenge**：Previous open-vocabulary 3D Gaussian Splatting methods often fail to distinguish individual 3D instances, relying instead on coarse heatmaps between scene features and text queries; this limits their ability to perform true panoptic segmentation (simultaneous semantic and instance segmentation) which is essential for scene understanding.
* 📖 **Introduction**：PanoGS addresses this by combining a pyramid tri-plane representation for learning robust 3D language features with a graph clustering-based segmentation algorithm. It groups 3D Gaussians into geometrically and semantically consistent "super-primitives" (using SAM-guided edge affinity), enabling accurate, open-vocabulary 3D panoptic segmentation that effectively separates individual instances while maintaining semantic coherence.



**\[4]. LangSplat: 3D Language Gaussian Splatting (CVPR 2024)**

* 🧑‍🎓 **Author**：Minghan Qin, Wanhua Li, Jiawei Zhou, Haoqian Wang, Hanspeter Pfister
* 🔗 **Link**：\[[arXiv:2312.16084](https://arxiv.org/abs/2312.16084)]
* 🤔 **Challenge**：Explicitly modeling high-dimensional language features (like CLIP) in 3D scenes leads to massive memory consumption, and NeRF-based language field methods are extremely slow to render, making them unsuitable for real-time open-vocabulary queries.
* 📖 **Introduction**：LangSplat introduces a method for constructing language fields based on 3DGS. It utilizes a Scene-wise Autoencoder to compress high-dimensional CLIP language features into a low-dimensional latent space, decoding them only after rendering to drastically reduce memory usage. Additionally, it uses SAM's hierarchical semantic information to resolve semantic ambiguity in 3D point clouds. This approach achieves rendering speeds 199 times faster than LERF, supporting precise 3D open-vocabulary search and localization.



**\[3]. Feature 3DGS: Supercharging 3D Gaussian Splatting to Enable Distilled Feature Fields (CVPR 2024)**

* 🧑‍🎓 **Author**：Shijie Zhou, Haoran Chang, Sicheng Jiang, Zhiwen Fan, Zehao Zhu, Dejia Xu, Pradyumna Chari, Suya You, Zhangyang Wang, Achuta Kadambi
* 🔗 **Link**：\[[arXiv:2312.03203](https://arxiv.org/abs/2312.03203)]
* 🤔 **Challenge**：Integrating high-dimensional semantic features (from SAM, CLIP, etc.) directly into 3DGS is difficult due to the significant differences in spatial resolution and channel count between RGB images and feature maps; direct rendering of high-dimensional features also causes significant speed degradation.
* 📖 **Introduction**：Feature 3DGS proposes a general framework for feature field distillation. The core innovation is a parallel N-dimensional Gaussian Rasterizer paired with a lightweight convolutional acceleration module. This allows the model to efficiently distill semantic features of arbitrary dimensions from 2D foundation models (like SAM) into 3D Gaussians. It enables 3D semantic segmentation and editing based on text, points, or bounding box prompts while maintaining real-time rendering performance.



**\[2]. Segment Any 3D Gaussians (AAAI 2025)**

* 🧑‍🎓 **Author**：Jiazhong Cen, Jiemin Fang, Chen Yang, Lingxi Xie, Xiaopeng Zhang, Wei Shen, Qi Tian
* 🔗 **Link**：\[[arXiv:2312.00860](https://arxiv.org/abs/2312.00860)]
* 🤔 **Challenge**：Applying 2D foundation models (like SAM) to 3D scenes is difficult due to the lack of 3D consistency and the high computational cost required for real-time interaction; existing methods struggle to handle multi-granularity ambiguity where an object can be segmented at different levels of detail.
* 📖 **Introduction**：This paper introduces SAGA (Segment Any 3D GAussians), an interactive 3D segmentation approach. It efficiently distills multi-granularity 2D segmentation features from SAM into 3D Gaussian point features using a "scale-gated affinity feature" and contrastive training. This allows users to perform millisecond-level, real-time segmentation of 3D objects using various prompts (points, scribbles, or masks) with high boundary quality.



**\[1]. Gaussian Grouping: Segment and Edit Anything in 3D Scenes (ECCV 2024)**

* 🧑‍🎓 **Author**：Mingqiao Ye, Martin Danelljan, Fisher Yu, Lei Ke
* 🔗 **Link**：\[[arXiv:2312.00732](https://arxiv.org/abs/2312.00732)]
* 🤔 **Challenge**：While 3DGS excels in rendering speed and quality, it lacks fine-grained, object-level scene understanding (typically focusing only on appearance and geometry); traditional NeRF-based segmentation methods are slow and struggle with complex open-world editing tasks.
* 📖 **Introduction**：This paper proposes Gaussian Grouping, which adds a compact "Identity Encoding" to each 3D Gaussian to group those belonging to the same object. It leverages multi-view 2D masks generated by SAM as supervision, enabling zero-shot segmentation in 3D space via contrastive learning. This method not only reconstructs and segments 3D scenes with high quality but also supports direct editing operations on grouped Gaussians, such as object removal, inpainting, and style transfer.
