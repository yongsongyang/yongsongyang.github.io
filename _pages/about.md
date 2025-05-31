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
Currently, I'm an integration engeer working in BYD company limited. Prior to this, I received my master's degree of Mechanical Engineering from [Harbin Institute of Technology](https://www.hit.edu.cn/). My research interest focus on State Estimation; Object Detection; Image Segmentation; Model Distillation; Multimodal Learning.
You can find my [CV](../assets/CV-YongsongYang.pdf) there.

Research
======
**Quantized Prompt-guided Video Generation via Stable Video Diffusion Model**  
•	Built the stable video diffusion (SVD) model, and implemented a quantization strategy, reducing the model size by 65% by converting weights from FP32 to INT8 without significant performance loss.  
•	Fine-tuned the SVD model using Low-Rank Adaptation (LoRA), optimizing the loss between predicted and actual noise to enhance generation quality.  
•	Processed CLIP text embeddings and random noise through a U-Net with cross-attention mechanisms, ensuring alignment between prompts and generated frames.  
•	To generate high-quality videos, the refined latent representation is decoded by variational autoencoder (VAE) after iterative denoising via a scheduler.  

**3D Image Segmentation based on Distilled Separate Anything Model**  
•	For efficient medical image segmentation, medical segment anything model (MedSAM) was re-built and trained on diverse medical datasets, achieving robust performance across various modalities.  
•	To address the challenge of high computational costs while maintaining accuracy, image encoder TinyViT was distilled from the original ViT by imposing the image embedding outputs to be the same.  
•	The results validated LiteMedSAM's ability to deliver accurate segmentation with reduced resource requirements, aligning with the original goal of enhancing accessibility for medical image analysis.  

**Mamba-UNet for 3D Segmentation via Cross Semi-Supervised Learning**  
•	Semi-Mamba-UNet, a novel semi-supervised medical image segmentation framework integrating Visual Mamba with U-Net, was reproduced to address the challenges of limited annotations and long-range dependency modeling in medical imaging.  
•	The model leverages pixel-level contrastive learning and cross-supervised training between Mamba-UNet and CNN-based UNet to enhance feature learning and pseudo-label quality.  
•	Experimental results on ACDC datasets demonstrated superior performance, achieving 91.14% Dice on cardiac MRI by effectively combining Mamba's global context capture with semi-supervised learning, showcasing its potential for practical applications with sparse annotations.   

**Adaptive Fine-tuning of YOLOv11 for Robust Person Detection in Dynamic scenes**  
•	Enhanced the YOLOv11n model's robustness by fine-tuning it on the multi-scene WiderPerson dataset, improving its detection accuracy in dynamic environments.  
•	To optimize feature retention and adaptation ability, hierarchical learning rates was implemented, ensuring balanced updates across different network layers.  
•	Streamlined the model by pruning redundant convolutional layers based on gradient importance analysis, significantly boosting inference speed without compromising detection performance.  
•	The refinements collectively improved the model's efficiency and adaptability for real-world person detection tasks in occlusions, scale variations, and diverse environmental conditions.  

**Dual-timescale Joint Estimation for Battery States based on Transfer Learning**  
•	For State of Health (SOH) estimation under dynamic working conditions, an Ada-CNN-GRU-Ave model was developed. Utilizing dual-time scale inputs, the model achieved an MAE of 0.02% and RMSE of 0.03%, significantly outperforming traditional methods.  
•	To enable joint SOC and SOH estimation, a Joint Adaptive Deep Transfer Learning (JADTL) model was introduced leveraging previous states output and current characteristics input. By combining Ada-CNN-GRU-KF and Ada-CNN-GRU-Ave, the model achieved MAE of 0.99% (SOC) and 0.07% (SOH).  
•	To overcome data redundancy and computational inefficiency in SOH estimation, a novel sampling strategy (0.1 Hz) and averaging post-processor were implemented. This reduced computational burden while maintaining high accuracy, with results converging within 15 seconds despite extreme initial errors.  

**Sparse Data Reconstruction based on Masked Auto-Encoder with extrapolator**  
•	To address the challenge of limited computational resource in edge devices and cloud transmission bandwidth for edge-cloud collaboration computing, this study proposes an Extrapolator Masked Autoencoder (ExtraMAE) framework for data reconstruction.  
•	Sampled time series data into sparse inputs (with 80% masking), then employs a self-supervised learning architecture with GRU-based encoder that captures temporal dynamics from unmasked patches.  
•	Recovered latent representations of masked patches through feature-space interpolation by an extrapolator, and reconstructed dense time series from a GRU-based decoder while preserving original unmasked values.  
•	The model enabled downstream SOC estimation with MAE of 0.29% on the reconstructed time series data - outperforming the estimation result with MAE of 1.50% under sparse data.  

**Battery State-of-Charge Estimation based on Cross Domain Transfer Learning**  
•	To extract the information in multidimensional time series, CNN layers were implemented for spatial feature learning while GRU layers were utilized for temporal dependency capture.  
•	For the generalization of SOC estimation under varying conditions, a distilled Ada-CNN-GRU was proposed by reducing source-target domain distribution diversity, achieving sub-1% MAE under dynamic driving cycles.  
•	For steady estimation outputs, Kalman filter is implemented as a post data processor to smooth fluctuations.  
•	A novel feedback mechanism was implemented to predict and correct systematic errors. By training a secondary model to estimate SOC errors and feeding them back as inputs, the framework reduced estimation inaccuracies.

