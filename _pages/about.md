---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

About Me
======
Currently, I'm an integration engeer working in BYD company limited. Prior to this, I received my master's degree of Mechanical Engineering from [Harbin Institute of Technology](https://www.hit.edu.cn/). My research interest focus on developing universal multimodal architectures for content generation, improving learning efficiency/accuracy, and enhancing model interpretability.
You can find my CV here: [Curriculum Vitae](../assets/CV-YongsongYang.pdf).

Research
======
**Quantized Prompt-guided Video Generation via Stable Video Diffusion Model**  
•	Quantization strategy from FP32 to FP16 was implemented achieving a 50% reduction in model size.  
•	SVD model was finetuned with LoRA, and optimizing loss between predicted and actual noise  
•	Text embedding from CLIP and random noise are processed by a U-Net with cross attention.  
•	After iterative denoising via a scheduler, the refined latent is decoded by a VAE into the final video.  

**3D Image Segmentation based on Distilled Separate Anything Model**  
•	SAM was built and full parameters were fine-tuned based on pretrained model leveraging 3d image dataset;  
•	Image encoder TinyViT was distilled from ViT by imposing the image embedding outputs to be the same;  
•	The Distilled SAM strikes a balance among model size, segmentation accuracy and inference speed;  

**Mamba-UNet for 3D Segmentation via Cross Semi-Supervised Learning**  
•	Mamba was built based on encoder-decoder structure with skip connections for multi-scale feature fusion;  
•	Model is trained on pseudo-label produced by Unet and MambaUnet via cross supervised learning;  
•	Validation results showed superior performance in IoU and accuracy compared to classic network Unet;  

**Adaptive Fine-tuning of YOLOv11 for Robust Person Detection in Dynamic scenes**  
•	The YOLOv11n model's robustness was enhanced through fine-tuning on the multi-scene WiderPerson dataset;  
•	Hierarchical learning rates were employed to optimize YOLOv11n's feature retention and adaptation ability;  
•	Redundant convolutional layers were pruned based on gradient importance to optimize model inference speed;  

**Dual-timescale Joint Estimation for Battery States based on Transfer Learning**  
•	Ada-CNN-GRU-Ave model was proposed leveraging cross time scale characteristics for state of health estimation;  
•	Joint states estimation model was proposed leveraging previous states output and current characteristics input, achieving higher prediction accuracy and generalization;  

**Sparse Data Reconstruction based on Masked Auto-Encoder with extrapolator**  
•	Time series data was sampled to sparse data and sent to the cloud for data generate and reconstruction;  
•	Via self-supervised learning, ExtraMAE was built to capture temporal dynamics of original time series;  
•	Extrapolator was built to recover latent representations and mapping them back into the feature space;  
•	The model attained state prediction accuracy exceeding 90% based on the reconstructed time series data;  

**Battery State-of-Charge Estimation based on Cross Domain Transfer Learning**  
•	Distilled Ada-CNN-GRU was proposed by reducing source-target domain distribution diversity;  
•	Error feedback structure was proposed leveraging model bias as feature to calibrate estimation results;  
•	Combining Kalman Filter as post-processor, robustness and accuracy of state estimation were improved;  
