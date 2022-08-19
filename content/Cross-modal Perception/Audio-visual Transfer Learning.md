# Motivation
The audio-visual consistency in semantics suggests that the learning of one modality is expected to be aided by the semantic knowledge of the other one. This is the aim of the audio-visual transfer learning task. 


# Demo
![soundnet.jpg](content/images/soundnet.jpg)

[Image Source](https://proceedings.neurips.cc/paper/2016/hash/7dcd340d84f762eba80aa538b0c527f7-Abstract.html)


# Overview of the field
- To avoid the expensive and time-consuming labelling process, Aytar et al. [1] designed a teacher-student network to train the student audio model with a pre-trained vision teacher, by resorting to large-scale and economically acquired unlabelled videos
- Correspondingly, Owens et al. [2] proposed to use the ambient sound as a supervisory signal to learn visual representations. 
- Afterwards, Gan et al. [3] also trained the stereo sound student model by transferring the knowledge of the visual teacher for the vehicle tracking task. Their model can independently localize the object purely based on stereo sound during the test. 
- The above strategy only uses the RGB visual teacher during training, which limits their performance, since RGB modality is vulnerable to the variants of factors like weather and illumination. 
- Hence, Valverde et al. [4] combined multiple visual teacher networks, including RGB, depth, and thermal, to fully utilize the complementary visual cues for improving the robustness of audio student network. 
- Similarly, Yin et al. [5] designed a robust audio-visual teacher network to fuse complementary information of multiple modalities, facilitating the learning of the visual student network. Instead, Zhang et al. [6] distilled the knowledge of audio-visual teachers at three different levels: label-level, embedding-level and distribution level. 
- To sum up, the above methods strengthen the distillation performance by increasing teacher numbers or distillation levels.
- In contrast, Xue et al. [7] used a uni-modal teacher to train a multi-modal student. They found that the student could correct inaccurate predictions and generalize better than its uni-modal teacher. 
- However, the employed videos for transfer are often ``in the wild'', thus visual can be unaligned with the accompanying audio (e.g., audio is background music), which brings noise for transfer learning. Chen et al. [8] considered this scenario and proposed to capture the task-related semantics via compositional contrastive learning for robust transfer.
- Overall, existing methods strengthen the transfer quality in terms of number of teachers, transfer levels as well as transfer robustness.


[1] [SoundNet: Learning Sound Representations from Unlabeled Video](https://proceedings.neurips.cc/paper/2016/hash/7dcd340d84f762eba80aa538b0c527f7-Abstract.html)
[2] [Ambient Sound Provides Supervision for Visual Learning](https://arxiv.org/abs/1608.07017)
[3] [Self-Supervised Moving Vehicle Tracking With Stereo Sound](https://openaccess.thecvf.com/content_ICCV_2019/html/Gan_Self-Supervised_Moving_Vehicle_Tracking_With_Stereo_Sound_ICCV_2019_paper.html)
[4] [There Is More Than Meets the Eye: Self-Supervised Multi-Object Detection and Tracking With Sound by Distilling Multimodal Knowledge](https://openaccess.thecvf.com/content/CVPR2021/html/Valverde_There_Is_More_Than_Meets_the_Eye_Self-Supervised_Multi-Object_Detection_CVPR_2021_paper.html?ref=https://githubhelp.com)
[5] [Enhanced Audio Tagging via Multi- to Single-Modal Teacher-Student Mutual Learning](https://ojs.aaai.org/index.php/AAAI/article/view/17280)
[6] [Knowledge Distillation from Multi-Modality to Single-Modality for Person Verification](https://drive.google.com/file/d/1ISP0ot1WFxZz_IhTAOiWu4nT-Q1bXWtH/view)
[7] [Multimodal Knowledge Expansion](https://openaccess.thecvf.com/content/ICCV2021/html/Xue_Multimodal_Knowledge_Expansion_ICCV_2021_paper.html)
[8] [Distilling Audio-visual Knowledge by Compositional Contrastive Learning](https://openaccess.thecvf.com/content/CVPR2021/papers/Chen_Distilling_Audio-Visual_Knowledge_by_Compositional_Contrastive_Learning_CVPR_2021_paper.pdf)