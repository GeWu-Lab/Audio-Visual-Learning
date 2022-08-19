# Motivation
The audio-visual question answering and dialog task aim to conduct cross-modal spatial-temporal reasoning about the audio-visual scenes.


# Demo
![qa.jpg](content/images/qa.jpg)

[Image Source](https://gewu-lab.github.io/MUSIC-AVQA/)

# Overview of the field
- The uni-modal question answering tasks have been sufficiently studied, but they are hard to be equipped with more realistic inference ability with partial information of scenes. Since sight and hearing are two vital senses in human cognition, the audio-visual question answering task has emerged recently [1,2]. 
- Yun et al. [1] brought up the Pano-AVQA dataset, containing $360^{\circ}$ videos and corresponding question-answer pairs. The Pano-AVQA dataset covers two types of question-answer pairs: spherical spatial relation and audio-visual relation, to better explore the understanding of the panoramic scenes. 
- Li et al. [2] proposed a large-scale MUSIC-AVQA dataset to facilitate spatial-temporal reasoning under dynamic and long-term audio-visual scenes. The audio-visual scenes in MUSIC-AVQA are mainly musical performances which is a typical multi-modal scenario with abundant audio-visual components and their interaction. To achieve effective question answering, they first visually grounded the sounding regions, then conducted spatial-temporal reasoning with attention mechanism.
- Recently, another active area is audio-visual scene-aware dialog. It aims to train the agent that can converse with humans about a temporally varying audio-visual scene, using natural, conversational language [3,4,5,6]. Compared with question-answering, the scene-aware dialog further considers the context of conversations. 
- Alamri et al. [3] first collected the Audio Visual Scene-Aware Dialog dataset where each sample contains a scene-aware dialog about the video. They provided a simple baseline that leveraged the history dialog and audio-visual input to rank candidate answers. 
- Schwartz et al. [6] adopted an end-to-end training strategy. They used a multi-modal attention mechanism to capture cross-modal interactions, then utilized a LSTM module to generate answers.
- To effectively represent then infer on multiple modalities, Geng et al. [7] presented a spatio-temporal scene graph to capture key audio-visual cues, then used a sequential transformer-based mechanism to highlight the question-aware representations for answer generation.
- Overall, the above question answering as well as dialog tasks attempt to explore the audio-visual correlations of events in spatial and temporal, based on the decoupled audio-visual scenes. This is a hopeful direction to better mimic the scene understanding ability of humans.


[1] [Pano-AVQA: Grounded Audio-Visual Question Answering on 360deg Videos](https://openaccess.thecvf.com/content/ICCV2021/html/Yun_Pano-AVQA_Grounded_Audio-Visual_Question_Answering_on_360deg_Videos_ICCV_2021_paper.html)
[2] [Learning To Answer Questions in Dynamic Audio-Visual Scenarios](https://openaccess.thecvf.com/content/CVPR2022/html/Li_Learning_To_Answer_Questions_in_Dynamic_Audio-Visual_Scenarios_CVPR_2022_paper.html)
[3] [Audio Visual Scene-Aware Dialog](https://openaccess.thecvf.com/content_CVPR_2019/html/Alamri_Audio_Visual_Scene-Aware_Dialog_CVPR_2019_paper.html)
[4] [Joint Student-Teacher Learning for Audio-Visual Scene-Aware Dialog](https://www.merl.com/publications/docs/TR2019-097.pdf)
[5] [End-to-end Audio Visual Scene-aware Dialog Using Multimodal Attention-based Video Features](https://ieeexplore.ieee.org/abstract/document/8682583)
[6] [A Simple Baseline for Audio-Visual Scene-Aware Dialog](https://openaccess.thecvf.com/content_CVPR_2019/html/Schwartz_A_Simple_Baseline_for_Audio-Visual_Scene-Aware_Dialog_CVPR_2019_paper.html)
[7] [Dynamic Graph Representation Learning for Video Dialog via Multi-Modal Shuffled Transformers](https://ojs.aaai.org/index.php/AAAI/article/view/16231)