# Motivation
In most audio-visual tasks, like audio-visual correspondence, the audio and visual context is assumed to be matched over the whole video. But videos, especially unconstrained videos, often contain temporally irrelevant audio-visual segments. For example, only some segments of videos with the action ''playing the basketball'' are both audible and visible for this action, since the camera can move to the audience during the shoot. 

# Demo
![parsing.png](content/images/parsing.png)

[Image Source](https://link.springer.com/chapter/10.1007/978-3-030-58580-8_26)


# Overview of the field
- Tian et al. [1] first introduced the audio-visual event localization task, which aims to temporally demarcate both audible and visible events from a video. They treated this task as a sequence labelling problem. An audio-driven visual attention mechanism is developed to localize sounding objects in visual and a dual multi-modal residual network is designed to integrate audio-visual features. 
- Subsequently, Lin et al. [2] used LSTM to solve the event localization in a sequence-to-sequence manner, integrating both global and local audio-visual information. With a similar purpose that capturing global information, Wu et al. [3] designed the dual attention matching module to model both the high-level event information as well as local temporal information. 
- Besides, other attention mechanisms are following proposed to explore the inter- and intra-modal correlations [4,5]}. To filter the interference of irrelevant audio-visual pairs during training, Zhou et al. [6] presented the Positive Sample Propagation method to select audio-visual pairs with positive connections and ignore the negative ones. 
- Further considering the noisy background, Xia et al. [7] designed the cross-modal time-level and event-level background suppression mechanism to alleviate the audio-visual inconsistency problem. 
- The audio-visual event localization task aims to highlight both audible and visible segments of a video. This strict constraint is hard to well ground the action in the ''in the wild'' video, where the audio and visual information is often not aligned, e.g., the out-of-screen case. Hence, the audio-visual video parsing task, which detects audible, visible and audible-visible events in the temporal dimension, is introduced to have a more fine-grained audio-visual scene understanding [8]. 
- Tian et al. [8] formulated the audio-visual parsing as the multi-modal multiple instances learning in a weakly-supervised manner. They adopted a hybrid attention network and multi-modal multiple instance learning pooling method to aggregate and exploit the multi-modal temporal contexts, then discovered and mitigated the noisy label for each modality. 
- To generate more reliable uni-modal localization results, Wu et al. [9] individually predicted event labels for each modality via exchanging audio or visual track with other unrelated videos. This strategy is based on assumption that the prediction of the synthetic video would still be confident if the uni-modal signals indeed contain information about the target event. 
- In addition, Lin et al. [10] proposed to leverage the event semantics information across videos and the correlation between event categories to better distinguish and locate different events. 
- Later, more audio-visual parsing methods are presented with improvement at feature aggregation or attention module [11,12]. 
- Overall, the audio-visual event localization and parsing task ground audio-visual events of each modality temporally, obtaining a more fine-grained perception and understanding of audio-visual scenes.


[1] [Audio-visual Event Localization in Unconstrained Videos](https://openaccess.thecvf.com/content_ECCV_2018/html/Yapeng_Tian_Audio-Visual_Event_Localization_ECCV_2018_paper.html)
[2] [Dual-modality Seq2Seq Network for Audio-visual Event Localization](https://ieeexplore.ieee.org/abstract/document/8683226/)
[3] [Dual Attention Matching for Audio-Visual Event Localization](https://openaccess.thecvf.com/content_ICCV_2019/html/Wu_Dual_Attention_Matching_for_Audio-Visual_Event_Localization_ICCV_2019_paper.html)
[4] [Audiovisual Transformer with Instance Attention for Audio-Visual Event Localization](https://openaccess.thecvf.com/content/ACCV2020/html/Lin_Audiovisual_Transformer_with_Instance_Attention_for_Audio-Visual_Event_Localization_ACCV_2020_paper.html)
[5] [Audio-Visual Event Localization via Recursive Fusion by Joint Co-Attention](https://openaccess.thecvf.com/content/WACV2021/html/Duan_Audio-Visual_Event_Localization_via_Recursive_Fusion_by_Joint_Co-Attention_WACV_2021_paper.html)
[6] [Positive Sample Propagation along the Audio-Visual Event Line](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhou_Positive_Sample_Propagation_Along_the_Audio-Visual_Event_Line_CVPR_2021_paper.pdf)
[7] [Cross-Modal Background Suppression for Audio-Visual Event Localization](https://openaccess.thecvf.com/content/CVPR2022/html/Xia_Cross-Modal_Background_Suppression_for_Audio-Visual_Event_Localization_CVPR_2022_paper.html)
[8] [Unified Multisensory Perception: Weakly-Supervised Audio-Visual Video Parsing](https://link.springer.com/chapter/10.1007/978-3-030-58580-8_26)
[9] [Exploring Heterogeneous Clues for Weakly-Supervised Audio-Visual Video Parsing](https://openaccess.thecvf.com/content/CVPR2021/html/Wu_Exploring_Heterogeneous_Clues_for_Weakly-Supervised_Audio-Visual_Video_Parsing_CVPR_2021_paper.html)
[10] [Exploring Cross-Video and Cross-Modality Signals for Weakly-Supervised Audio-Visual Video Parsing](https://proceedings.neurips.cc/paper/2021/hash/5f93f983524def3dca464469d2cf9f3e-Abstract.html)
[11] [Investigating Modality Bias in Audio Visual Video Parsing](https://arxiv.org/abs/2203.16860)
[12] [Distributed Audio-Visual Parsing Based On Multimodal Transformer and Deep Joint Source Channel Coding](https://ieeexplore.ieee.org/abstract/document/9746660/)
