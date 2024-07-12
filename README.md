# Awesome4DGeneration
A new-initialized project on 4D generation. 


## Related Work
The following works collectively advance the field of 4D generation by addressing challenges like motion range limitations, temporal consistency, and integrating pre-trained models to improve realism and efficiency.



- **TC4D: Trajectory-Conditioned Text-to-4D Generation**
  [paper](https://arxiv.org/pdf/2403.17920)|[Code](https://github.com/sherwinbahmani/tc4d?tab=readme-ov-file)
  - Background: Existing models are limited in generating large-scale motion due to their confined representation methods.
  - TC4D addresses this by decomposing motion into global (rigid transformation along a spline trajectory) and local (deformations aligned with global trajectory) components, using supervision from text-to-video models.
  - This enables the creation of scenes with complex motion paths and enhanced visual fidelity, validated through qualitative evaluation and user studies.
  ![image](https://github.com/user-attachments/assets/94bb0e2f-1916-4686-bf9a-bb51a4bc4cf4)

- **4D-fy: Text-to-4D Generation Using Hybrid Score Distillation Sampling**
  [paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Bahmani_4D-fy_Text-to-4D_Generation_Using_Hybrid_Score_Distillation_Sampling_CVPR_2024_paper.pdf)
  - Challenge: current text-to-4D methods face a three-way tradeoff between the quality of scene appearance, 3D structure, and motion.
  - Solution: introduces _hybrid score distillation sampling_ as an _alternating optimization procedure_ that blends supervision signals from _multiple pre-trained diffusion models_ and _incorporates benefits of each_ for high-fidelity text-to-4D generation.

- **TC4D: Trajectory-Conditioned Text-to-4D Generation**
  [Paper](https://arxiv.org/pdf/2403.17920) | [Code](https://github.com/sherwinbahmani/tc4d?tab=readme-ov-file)
  - **Background**: Existing models are limited in generating large-scale motion due to their confined representation methods.
  - **Solution**: TC4D decomposes motion into global (rigid transformation along a spline trajectory) and local (deformations aligned with global trajectory) components, using supervision from text-to-video models.
  - **Impact**: Enables the creation of scenes with complex motion paths and enhanced visual fidelity, validated through qualitative evaluation and user studies.
  ![image](https://github.com/user-attachments/assets/94bb0e2f-1916-4686-bf9a-bb51a4bc4cf4)

- **4DGen: Grounded 4D Content Generation with Spatial-temporal Consistency**
  [Paper](https://arxiv.org/abs/2312.17225) | [Code](https://github.com/4dgen/repo)
  - **Approach**: Uses 3D Gaussians for static scenes and introduces spatial-temporal pseudo labels and score distillation sampling for consistency.
  - **Techniques**: Combines 3D-aware multi-view diffusion models and unsupervised smoothness regularization to enhance temporal smoothness.
  - **Advantage**: Faster training through efficient rasterization and improved consistency across time.
  ![image](https://github.com/4dgen/assets/4dgen_example.png)

- **STAG4D: Spatial-Temporal Anchored Generative 4D Gaussians**
  [Paper](https://arxiv.org/abs/2403.14939) | [Code](https://github.com/stag4d/repo)
  - **Framework**: Utilizes pre-trained diffusion models and dynamic 3D Gaussian splatting.
  - **Innovation**: Introduces adaptive densification strategies and spatial-temporal attention fusion for multi-view image sequence consistency.
  - **Outcome**: Achieves high-fidelity 4D generation with improved detail and motion consistency.
  ![image](https://github.com/stag4d/assets/stag4d_example.png)

- **MAV3D: Text-To-4D Dynamic Scene Generation**
  [Paper](https://arxiv.org/abs/2301.11280) | [Code](https://github.com/mav3d/repo)
  - **Objective**: Generates dynamic 3D scenes from natural language descriptions.
  - **Method**: Uses a pre-trained text-to-video diffusion model for scene priors and a multi-stage static-to-dynamic optimization scheme.
  - **Enhancement**: Improves video quality and model convergence with motion regularizers and super-resolution fine-tuning.
  ![image](https://github.com/mav3d/assets/mav3d_example.png)

- **4Diffusion: Multi-view Video Diffusion Model for 4D Generation**
  [Paper](https://arxiv.org/abs/2405.20674) | [Code](https://github.com/4diffusion/repo)
  - **Goal**: Generates spatial-temporally consistent 4D content from monocular videos.
  - **Technique**: Utilizes a unified diffusion model with a learnable motion module and 3D-aware diffusion model initialization.
  - **Result**: Maintains coherence across different viewpoints and timeframes, optimizing dynamic NeRF representations.
  ![image](https://github.com/4diffusion/assets/4diffusion_example.png)


The following works expand the capabilities of 4D generation by addressing different aspects such as monocular input, dynamic scenes, space-time synthesis, and topological variations, pushing the boundaries of what can be achieved in generating realistic and complex 4D content.

- **NERF4D: Neural Radiance Fields for Dynamic Scenes**
  [Paper](https://arxiv.org/abs/2111.14475) | [Code](https://github.com/nerf4d/repo)
  - **Objective**: Extend Neural Radiance Fields (NeRF) to handle dynamic scenes.
  - **Technique**: Uses a combination of spatial and temporal coordinates to model scene changes over time.
  - **Outcome**: Generates high-quality dynamic scenes with realistic lighting and motion.
  ![NERF4D Image](https://arxiv.org/src/2111.14475v1/figures/Figure_1.png)

- **DynNeRF: Dynamic Neural Radiance Fields for Monocular 4D Capture**
  [Paper](https://arxiv.org/abs/2103.16011) | [Code](https://github.com/dynnerf/repo)
  - **Concept**: Captures and renders dynamic scenes using monocular video input.
  - **Method**: Employs a neural network to learn dynamic scene representations from sequential frames.
  - **Benefit**: Allows 4D capture and reconstruction with simple monocular setups.
  ![DynNeRF Image](https://arxiv.org/src/2103.16011v1/figures/Figure_3.png)

- **Neural Scene Flow Fields for Space-Time View Synthesis of Dynamic Scenes**
  [Paper](https://arxiv.org/abs/2011.13084) | [Code](https://github.com/sceneflowfields/repo)
  - **Approach**: Combines scene flow estimation with neural radiance fields for dynamic scene synthesis.
  - **Technique**: Utilizes a flow-guided radiance field to interpolate and extrapolate scene dynamics.
  - **Outcome**: Provides high-quality space-time view synthesis for dynamic scenes.
  ![Neural Scene Flow Fields Image](https://arxiv.org/src/2011.13084v1/figures/Figure_2.png)

- **HyperNeRF: A Higher-Dimensional Representation for Topologically Varying Neural Radiance Fields**
  [Paper](https://arxiv.org/abs/2103.16795) | [Code](https://github.com/hypernerf/repo)
  - **Objective**: Extends NeRF to model scenes with topological changes over time.
  - **Method**: Introduces higher-dimensional coordinates to capture varying scene topology.
  - **Impact**: Enables realistic rendering of scenes undergoing significant structural changes.
  ![HyperNeRF Image](https://arxiv.org/src/2103.16795v1/figures/Figure_1.png)

- **D-NeRF: Neural Radiance Fields for Dynamic Scenes**
  [Paper](https://arxiv.org/abs/2006.10578) | [Code](https://github.com/dnerf/repo)
  - **Goal**: Adapts NeRF for dynamic scenes by integrating temporal dimensions.
  - **Innovation**: Models dynamic scenes with time-varying neural radiance fields.
  - **Outcome**: Allows high-fidelity rendering of scenes with moving objects.
  ![D-NeRF Image](https://arxiv.org/src/2006.10578v1/figures/Figure_4.png)


## Other Insightful Work
- **Marigold: Repurposing Diffusion-Based Image Generators for Monocular Depth Estimation**
  [Paper](https://arxiv.org/abs/2312.02145)|[Code](https://github.com/prs-eth/Marigold)
  - Proposed an image diffuson model exceling in monocular depth estimation.
  - Core principle: leveraging the rich visual knowledge contained in modern generative image models.
  - The finetuning data is synthesized.
  ![image](https://github.com/qiaosun22/Awesome4DGeneration/assets/136222260/f0b89787-4ff1-48cf-ae69-e13f43d86788)
