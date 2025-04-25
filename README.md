% # PPD_IQA

# PPD-IQA: A Bottom-Up and Top-Down Combined Approach for Blind Image Quality Assessment via Prototype-Prompted Disentangling

This repository is a PyTorch implementation of PPD-IQA (accepted by IEEE TRANSACTIONS ON EMERGING TOPICS IN COMPUTATIONAL INTELLIGENCE ). The code of PPD-IQA is being organized.

#### Abstract
Blind Image Quality Assessment (BIQA) aims to predict the image quality automatically by mimicking the perception mechanism of the human vision system (HVS). As a perception task, BIQA should consider the synergy of bottom-up and top-down information. The bottom-up and top-down information are sensory information and task-relevant prior information, respectively. Specifically, we consider that quality perception derives from the synergy of bottom-up information obtained from vision sensory and the quality-shared prior as top-down information, which is learned by HVS during daily life. Recently, with the successful application of large pre-trained vision-language models like CLIP in prompting downstream tasks, a series of prompt-based BIQA methods are proposed to obtain top-down information and synergize it with bottom-up information for the final quality-oriented features. However, directly deploying such models for BIQA is challenging since additional annotations and well-designed prompt templates are required and a slight change in template wording could have a huge impact on performance. To avoid these challenges, we proposed a novel end-to-end method, dubbed PPD-IQA, which learns the top-down information from a proxy classification task without a pre-trained vision-language model by prototype learning. The learned top-down information is referred to as a group of quality prototypes, representing centers of samples with similar quality perception. Prompted by the quality prototypes, we can disentangle the bottom-up tokens extracted by a pre-trained Vision Transformer (ViT) into quality-shared and content-specific features in the perception space, which generate final quality predictions synergistically. The experimental results demonstrate that our method can achieve competitive performance on both synthetic and authentic IQA datasets without any additional annotations and well-designed prompt templates, which is more practical in real-world applications.




#### Citation
If our work is valuable to you, please cite our work:
```
@ARTICLE{wang2025ppd,
  author={Wang, Hui and Zhang, Zhongzhou and Yang, Ziyuan and Wang, Guangcheng and Zhang, Yi},
  journal={IEEE TRANSACTIONS ON EMERGING TOPICS IN COMPUTATIONAL INTELLIGENCE}, 
  title={PPD-IQA: A Bottom-Up and Top-Down Combined Approach for Blind Image Quality Assessment via Prototype-Prompted Disentangling}, 
  year={2025}
```
