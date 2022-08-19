# Motivation
Humans' audition system can determine the location of hearing sounds, which is called the binaural effect. The recorded binaural audio is then expected to recover the stereo sound sensation. However, recording such a spatial sound requires special equipment that is not easily accessible. Hence, the audio-visual spatial consistency inspires researchers to generate spatial sound with the guidance of visual information.


# Demo
![spatial.mp4](content/videos/spatial.mp4)

[Video Source](https://www.youtube.com/watch?v=Wrx3pv_ixdI&t=144s)


# Overview of the field
- Li et al. [1] proposed to generate the stereo sound of a specific room via integrating synthesised early reverberation and measured late reverberation tail, while Morgado et al. [2] adopted an end-to-end deep neural framework for ambisonic sound generation using $360^{\circ}$ videos. However, $360^{\circ}$ videos are limited in amounts and scenarios, making these methods cannot generalize to other environments well. 
- Subsequently, some studies are proposed to use the Normal Field of View videos for reconstructing binaural audio from mono sound, driven by the visual location of the sounding source [3,4,5]~\cite{gao20192,lu2019self,parida2022beyond}. These methods are built in a data-driven way, relying on the ground truth stereo sound as the supervision. Although they achieve promising performance, the supervised manner narrows their application to the specific scenes. 
- Thus, Zhou et al. [6] formulated the spatial sound generation task into an extreme case of sound separation, combining stereo sound and mono sound as training data to improve model performance and generalization.
- To further alleviate the dependence on the insufficient and expensive stereo sound, Xu et al. [7] utilized the head-related impulse response and spherical harmonic decomposition to build pseudo visual-stereo pairs from mono sound data. Instead, Lin et al. [8] exploited the association between each audio component and the spatial regions of interest to explore the audio-visual spatial consistency. 
- As stated, spatial sound generation methods gradually alleviate reliance on ground truth stereo videos, expanding their application scenarios.


[1] [Scene-aware Audio for 360 Videos](https://arxiv.org/pdf/1805.04792.pdf)
[2] [Self-Supervised Generation of Spatial Audio for 360° Video](https://proceedings.neurips.cc/paper/2018/hash/01161aaa0b6d1345dd8fe4e481144d84-Abstract.html)
[3] [2.5D Visual Sound](https://openaccess.thecvf.com/content_CVPR_2019/html/Gao_2.5D_Visual_Sound_CVPR_2019_paper.html) 
[4] [Self-Supervised Audio Spatialization with Correspondence Classifier](https://ieeexplore.ieee.org/abstract/document/8803494/)
[5] [Beyond Mono to Binaural: Generating Binaural Audio From Mono Audio With Depth and Cross Modal Attention](https://openaccess.thecvf.com/content/WACV2022/html/Parida_Beyond_Mono_to_Binaural_Generating_Binaural_Audio_From_Mono_Audio_WACV_2022_paper.html)
[6] [Sep-Stereo: Visually Guided Stereophonic Audio Generation by Associating Source Separation](https://link.springer.com/chapter/10.1007/978-3-030-58610-2_4)
[7] [Visually Informed Binaural Audio Generation without Binaural Audios](https://openaccess.thecvf.com/content/CVPR2021/html/Xu_Visually_Informed_Binaural_Audio_Generation_without_Binaural_Audios_CVPR_2021_paper.html), 2021
[8] [Exploiting Audio-Visual Consistency with Partial Supervision for Spatial Audio Generation](https://ojs.aaai.org/index.php/AAAI/article/view/16302)