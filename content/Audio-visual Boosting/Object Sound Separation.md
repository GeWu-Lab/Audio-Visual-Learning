# Motivation
Similar to the face-voice association in the speech situation, scenarios where simultaneously exist multiple sounding objects, are common in our daily life. Object sound separation aims to isolate the sound produced by the specific object from the mixture.


# Demo
![sound_separation.mp4](content/videos/sound_separation.mp4)

[Video Source](https://www.youtube.com/watch?v=m6fo2A7qGQM)

# Overview of the field
- Since the visual objects in the same semantic category usually produce similar sound pattern, researchers proposed to introduce the static visual appearance of object to split its audio signal from the mixed ones of different categories objects [1,2]. 
- However, these methods cannot well handle the scenarios that sounding objects are with the same category, since the objects appearance are visually similar. Thus, the motion information, like the trajectory cues [3] and keypoint-based structural representation [4] is introduced, by further considering the temporal and spatial consistency between audio and visual modalities.
- To better build the audio-visual mapping, most methods above employ the strategy that mixes existing audio-visual segments, then learns to reconstruct each of them, to train the model. Although they have achieved significant results, the acoustic properties as well as visual environment information of real multi-source videos are practically neglected in the synthetic ones. Hence, Gao et al. [5] proposed the co-separation training paradigm that learns object-level audio-visual correlation in realistic multi-source videos.
- Recently, considering the same object may produce diverse sounds, Chatterjee et al. [6] formulated the visual scene as a graph, then modelled the characteristics of different interactions for the same object. 
- In general, sound separation has gradually evolved in many aspects, including the difficulty degree of separation and training paradigm.


[1] [Learning to Separate Object Sounds by Watching Unlabeled Video](https://openaccess.thecvf.com/content_ECCV_2018/html/Ruohan_Gao_Learning_to_Separate_ECCV_2018_paper.html)
[2] [The Sound of Pixels](https://openaccess.thecvf.com/content_ECCV_2018/html/Hang_Zhao_The_Sound_of_ECCV_2018_paper.html)
[3] [The Sound of Motions](https://openaccess.thecvf.com/content_ICCV_2019/html/Zhao_The_Sound_of_Motions_ICCV_2019_paper.html)
[4] [Music Gesture for Visual Sound Separation](https://openaccess.thecvf.com/content_CVPR_2020/html/Gan_Music_Gesture_for_Visual_Sound_Separation_CVPR_2020_paper.html)
[6] [Recursive Visual Sound Separation Using Minus-Plus Net](https://openaccess.thecvf.com/content_ICCV_2019/html/Xu_Recursive_Visual_Sound_Separation_Using_Minus-Plus_Net_ICCV_2019_paper.html)
[5] [Co-Separating Sounds of Visual Objects](https://openaccess.thecvf.com/content_ICCV_2019/html/Gao_Co-Separating_Sounds_of_Visual_Objects_ICCV_2019_paper.html)
[6] [Visual Scene Graphs for Audio Source Separation](https://openaccess.thecvf.com/content/ICCV2021/html/Chatterjee_Visual_Scene_Graphs_for_Audio_Source_Separation_ICCV_2021_paper.html)
