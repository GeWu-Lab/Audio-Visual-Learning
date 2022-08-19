# Motivation
Apart from the spatial sound generation based on visual input, it is feasible to use spatial sound to estimate the spatial information of visual scene, especially in low-light or no-light conditions. The spatial consistency between audio and visual modalities makes this task achievable. 


# Demo
![depth.jpg](content/images/depth.jpg)

[Image Source](https://link.springer.com/chapter/10.1007/978-3-030-58545-7_38)

# Overview of the field
- Christensen et al. [1] proposed the BatVision system that predicts depth maps purely based on binaural echo information. Meanwhile, Gao et al. [2] offered a new training fashion that interacts with the environment in an audio-visual way. They fused the monocular image features and binaural echo features to improve the depth estimation quality. 
- Beyond simply fusing audio-visual features, Parida et al. [3] explicitly took the material properties of various objects within a scene into consideration, significantly enhancing the depth estimation performance. 
- The above methods tend to use a single audio feature, typically spectrogram, and other audio features are seldom been paid attention to. Hence, Irie et al. [4] introduced angular spectrum, which is useful in geometric prediction tasks, achieving impressive estimation results. 
- Overall, audio-visual depth estimation is a developing field that promises to expand into more realistic scenarios of application.


[1] [BatVision: Learning to See 3D Spatial Layout with Two Ears](https://ieeexplore.ieee.org/abstract/document/9196934/)
[2] [VISUALECHOES: Spatial Image Representation Learning Through Echolocation](https://link.springer.com/chapter/10.1007/978-3-030-58545-7_38)
[3] [Beyond Image to Depth: Improving Depth Prediction Using Echoes](https://openaccess.thecvf.com/content/CVPR2021/html/Parida_Beyond_Image_to_Depth_Improving_Depth_Prediction_Using_Echoes_CVPR_2021_paper.html)
[4] [Co-Attention-Guided Bilinear Model for Echo-Based Depth Estimation](https://ieeexplore.ieee.org/abstract/document/9746476/)