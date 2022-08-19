# Motivation
The correlation between motion and produced sound provides the possibility to reconstruct the audio signal based on silent videos. The scenes of mono sound generation cover speech reconstruction, music generation as well as natural sound generation. 


# Demo
![speech_ge.mp4](content/videos/speech_ge.mp4)

[Video Source](https://www.youtube.com/watch?v=Xjbn7h7tpg0)

![music_ge.mp4](content/videos/music_ge.mp4)

[Video Source](https://www.youtube.com/watch?v=bo5UzyDB80E)

![natural_ge.mp4](content/videos/natural_ge.mp4)

[Video Source](https://www.youtube.com/watch?v=0FW99AQmMc8)


# Overview of the field
## Speech scene
- Under the speech scenarios, the speech content can be revealed by visual information, including the movement of lips and tongue. This fact inspires the speech reconstruction task which aims to generate the audio signal from silent videos.
- Early studies of this task proposed to estimate the spectral envelope from the hand-crafted visual feature, then the spectral envelope is used to synthetic corresponding audio signal [1,2]. 
- Since it is time-consuming and hard to construct suitable hand-crafted visual features, the subsequent works learnt to extract visual features from raw data [3,4,5]. 
- To avoid the burden of learning audio-related intermediate representation, the Generative Adversarial Networks-based model is proposed to directly synthesize audio waveform from silent videos [6,7]. 
- Moreover, considering video of one single view is hard to capture complete information, multi-view videos (e.g., frontal and profile views) are used to improve generation quality [8,9]. 
## Music scene
- Musical scene is another typical audio-visual scenario. To generate high-quality music, intermediate representations, like musical instrument digital interface, are utilized to bridge the visual changes of playing instruments and generated audio.
- Early studies of music generation focused on relatively simple musical scenes, especially the piano case, using traditional computer vision techniques to capture the changes of instrument [10]. More recently, deep learning-based models, including Variational Autoencoder and GANs, have emerged to capture the playing motion in terms of body keypoints [11,12] and movements [13] in general instrument scenes.
- The above methods aim to produce determined music based on strict audio-visual correspondence, while Di et al. [14] leveraged the rhythmic relations between video and music at the semantic level to generate non-determined background music, matching the given video.
## Natural sound scene
- Further, the sound generation of natural scenes is more challenging since the audio-visual correspondence in realistic scenes is hard to be captured, compared with the limited speech or musical scenes. 
- Owens et al. [15] pioneered the natural sound generation task via collecting the Greatest Hits dataset and presented a model that generates sound based on visual changes of hitting or scratching objects. 
- Subsequently, Zhou et al. [16] employed the SampleRNN model to generate raw waveform samples given the visual appearance and optical flow, covering ambient sounds and sounds of animals or peoples. 
- Chen et al. [17] took the object-irrelevant background sound into consideration, achieving high-quality results. 
- Recently, Iashin et al. [18] presented an efficient visual-driven generation method via a codebook representation that is trained by a variant of GANs. 
- Generally, mono sound generation has been a flourishing field, covering multiple audio-visual scenarios.


[1] [Reconstructing intelligible audio speech from visual speech features](https://www.isca-speech.org/archive_v0/interspeech_2015/papers/i15_3355.pdf)
[2] [Generating Intelligible Audio Speech From Visual Speech](https://ieeexplore.ieee.org/document/7949073/)
[3] [Vid2speech: Speech Reconstruction From Silent Video](https://ieeexplore.ieee.org/abstract/document/7953127)
[4] [Improved Speech Reconstruction From Silent Video](https://openaccess.thecvf.com/content_ICCV_2017_workshops/w8/html/Ephrat_Improved_Speech_Reconstruction_ICCV_2017_paper.html)
[5] Lip2Audspec: Speech Reconstruction from Silent Lip Movements Video](https://ieeexplore.ieee.org/abstract/document/8461856)
[6] [Video-Driven Speech Reconstruction using Generative Adversarial Networks](https://arxiv.org/abs/1906.06301)
[7] [End-to-End Video-to-Speech Synthesis Using Generative Adversarial Networks](https://ieeexplore.ieee.org/abstract/document/9760273)
[8] [Harnessing AI for Speech Reconstruction using Multi-view Silent Video Feed](https://arxiv.org/abs/1807.00619)
[9] [Hush-Hush Speak: Speech Reconstruction Using Silent Videos](https://www.isca-speech.org/archive_v0/Interspeech_2019/pdfs/3269.pdf)
[10] [Real-Time Piano Music Transcription Based on Computer Vision](https://ieeexplore.ieee.org/abstract/document/7225173)
[11] [Foley Music: Learning to Generate Music from Videos](https://link.springer.com/chapter/10.1007/978-3-030-58621-8_44)
[12] [Multi-Instrumentalist Net: Unsupervised Generation of Music from Body Movements](https://arxiv.org/abs/2012.03478)
[13] [Collaborative Learning to Generate Audio-Video Jointly](https://ieeexplore.ieee.org/abstract/document/9413802/)
[14] [Video Background Music Generation with Controllable Music Transformer](https://dl.acm.org/doi/abs/10.1145/3474085.3475195)
[15] [Visually Indicated Sounds](https://openaccess.thecvf.com/content_cvpr_2016/html/Owens_Visually_Indicated_Sounds_CVPR_2016_paper.html)
[16] [Visual to Sound: Generating Natural Sound for Videos in the Wild](https://openaccess.thecvf.com/content_cvpr_2018/html/Zhou_Visual_to_Sound_CVPR_2018_paper.html)
[17] [Generating Visually Aligned Sound From Videos](https://ieeexplore.ieee.org/abstract/document/9151258)
[18] [Taming Visually Guided Sound Generation](https://arxiv.org/abs/2110.08791)