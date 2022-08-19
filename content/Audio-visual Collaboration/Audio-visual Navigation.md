# Motivation
Besides localizing objects in recorded videos, localizing and navigating in spatial space is natural for humans. In embodied artificial intelligence field, navigation is a vital topic and visual clues are the main information source. However, for humans, hearing can also provide useful spatial information for our exploration of an unfamiliar environment. Thus, the audio-visual navigation task is introduced, aiming to search and locate the target sounding goal in a complex 3D environment.


# Demo
![navigation.mp4](content/videos/navigation.mp4)

[Video Source](https://www.youtube.com/watch?v=4uiptTUyq30)

# Overview of the field
- Chen et al. [1] adopted an end-to-end multi-modal deep reinforcement learning method to explore navigation policies with a stream of audio-visual observations. Concurrently, Gan et al. [2] designed a planner for the action sequence generation, based on the captured spatial memory and observed audio-visual information. 
- To further improve the efficiency of navigation, Chen et al. [3] proposed to set a series of waypoints in a hierarchical model, then a planner plays the path to each waypoint. 
- These prior works assume the sounding goal constantly produces a steady repeating sound. Differently, Chen et al. [4] introduced the semantic audio-visual navigation task that the produced sound of the sounding goal is semantically consistent with the scene (e.g., water dripping in the bathroom).
- The above works often navigate in the environment with a single static sounding goal. Thus, researchers attempted to navigate in more complex scenarios with moving and distracting sounds [5,6]. 
- Relatively, Majumder et al. [7] proposed to train the agent for separating the target source in the 3D environment via moving around based on audio-visual observations. 
- In general, existing audio-visual navigation studies have worked well in the simple simulation 3D environment, but are still a subset of human navigation scenarios, and more realistic cases are under-solved.


[1] [SoundSpaces: Audio-Visual Navigation in 3D Environments](https://link.springer.com/chapter/10.1007/978-3-030-58539-6_2)
[2] [Look, Listen, and Act: Towards Audio-Visual Embodied Navigation](https://ieeexplore.ieee.org/abstract/document/9197008)
[3] [Learning to Set Waypoints for Audio-Visual Navigation](https://arxiv.org/abs/2008.09622)
[4] [Semantic Audio-Visual Navigation](https://openaccess.thecvf.com/content/CVPR2021/html/Chen_Semantic_Audio-Visual_Navigation_CVPR_2021_paper.html)
[5] [Catch Me If You Hear Me: Audio-Visual Navigation in Complex Unmapped Environments with Moving Sounds](https://arxiv.org/abs/2111.14843)
[6] [Sound Adversarial Audio-Visual Navigation](https://arxiv.org/abs/2202.10910)
[7] [Move2Hear: Active Audio-Visual Source Separation](https://openaccess.thecvf.com/content/ICCV2021/html/Majumder_Move2Hear_Active_Audio-Visual_Source_Separation_ICCV_2021_paper.html)
