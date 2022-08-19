# Motivation
In most cases, the sound can be related to its sounding source in visual as the audio and visual often occur simultaneously. The sound localization task aims to find and locate the sound-related regions in videos for the input audio.


# Demo
![localization.mp4](content/videos/localization.mp4)

[Video Source](https://www.youtube.com/watch?v=XRU-R32t6rU)

# Overview of the field
- Early attempts on this task used shallow probabilistic models [1,2] or CCA-related methods [3] to associate audio and visual signal. 
- Recently, deep neural networks bring this task into a new stage. Audio-Visual Correspondence framework is a typical training scheme. It learns to maximize the similarity between sound features and the visual embeddings of the same sounding object [4,5,6].
- These methods mostly work well in simple single-source scenarios while are hard to handle the cocktail-party scenario with multiple sounding sources. Thus, Zhao et al. [7,8] combined the audio-visual source separation objective with localization task, and employed the mix-then-separate framework to generate correspondence between pixels and separated audio signals. 
- Differently, Hu et al. [9] formulated the image and sound as graphs and adopted a cycle-consistent random walk strategy for separating as well as localizing mixed sounds. 
- The above methods only locate the sounding area in videos but do not consider the semantics of objects. Hu et al. [10] employed the clustering method to establish a category-representation object dictionary and conducted class-aware sounding object localization in the cocktail-party scenario.
- Considering the above methods often only capture the coarse object contour, Zhou et al. [11] released a segmentation dataset with pixel-level annotation of localization. They introduced the audio-visual segmentation task, whose goal is to conduct pixel-level sounding localization. 
- Overall, the sound localization in video methods ground the sounding regions in visual, achieving fine-grained scene understanding.


[1] [Audio Vision: Using Audio-Visual Synchrony to Locate Sounds](https://proceedings.neurips.cc/paper/1999/hash/b618c3210e934362ac261db280128c22-Abstract.html)
[2] [Pixels that sound](https://ieeexplore.ieee.org/document/1467253)
[3] [Multimodal Analysis for Identification and Segmentation of Moving-Sounding Objects](https://ieeexplore.ieee.org/document/6357311/)
[4] [Objects that Sound](https://openaccess.thecvf.com/content_ECCV_2018/html/Relja_Arandjelovic_Objects_that_Sound_ECCV_2018_paper.html)
[5] [Audio-Visual Scene Analysis with Self-Supervised Multisensory Features](https://openaccess.thecvf.com/content_ECCV_2018/html/Andrew_Owens_Audio-Visual_Scene_Analysis_ECCV_2018_paper.html)
[6] [Learning to Localize Sound Sources in Visual Scenes: Analysis and Applications](https://ieeexplore.ieee.org/abstract/document/8894565/)
[7] [The Sound of Pixels](https://openaccess.thecvf.com/content_ECCV_2018/html/Hang_Zhao_The_Sound_of_ECCV_2018_paper.html)
[8] [The Sound of Motions](https://openaccess.thecvf.com/content_ICCV_2019/html/Zhao_The_Sound_of_Motions_ICCV_2019_paper.html)
[9] [Mix and Localize: Localizing Sound Sources in Mixtures](https://openaccess.thecvf.com/content/CVPR2022/html/Hu_Mix_and_Localize_Localizing_Sound_Sources_in_Mixtures_CVPR_2022_paper.html)
[10] [Class-aware Sounding Objects Localization via Audiovisual Correspondence](https://ieeexplore.ieee.org/abstract/document/9662191/)
[11] [Audio-Visual Segmentation](https://arxiv.org/abs/2207.05042)
