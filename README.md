# Awesome4DGeneration
A new-initialized project on 4D generation. 


# Related Work
- Marigold: Repurposing Diffusion-Based Image Generators for Monocular Depth Estimation
  [Paper](https://arxiv.org/abs/2312.02145)|[Code](https://github.com/prs-eth/Marigold)\
  - Proposed an image diffuson model exceling in monocular depth estimation.
  - Core principle: leveraging the rich visual knowledge contained in modern generative image models.
  - The finetuning data is synthesized.
  ![image](https://github.com/qiaosun22/Awesome4DGeneration/assets/136222260/f0b89787-4ff1-48cf-ae69-e13f43d86788)

- TC4D: Trajectory-Conditioned Text-to-4D Generation
  [paper](https://arxiv.org/pdf/2403.17920)|[Code](https://github.com/sherwinbahmani/tc4d?tab=readme-ov-file)\
  - Background: Existing models are limited in generating large-scale motion due to their confined representation methods.
  - TC4D addresses this by decomposing motion into global (rigid transformation along a spline trajectory) and local (deformations aligned with global trajectory) components, using supervision from text-to-video models.
  - This enables the creation of scenes with complex motion paths and enhanced visual fidelity, validated through qualitative evaluation and user studies.
  ![image](https://github.com/user-attachments/assets/94bb0e2f-1916-4686-bf9a-bb51a4bc4cf4)

- 4D-fy: Text-to-4D Generation Using Hybrid Score Distillation Sampling
  [paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Bahmani_4D-fy_Text-to-4D_Generation_Using_Hybrid_Score_Distillation_Sampling_CVPR_2024_paper.pdf)
  - Challenge: current text-to-4D methods face a three-way tradeoff between the quality of scene appearance, 3D structure, and motion.
  - Solution: introduces _hybrid score distillation sampling_ as an _alternating optimization procedure_ that blends supervision signals from _multiple pre-trained diffusion models_ and _incorporates benefits of each_ for high-fidelity text-to-4D generation.
