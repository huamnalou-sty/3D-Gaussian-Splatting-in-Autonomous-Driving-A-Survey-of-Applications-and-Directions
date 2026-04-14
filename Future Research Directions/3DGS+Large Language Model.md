**\[11]. MiDSummer: Multi-Guidance Diffusion for Controllable Zero-Shot Immersive Gaussian Splatting Scene Generation (ICCV 2025)**

* 🧑‍🎓 **Author**：Hu, Anjun and Tomsett, Richard and Gourmet, Valentin and Camplani, Massimo and Kandola, Jas and Xie, Hanting
* 🔗 **Link**：\[[https://openaccess.thecvf.com/content/ICCV2025/html/Hu\_MiDSummer\_Multi-Guidance\_Diffusion\_for\_Controllable\_Zero-Shot\_Immersive\_Gaussian\_Splatting\_Scene\_ICCV\_2025\_paper.html](https://openaccess.thecvf.com/content/ICCV2025/html/Hu_MiDSummer_Multi-Guidance_Diffusion_for_Controllable_Zero-Shot_Immersive_Gaussian_Splatting_Scene_ICCV_2025_paper.html)]
* 🤔 **Challenge**：Current 3D scene generation methods struggle to achieve precise control over scene layout while maintaining open-world generalization and physical plausibility; relying solely on diffusion models often fails to balance high-level semantic reasoning with low-level geometric control.
* 📖 **Introduction**：MiDSummer proposes a "Multi-Guidance Diffusion" framework specifically for controllable, zero-shot immersive 3DGS scene generation. It uniquely combines the open-vocabulary reasoning capabilities of LLMs with the geometric precision of Graph Diffusion Models (GDM). Specifically, the LLM plans the scene layout and generates "self-consistency scores," which guide the GDM to produce physically plausible layouts. These are finally assembled to generate high-quality 3D Gaussian scenes, achieving a precise transformation from text to complex immersive environments.



**\[10]. LangSplatV2: High-dimensional 3D Language Gaussian Splatting with 450+ FPS**

* 🧑‍🎓 **Author**：Wanhua Li, Yujie Zhao, Minghan Qin, Yang Liu, Yuanhao Cai, Chuang Gan, Hanspeter Pfister
* 🔗 **Link**：\[[arXiv:2507.07136](https://arxiv.org/abs/2507.07136)]
* 🤔 **Challenge**：Embedding high-dimensional language features (like CLIP/LLM features) into 3DGS typically significantly reduces rendering speed and struggles to handle the high resolution and speed bottlenecks required for Open-vocabulary Querying, limiting real-time interactive applications.
* 📖 **Introduction**：LangSplatV2 is an upgrade to the classic LangSplat. It introduces a novel feature decoupling technique that separates rendering speed from feature dimensions. This allows it to embed high-dimensional language semantics while achieving an astonishing 450+ FPS rendering speed. The model utilizes LLM/CLIP features to construct a precise 3D Language Field, supporting highly efficient open-vocabulary 3D querying and semantic understanding, providing a solid infrastructure for real-time 3D interaction and LLM-driven scene QA.



**\[9]. GaussianEditor: Editing 3D Gaussians Delicately with Text Instructions (CVPR 2024)**

* 🧑‍🎓 **Author**：Junjie Wang, Jiemin Fang, Xiaopeng Zhang, Lingxi Xie, Qi Tian
* 🔗 **Link**：\[[arXiv:2311.16037](https://arxiv.org/abs/2311.16037)]
* 🤔 **Challenge**：Performing fine-grained local editing on 3D scenes using only short text instructions is very difficult because computers struggle to accurately map text to specific Regions of Interest (RoI) in 3D, often leading to incorrect edit ranges or background damage.
* 📖 **Introduction**：GaussianEditor proposes a systematic editing framework that explicitly introduces an LLM Assistant to enhance controllability. First, the LLM analyzes user text instructions to extract a precise target region (Text RoI); then, the system uses visual grounding techniques to align the Text RoI into 3D Gaussian space (Gaussian RoI); finally, combining diffusion model priors, it refines only the Gaussians in the target area. This method effectively translates the LLM's semantic understanding into precise control over 3D geometry.



**\[9]. LLM-Grounder: Open-Vocabulary 3D Visual Grounding with Large Language Model as an Agent**

* 🧑‍🎓 **Author**：Jianing Yang, Xuweiyi Chen, Shengyi Qian, Nikhil Madaan, Madhavan Iyengar, David F. Fouhey, Joyce Chai
* 🔗 **Link**：\[[arXiv:2309.12311](https://arxiv.org/abs/2309.12311)]
* 🤔 **Challenge**：Traditional 3D Visual Grounding often relies on predefined categories or closed datasets, making it difficult to handle complex natural language descriptions and open-world object localization.
* 📖 **Introduction**：LLM-Grounder utilizes an LLM as the reasoning core, decomposing complex natural language queries into a series of executable steps (such as object attributes and spatial relationships). It combines the explicit scene representation provided by 3D Gaussian Splatting, allowing the LLM to directly "reason" and "locate" within 3D space. This method can handle open-vocabulary queries without retraining, significantly improving a robot's ability to understand user instructions and locate target objects in unknown environments.



**\[8]. GALA3D: Towards Text-to-3D Complex Scene Generation via Layout-guided Generative Gaussian Splatting (ICML 2024)**

* 🧑‍🎓 **Author**：Xiaoyu Zhou, Xingjian Ran, Yajiao Xiong, Jinlin He, Zhiwei Lin, Yongtao Wang, Deqing Sun, Ming-Hsuan Yang
* 🔗 **Link**：\[[arXiv:2402.07207](https://arxiv.org/abs/2402.07207)]
* 🤔 **Challenge**：Generating complex 3D scenes from text requires precise control over multiple objects and their spatial arrangement; existing holistic generation methods often lack user controllability and struggle with object-scene consistency.
* 📖 **Introduction**：GALA3D employs Large Language Models (LLMs) to generate an initial scene layout from text prompts. This layout acts as a strong prior to guide the optimization of a Gaussian Splatting representation, ensuring that individual objects are generated with high fidelity while maintaining a coherent and user-controllable global scene structure.



**\[7]. Hyper-3DG: Text-to-3D Gaussian Generation via Hypergraph**

* 🧑‍🎓 **Author**：Donglin Di, Jiahui Yang, Chaofan Luo, Zhou Xue, Wei Chen, Xun Yang, Yue Gao
* 🔗 **Link**：\[[arXiv:2403.09236](https://arxiv.org/abs/2403.09236)]
* 🤔 **Challenge**：Generating high-quality 3D objects from text is difficult due to the sophisticated high-order correlations between geometry and texture; standard optimization often leads to degradation or inconsistencies.
* 📖 **Introduction**：Hyper-3DG utilizes a "Geometry and Texture Hypergraph Refiner" (HGRefiner) to capture high-order correlations within 3D objects. By conducting hypergraph learning on patch-level 3D Gaussians, it refines both explicit attributes and latent visual features, significantly enhancing the quality and detail of text-generated 3D content.



**\[6]. PhiP-G: Physics-Guided Text-to-3D Compositional Scene Generation**

* 🧑‍🎓 **Author**：Qixuan Li, Chao Wang, Zongjin He, Yan Peng
* 🔗 **Link**：\[[arXiv:2502.00708](https://arxiv.org/abs/2502.00708)]
* 🤔 **Challenge**：Text-to-3D generation often fails when creating compositional scenes because models struggle to ensure that the layout of multiple objects complies with physical laws and accurately reflects complex semantic relationships described in text.
* 📖 **Introduction**：PhiP-G is a physics-guided framework that integrates LLM-based agents with a "world model" for scene layout. It uses LLMs to generate a scene graph and employs a physical pool (with adhesion capabilities) to predict physically plausible layouts, which then guide the generation of 3D Gaussian assets, resulting in scenes that are both semantically correct and physically consistent.



**\[5]. SplatTalk: 3D VQA with Gaussian Splatting (ICCV 2025)**

* 🧑‍🎓 **Author**：Anh Thai, Songyou Peng, Kyle Genova, Leonidas Guibas, Thomas Funkhouser
* 🔗 **Link**：\[[arXiv:2503.06271](https://arxiv.org/abs/2503.06271)]
* 🤔 **Challenge**：Zero-shot 3D Visual Question Answering (3D VQA) typically requires explicit 3D surface representations (meshes/point clouds) or large-scale 3D-language annotations, which are scarce and difficult to obtain.
* 📖 **Introduction**：SplatTalk introduces a self-supervised framework that lifts 2D vision-language features into a 3D Gaussian field. It extracts "3D tokens" from the Gaussian representation that are directly compatible with pretrained LLMs (like Qwen2), enabling the model to answer complex questions about the 3D scene's content and spatial configuration without any 3D-language supervision.



**\[4]. LIVE-GS: LLM Powers Interactive VR by Enhancing Gaussian Splatting**

* 🧑‍🎓 **Author**：Haotian Mao, Zhuoxiong Xu, Siyue Wei, Yule Quan, Nianchen Deng, Xubo Yang
* 🔗 **Link**：\[[arXiv:2412.09176](https://arxiv.org/abs/2412.09176)]
* 🤔 **Challenge**：Current interactive VR systems based on 3DGS are often limited to simple elastic deformations due to a lack of semantic understanding and physical properties, leading to unrealistic user experiences.
* 📖 **Introduction**：LIVE-GS is a highly realistic interactive VR system that integrates 3DGS with LLM-driven physics. It uses GPT-4o to analyze the physical properties of objects from images and guides a physics engine (based on the Obi solver) to simulate realistic interactions (like collisions and gravity) in real-time, bridging the gap between visual fidelity and physical plausibility.



**\[3]. ChatSplat: 3D Conversational Gaussian Splatting**

* 🧑‍🎓 **Author**：Hanlin Chen, Fangyin Wei, Gim Hee Lee
* 🔗 **Link**：\[[arXiv:2412.00734](https://arxiv.org/abs/2412.00734)]
* 🤔 **Challenge**：Interacting with 3D environments via language is often limited to simple segmentation; existing methods lack the ability to support rich, multi-level conversations (object, view, and scene levels) and often suffer from the complexity of prompt engineering.
* 📖 **Introduction**：ChatSplat constructs a 3D language field that enables comprehensive chat-based interaction within 3D space. It distinguishes between object-level, view-level, and scene-level interactions by encoding 3D scenes into "language tokens" that a pretrained LLM can process, allowing users to converse naturally with the scene about object properties and spatial arrangements.



**\[2]. Chain of Semantics Programming in 3D Gaussian Splatting Representation for 3D Vision Grounding (CVPR 2025)**

* 🧑‍🎓 **Author**：Jiaxin Shi, Mingyue Xiang, Hao Sun, Yixuan Huang, Zhi Weng
* 🔗 **Link**：\[[https://openaccess.thecvf.com/content/CVPR2025/papers/Shi\_Chain\_of\_Semantics\_Programming\_in\_3D\_Gaussian\_Splatting\_Representation\_for\_CVPR\_2025\_paper.pdf](https://openaccess.thecvf.com/content/CVPR2025/papers/Shi_Chain_of_Semantics_Programming_in_3D_Gaussian_Splatting_Representation_for_CVPR_2025_paper.pdf)]
* 🤔 **Challenge**：3D Vision Grounding (3DVG) faces difficulties in understanding fine-grained semantics and spatial relationships within implicit 3D representations; existing methods struggle to decouple these complex relationships and typically require expensive per-scene training.
* 📖 **Introduction**：This paper proposes a zero-shot neuro-symbolic framework that utilizes LLMs to perform "Chain of Semantics Programming" (CoSP). It deconstructs complex natural language utterances into a relationship graph and performs step-by-step reasoning directly within the 3D Gaussian Splatting representation, achieving state-of-the-art visual grounding without requiring densification or depth information.



**\[1]. Query3D: LLM-Powered Open-Vocabulary Scene Segmentation with Language Embedded 3D Gaussians**

* 🧑‍🎓 **Author**：Amirhosein Chahe, Lifeng Zhou
* 🔗 **Link**：\[[arXiv:2408.03516](https://arxiv.org/abs/2408.03516)]
* 🤔 **Challenge**：Open-vocabulary querying in 3D scenes (especially for autonomous driving) is critical but challenging; traditional methods relying on fixed canonical phrases fail to capture the subtle distinctions and deep scene understanding required for complex, context-dependent queries.
* 📖 **Introduction**：Query3D enhances Language Embedded 3D Gaussian Splatting (LE3DGS) with an LLM-powered query processing pipeline. It employs LLMs to dynamically generate "context-aware canonical phrases" and "helping positive words" that serve as semantic anchors, enabling precise, open-vocabulary segmentation and object localization that significantly outperforms fixed-phrase baselines.
