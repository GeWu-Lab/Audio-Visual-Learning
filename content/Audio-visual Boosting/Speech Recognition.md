# Motivation 
Speech recognition task aims to translate audio information into format text. The audio quality is sensitive to the channel, environment and speech style in practice, making speech recognition performance degrade greatly. To further obtain the robust model, researchers are inspired by human speech perception that relies on both audio and visual to decide what is being said, especially in noisy scenarios. Concretely, the movement of the speech-related face region is often synchronized with the corresponding audio temporally. Meanwhile, the revealed speech content of audio and face, especially lips, is also highly consistent. Thus, stable visual information in various acoustical environments is introduced to build a more robust speech recognition system.

# Demo
![speech.mp4](content/videos/speech.mp4)

[Video Source](https://www.youtube.com/watch?v=nGZN1UzKUVs)

# Overview of the field
- In early studies, the visual features are extracted by prior lip-shape representation frameworks [1,2] or some low-level visual algorithms [3]. Hidden Markov model-related methods are generally utilized in the modelling of audio-visual synchrony state over time [4,5,6]. 
- Subsequently, the rising neural networks are utilized to extract features [7], since the hand-crafted features either require fine labelling or are vulnerable to factors such as illumination. What's more, the sequential information of videos can be better modelled via Recurrent Neural Networks [8,9]. 
- In these years, the transformer-based recognition framework is introduced to further build context dependence as well as cross-modal association [10,11,12]. 
- These novel model architectures bring the ability of audio-visual speech recognition to a new peak, while the dependence of deep learning methods on large-scale available data, makes the cost of labelling a huge burden. Hence, Shi et al. [13] attempted to build the audio-visual speech recognition model with unlabeled data via the clustering algorithm. 
- Generally, after introducing the visual modality, the speech recognition methods have evolved considerably in performance.


[1] [Visual Speech Recognition Using Active Shape Models and Hidden Markov Models](https://ieeexplore.ieee.org/document/543246)
[2] [Audiovisual Speech Processing](https://www.cambridge.org/core/books/audiovisual-speech-processing/EFC6432E42C4CD096F899D3F93AEE628)
[3] [A Comparison of Model and Transform-based Visual Features for Audio-visual LVCSR](https://ieeexplore.ieee.org/document/1237849)
[4] [Audio-visual Speech Modeling for Continuous Speech Recognition](https://ieeexplore.ieee.org/document/865479/)
[5] [Dynamic Bayesian Networks for Audio-visual Speech Recognition](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.94.7441&rep=rep1&type=pdf)
[6] [Dynamic Modality Weighting for Multi-stream hmms in Audio-visual Speech Recognition](https://dl.acm.org/doi/10.1145/1452392.1452442)
[7] [Audio-visual Speech Recognition Using Deep Learning](https://link.springer.com/article/10.1007/s10489-014-0629-7)
[8] [End-To-End Audiovisual Fusion With LSTMs](https://arxiv.org/abs/1709.04343)
[9] [Temporal Multimodal Learning in Audiovisual Speech Recognition](https://openaccess.thecvf.com/content_cvpr_2016/papers/Hu_Temporal_Multimodal_Learning_CVPR_2016_paper.pdf)
[10] [Deep Audio-visual Speech Recognition](https://ieeexplore.ieee.org/abstract/document/8585066)
[11] [Explicit Sparse Transformer: Concentrated Attention Through Explicit Selection](https://arxiv.org/abs/1912.11637)
[12] [Multimodal Sparse Transformer Network for Audio-V\visual Speech Recognition](https://ieeexplore.ieee.org/abstract/document/9755926)
[13] [Robust Self-Supervised Audio-V\visual Speech Recognition](https://arxiv.org/abs/2201.01763)