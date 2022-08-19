# Motivation
Cross-modal retrieval in the audio-visual scenario is another typical cross-modal perception task. Its purpose is to retrieve data of one modality based on the query of another, which has been a rapid development research area in these years.


# Demo
![retrevial.mp4](content/videos/retrevial.mp4)

[Video Source](https://www.youtube.com/watch?v=ZyINqDMo3Fg)

# Overview of the field
- Essentially, semantic associations build the bridge between modalities. Even though, the heterogeneous forms of audio-visual modalities make it necessary to map their representations into the same space, where the distance of data pairs reflects the semantic similarity.
- Variants of Canonical Correlation Analysis (CCA) are broadly utilized in the cross-modal retrieval task. They aim to find transformations of two modalities via maximizing the pairwise correlation including Kernel-CCA [1], Deep-CCA [2] and Cluster-CCA [3]. 
- Besides CCA-based methods, some researchers introduced other constraints to train the audio-visual model with a joint embedding space. Suris et al. [4] utilized both the cosine similarity loss and classification loss to project the uni-modal features into the common feature space.
- Hong et al. [5] used the ranking loss between modalities to improve the semantic similarity of video-music pairs. Instead, Hu et al. [6] proposed to build the correlation between image and music, with the assistance of text.
- These retrieval methods has been applied many cross-modal perception tasks, including music recommendation given video [5,7] and dance generation [8].


[1] [Kernel and Nonlinear Canonical Correlation Analysis](https://pubmed.ncbi.nlm.nih.gov/11195936/)
[2] [Deep Canonical Correlation Analysis](https://proceedings.mlr.press/v28/andrew13.html)
[3] [Cluster Canonical Correlation Analysis](http://proceedings.mlr.press/v33/rasiwasia14.pdf)
[4] [Cross-modal Embeddings for Video and Audio Retrieval](https://openaccess.thecvf.com/content_eccv_2018_workshops/w24/html/Suris_Cross-modal_Embeddings_for_Video_and_Audio_Retrieval_ECCVW_2018_paper.html)
[5] [Content-Based Video-Music Retrieval Using Soft Intra-Modal Structure Constraint](https://arxiv.org/abs/1704.06761)
[6] [Image2song: Song Retrieval via Bridging Image Content and Lyric Words](https://openaccess.thecvf.com/content_ICCV_2017/papers/Li_Image2song_Song_Retrieval_ICCV_2017_paper.pdf)
[7] [Audio-Visual Embedding for Cross-Modal Music Video Retrieval through Supervised Deep CCA](https://ieeexplore.ieee.org/abstract/document/8603275/)
[8] [Example-Based Automatic Music-Driven Conventional Dance Motion Synthesis](https://ieeexplore.ieee.org/document/5753889)