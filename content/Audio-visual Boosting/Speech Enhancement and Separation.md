# Motivation
Speech enhancement and separation are two tightly related tasks, which aim to recover clean target speech from a mixture of sound (e.g.  overlapped speech of multiple speakers or speech with background noise). In the beginning, these tasks take the audio signal as the input only, making them sensitive to the acoustic noise. As stated above, human speech perception relies on both sight and hearing. The motion of lips, tongue, as well as facial expressions, also reveal related semantics information. Meanwhile, visual information is often unaffected by acoustic noise and multiple speakers are visually isolated. Hence, the visual modality is brought into speech enhancement and separation tasks for generating high-quality audio.

# Demo
![speech_separation.mp4](content/videos/speech_separation.mp4)

[Video Source](https://www.youtube.com/watch?v=rVQVAPiJWKU)

# Overview of the field
- In the infancy of these studies, the knowledge-based methods and classical statistical approaches are proposed, including non-negative matrix factorization [1], mutual information [2], HMMs [3] and visually-derived Wiener filter [4]. 
- Later, the deep audio-visual models have demonstrated impressive performance on reconstructing clean speech signal with different forms (e.g., waveform [5] and spectrogram [6]) with the assistance of lip movement [7,8], face clips [9,10,11] and even static face image [12]. 
- Overall, the introducing of visual information strengthens the ability of speech enhancement and separation models by providing auxiliary information. 


[1] [Single-Channel Speech Separation using Sparse Non-Negative Matrix Factorization](http://mikkelschmidt.dk/papers/schmidt2006interspeech.pdf)
[2] [Learning Joint Statistical Models for Audio-Visual Fusion and Segregation](https://people.eecs.berkeley.edu/~trevor/papers/fishernips00.pdf)
[3] [Audio-Visual Sound Separation Via Hidden Markov Models](https://papers.nips.cc/paper/2001/hash/d47268e9db2e9aa3827bba3afb7ff94a-Abstract.html) 
[4] [Visually-Derived Wiener Filters for Speech Enhancement](https://ieeexplore.ieee.org/document/4218168)
[5] [Visually Assisted Time-Domain Speech Enhancement](https://ieeexplore.ieee.org/abstract/document/8969244)
[6] [Audio-Visual Speech Enhancement Using Multimodal Deep Convolutional Neural Networks](https://ieeexplore.ieee.org/abstract/document/8323326)
[7] [Visual Speech Enhancement](https://arxiv.org/abs/1711.08789)
[8] [The Conversation: Deep Audio-Visual Speech Enhancement](https://arxiv.org/abs/1804.04121)
[9] [Seeing Through Noise: Visually Driven Speaker Separation And Enhancement](https://ieeexplore.ieee.org/abstract/document/8462527)
[10] [Multimodal SpeakerBeam: Single Channel Target Speech Extraction with Audio-Visual Speaker Clues](https://www.isca-speech.org/archive_v0/Interspeech_2019/pdfs/1513.pdf)
[11] [Looking Into Your Speech: Learning Cross-Modal Affinity for Audio-Visual Speech Separation](https://openaccess.thecvf.com/content/CVPR2021/html/Lee_Looking_Into_Your_Speech_Learning_Cross-Modal_Affinity_for_Audio-Visual_Speech_CVPR_2021_paper.html?ref=https://githubhelp.com)
[12] [Facefilter: Audio-Visual Speech Separation Using Still Images](https://arxiv.org/abs/2005.07074)