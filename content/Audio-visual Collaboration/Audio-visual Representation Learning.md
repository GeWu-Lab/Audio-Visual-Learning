# Motivation
How to effectively extract representation from heterogeneous audio-visual modalities without human annotations, is an important topic. This is because that high-quality representation can contribute to a variety of downstream tasks. For audio-visual data, the consistencies across semantic, spatial as well as temporal between them, naturally provide supervision for representation learning. Not always but often, the visual and accompanying sound is synced in temporal and semantically consistent. Meanwhile, the spatial location in stereo scenarios is also consistent. These consistencies provide ideal supervision for audio-visual representation learning.


# Demo

![representation.jpg](content/images/representation.jpg)

[Image Source](https://proceedings.neurips.cc/paper/2020/hash/328e5d4c166bb340b314d457a208dc83-Abstract.html)




# Overview of the field
- In the early stage, de Sa et al. [1] proposed to minimize the audio-visual disagreement to learn from unlabelled data.
- Arandjelovic et al. [2] employed the semantic consistency and proposed the Audio-Visual Correspondence (AVC) learning framework whose goal is to determine whether the audio input and visual input are from the same video or not. Korbar et al. [3] further proposed the Audio-Visual Temporal Synchronization, which aims to decide whether a given audio input and a visual input are either in-sync or out-of-sync, considering the more strict audio-visual consistency in temporal. Besides, Morgado et al. [4] leveraged the spatial consistency between $360^{\circ}$ video and spatial audio as supervision to learn audio-visual representation, revealing advantages on a variety of downstream tasks. 
- The above primary methods are simple yet effective, but suffer from the data noise when training with ''in the wild'' videos [5]. Some recent methods further view the false negative pairs and false positive pairs as the noise [5,6]. They proposed to estimate the quality of audio-visual pairs, then optimize with a weighted contrastive learning loss, to alleviate the impact of false pairs.
- Further, to better learn representation in the scenes with multiple sound sources, Deep Multimodal Clustering model is proposed to first disentangle individual sources of each modality, then associate them across modalities [7].
- The learnt representation by these methods shows impressive results in multiple downstream tasks, such as acoustic scene classification and image classification, sometimes even surpassing human performance [3,7].
- The above methods are often performed in a pairwise fashion, which usually lack the modelling of the sample distribution. Therefore, deep clustering techniques are introduced. Alwassel et al. [8] first proposed the Cross-Modal Deep Clustering (XDC) method to learn representation in a self-supervised manner. They trained the audio and visual model alternatively with the cross-modal pseudo label. 
- Compared with the XDC method with single modality clusters, Asnao et al. [9] regarded multiple modalities as different data augmentation forms, then learnt audio-visual clusters to annotate the unlabelled videos. Furthermore, Chen et al. [10] combines the pair-wise contrastive learning scheme and clustering methods to fully capture semantic consistency. These deep audio-visual clustering methods provide another path to learning representation in a self-supervised manner.
- In recent years, with the increase in computation sources and accessible data, pre-training models that use pretext tasks to train on massive data with a large-scale number of parameters have emerged. In the beginning, the pre-training models flourish in the natural language processing field, then inspires the appearance of multi-modal pre-training models. 
- Omni-perception PreTrainer [11] is the first visual-text-audio pre-training model. They designed multi-modal pretext tasks for training at sample-level, token-level and modality-level, covering masked modality modelling, generation and contrastive learning schemes. 
- In the training of VATT [12] and AudioCLIP [13] model, the contrastive learning approach is also utilized to maximize cross-modal similarities. Zellers et al. [14] proposed a new contrastive masked span learning objective. They trained the model by figuring out which span of audio or text is masked out in the video sequence, besides contrastive learning constrain. 
- This pre-training strategy is claimed to enable rapid training as well as powerful generalization ability. The multi-modal pre-training model containing audio-visual modalities is now still in its early stages of development and is promising to greatly advance the generalizability under more scenarios.

[1] [Learning Classification with Unlabeled Data](https://proceedings.neurips.cc/paper/1993/file/e0ec453e28e061cc58ac43f91dc2f3f0-Paper.pdf)
[2] [Look, Listen and Learn](https://openaccess.thecvf.com/content_iccv_2017/html/Arandjelovic_Look_Listen_and_ICCV_2017_paper.html)
[3] [Cooperative Learning of Audio and Video Models from Self-Supervised Synchronization](https://proceedings.neurips.cc/paper/2018/hash/c4616f5a24a66668f11ca4fa80525dc4-Abstract.html)
[4] [Learning Representations from Audio-Visual Spatial Alignment](https://proceedings.neurips.cc/paper/2020/hash/328e5d4c166bb340b314d457a208dc83-Abstract.html)
[5] [Robust Audio-Visual Instance Discrimination](https://openaccess.thecvf.com/content/CVPR2021/html/Morgado_Robust_Audio-Visual_Instance_Discrimination_CVPR_2021_paper.html)
[6] [Audio-Visual Instance Discrimination with Cross-Modal Agreement](https://openaccess.thecvf.com/content/CVPR2021/html/Morgado_Audio-Visual_Instance_Discrimination_with_Cross-Modal_Agreement_CVPR_2021_paper.html)
[7] [Deep Multimodal Clustering for Unsupervised Audiovisual Learning](https://openaccess.thecvf.com/content_CVPR_2019/html/Hu_Deep_Multimodal_Clustering_for_Unsupervised_Audiovisual_Learning_CVPR_2019_paper.html)
[8] [Self-Supervised Learning by Cross-Modal Audio-Video Clustering](https://proceedings.neurips.cc/paper/2020/hash/6f2268bd1d3d3ebaabb04d6b5d099425-Abstract.html)
[9] [Labelling Unlabelled Videos From Scratch With Multi-Modal Self-Supervision](https://proceedings.neurips.cc/paper/2020/hash/31fefc0e570cb3860f2a6d4b38c6490d-Abstract.html)
[10] [Multimodal Clustering Networks for Self-Supervised Learning From Unlabeled Videos](https://openaccess.thecvf.com/content/ICCV2021/html/Chen_Multimodal_Clustering_Networks_for_Self-Supervised_Learning_From_Unlabeled_Videos_ICCV_2021_paper.html)
[11] [OPT: Omni-Perception Pre-Trainer for Cross-Modal Understanding and Generation](https://arxiv.org/abs/2107.00249)
[12] [VATT: Transformers for Multimodal Self-Supervised Learning from Raw Video, Audio and Text](https://proceedings.neurips.cc/paper/2021/hash/cb3213ada48302953cb0f166464ab356-Abstract.html)
[13] [Audioclip: Extending Clip to Image, Text and Audio](https://ieeexplore.ieee.org/abstract/document/9747631/)
[14] [MERLOT Reserve: Neural Script Knowledge Through Vision and Language and Sound](https://openaccess.thecvf.com/content/CVPR2022/html/Zellers_MERLOT_Reserve_Neural_Script_Knowledge_Through_Vision_and_Language_and_CVPR_2022_paper.html)