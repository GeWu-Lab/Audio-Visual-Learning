# Motivation
The saliency detection task aims to model the human attention mechanism. In daily life, our attention can be attracted by salient objects or things. Originally, saliency detection tasks only take visual information as the input, which aims to detect eye-attracting components in images or videos. Although humans rely on the visual system to perceive the surroundings to a great extent, other senses, especially hearing, can also affect the perception results. To comprehensively explore the human attention mechanism, it is necessary to integrate audio and visual.


# Demo
![saliency.mp4](content/videos/saliency.mp4)

[Video Source](https://www.youtube.com/watch?v=P62uIZxGM-U)

# Overview of the field
- The early studies in audio-visual saliency detection often utilized traditional hand-craft techniques to detect audio and visual saliency respectively then fused the uni-modal saliency map [1,2,3]. 
- These methods lack the consideration of inter-modal correlation. Recently, a series of deep-based saliency detection methods have emerged [4,5,6,7]. 
- Tavakoli et al. [4] designed a two-stream framework and used the concatenation fusion strategy, which is a relatively basic model. Further, STAViS model [5] is proposed to combine audio-visual information at multiple stages. 
- However, the dependence on the human eye-fixation label hinders the development of this field, since it is laborious to collect and annotate massive videos. Therefore, Wang et al. [8] designed a strategy for converting audio-visual semantic category tags into pseudo eye-fixation labels. Then they trained the saliency detection model in a weakly-supervised manner. 
- Overall, audio-visual saliency detection is a developing field and more in-depth exploration is expected.


[1] [Multimodal Saliency-based Bottom-up Attention a Framework for the Humanoid Robot iCub](https://ieeexplore.ieee.org/abstract/document/4543329/)
[2] [Multimodal Saliency-based Attention for Object-based Scene Analysis](https://ieeexplore.ieee.org/document/6095124)
[3] [Fixation Prediction through Multimodal Analysis](https://dl.acm.org/doi/10.1145/2996463)
[4] [DAVE: A Deep Audio-Visual Embedding for Dynamic Saliency Prediction](https://arxiv.org/abs/1905.10693)
[5] [STAViS: Spatio-Temporal AudioVisual Saliency Network](https://openaccess.thecvf.com/content_CVPR_2020/html/Tsiami_STAViS_Spatio-Temporal_AudioVisual_Saliency_Network_CVPR_2020_paper.html)
[6] [A Multimodal Saliency Model for Videos With High Audio-visual Correspondence](https://ieeexplore.ieee.org/abstract/document/8962278/)
[7] [ViNet: Pushing the limits of Visual Modality for Audio-Visuav Saliency Prediction](https://ieeexplore.ieee.org/abstract/document/9635989)
[8] [From Semantic Categories to Fixations: A Novel Weakly-Supervised Visual-Auditory Saliency Detection Approach](https://openaccess.thecvf.com/content/CVPR2021/html/Wang_From_Semantic_Categories_to_Fixations_A_Novel_Weakly-Supervised_Visual-Auditory_Saliency_CVPR_2021_paper.html)