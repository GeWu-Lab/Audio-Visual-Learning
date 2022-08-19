# Motivation
Speaker recognition is a series of tasks that pay attention to the identity of speaker, including speaker verification, identification and diarization. Speaker verification aims to verify whether an utterance is pronounced by a target speaker and speaker identification aims to determine speaker identity for an utterance. Speaker diarization answers the question ''who spoke when''. Audio and facial information are two important personal identities and speaker recognition methods with one of which have been a mature field. But these uni-modal methods are vulnerable to the variants of environments. The acoustic characteristics of audio are susceptible to many factors including background noise and the speaker's mood, while the facial information is sensitive to pose, illumination, and device. Therefore, the combination of multiple modalities is essential for building a more robust model, considering personal identities are semantically consistent in both audio and visual.


# Demo
![diarization.mp4](content/videos/diarization.mp4)
![diarization.jpg](content/images/diarization.jpg)

[Video Source](https://team.inria.fr/robotlearn/research/avdiarization/)


# Overview of the field
- In the early studies of speaker verification and identification, researchers often utilized hand-crafted features and conducted decision fusion to combine audio expert and visual expert [1,2,3,4]. 
- As deep learning develops by leaps and bounds, the uni-modal features tend to be extracted by neural networks and more feature-level fusion methods emerge, like concatenation [5] and attention mechanism [6,7], besides decision fusion [5,8]. 
- Compared with speaker verification and identification, the speaker diarization task needs to further split the given speech into speaker-homogeneous segments. After introducing visual modality, studies of diarization include two paths. 
- One path is to enhance diarization performance via fusing uni-modal results [9,10]. 
- Another path extends the diarization task into ''who spoken when and from where'' that further localizes the speech-related region in visual [11,12]. 
- In recent years, the requirement for numerous data of deep learning has resulted in the burden of collecting as well as labelling diarization datasets. Thus, the nature of audio-visual synchronization is further utilized to design the self-supervised audio-visual diarization method [13]. 
- Overall, audio-visual speaker recognition achieves impressive results with information from multiple views.


[1] [Fusion of Face and Speech Data for Person Identity Verification](https://ieeexplore.ieee.org/document/788647)
[2] [Multimodal Person Recognition Using Unconstrained Audio and Video](http://alumni.media.mit.edu/~tanzeem/choudhury_avbpa99.pdf)
[3] [Multi-level Fusion of Audio and Visual Features for Speaker Identification](https://link.springer.com/chapter/10.1007/11608288_66)
[4] [Audiovisual Celebrity Recognition in Unconstrained Web Videos](https://ieeexplore.ieee.org/document/4959999)
[5] [A Multi-View Approach to Audio-visual Speaker Verification](https://ieeexplore.ieee.org/abstract/document/9414260)
[6] [Noise-tolerant Audio-visual Online Person Verification Using an Attention-based Neural Network Fusion](https://ieeexplore.ieee.org/abstract/document/8683477)
[7] [Audio-visual Deep Neural Network for Robust Person Verification](https://ieeexplore.ieee.org/abstract/document/9350195)
[8] [Audio-visual Person Recognition in Multimedia Data From the Iarpa Janus Program](https://ieeexplore.ieee.org/abstract/document/8462122)
[9] [Audio-visual Speaker Diarization Using Fisher Linear Semi-discriminant Analysis](https://link.springer.com/article/10.1007/s11042-014-2274-x)
[10] [Multimodal Speaker Diarization](https://ieeexplore.ieee.org/abstract/document/5728824)
[11] [Audio Segmentation and Speaker Localization in Meeting Videos](https://ieeexplore.ieee.org/document/1699413)
[12] [Who Said That?: Audio-visual Speaker Diarisation Of Real-World Meetings](https://arxiv.org/abs/1906.10042)
[13] [Self-Supervised Learning for Audio-visual Speaker Diarization](https://ieeexplore.ieee.org/abstract/document/9054376)