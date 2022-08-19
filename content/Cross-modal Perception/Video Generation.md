# Motivation
Besides video-to-sound generation, sound-to-video generation is also a research field with much attention, which contains speech-based cases and music-based cases.


# Demo
![talking_ge.mp4](content/videos/talking_ge.mp4)

[Video Source](https://www.youtube.com/watch?v=lNQQHIggnUg)

![gesture_ge.mp4](content/videos/gesture_ge.mp4)

[Video Source](https://www.youtube.com/watch?v=tQLVyTVtsSU)

![dance_ge.mp4](content/videos/dance_ge.mp4)

[Video Source](https://www.youtube.com/watch?v=VrVsAcgFK_4&t=27s)

# Overview of the field
## Speech scene
- The speech-based generation mainly includes talking face/head generation and gesture generation. The former task aims to produce determined videos based on the input speech, and the latter focuses on predicting plausible content-related gestures. 
- The early talking face generation methods are speaker-dependent and rely on a large video corpus of the target person [1,2]. For example, Suwajanakorn et al. [1] proposed to generate the talking image via retrieving the appropriate lip region in the video footage of the target person. 
- Subsequently, speaker-independent face generation methods in an audio-driven manner are presented [3,4,5]. 
- These methods only focus on the generation of face or lip region, while when a person is speaking, other parts (e.g., facial expression and head pose) besides lips are also variable. Hence, researchers introduced structural information, such as landmark [7,8,9] and 3D model [10,11,12], to model the correlation between speech and more general facial parts. 
- Zhou et al. [13] further proposed an implicit low-dimension pose code to generate the pose-controllable talking face without the assistance of structural information. Such strategy could avoid the performance degradation caused by inaccuracy estimated structural representation. 
- Recently, the emotion information is disentangled from the speech to drive more fine-grained talking face generation [14].
- Talking alongside gestures is common for humans, which is helpful to emphasize specific information during communication. The alignment between gesture and speech is implicit and ambiguous, bringing difficulty to its modelling. 
- In the early stage, the gesture generation methods are mostly rule-based, resulting in the produced gesture being limited to a selected discrete set [15,16]. With the advance of deep learning, more methods begin to use the data-driven scheme to fully model the speech-gesture alignment pattern of different speakers, utilizing 2D [17,18] or 3D pose model [19,20]. 
- The early methods formulated this task as a classification problem [21], while more recent works consider it as the regression problem to generate continuous gesture [22,23]~\cite{alexanderson2020style,kucherenko2020gesticulator}. 
- Since each speaker often owns a specific speech-gesture alignment style, Ginosar et al. [17] proposed to model this speaker-specific style during generation. Ahuja et al. [24] further transferred the learnt style of one speaker to another via disentangling the style and content of gestures. 
- Recently, Liang [18] et al. decoupled speech information into semantic-relevant cues and semantic-irrelevant cues to explicitly learn and produce semantic-aware gestures. 

## Music scene
- Dancing to music is another sound-to-video generation scenario. The exploration of the alignment between dance and music characteristics (e.g., beat, rhythm and tempo) has attracted much attention for a long time. 
- The early works of dance generation tackle this task as a retrieval problem that mainly consider the motion-music similarity, limiting the diversity of dance [25,26,27]. 
- Later, models, like LSTM, were widely used to predict motion and pose given a music [28]. Recently, the dance generation task has been formulated from a generative perspective and achieved promising performance [29,30,31]. For example, Lee et al. [29] adopted the decomposition-to-composition learning framework to temporally align and synthesize dance with accompanying music. 
- Further, Huang et al. [32] took the music genre into consideration, beyond the alignment in terms of beat and rhythm. 
- Besides dancing to music, Shlizerman et al. [33] focused on the scenario of playing instruments. They proposed to generate plausible motion of playing given music. 
- Apart from these video generation tasks spanning various scenarios, several related methods are also proposed to manipulate the image content according to audio information [34,35]. 
- In a nutshell, the sound-to-video generation has produced many extraordinary works, which have the potential to facilitate a wide range of applications in practice. 


[1] [Realistic Facial Expression Synthesis for an Image-based Talking Head](https://ieeexplore.ieee.org/document/6011835)
[2] [Synthesizing Obama: learning lip sync from audio](https://dl.acm.org/doi/abs/10.1145/3072959.3073640)
[3] [Lip Movements Generation at a Glance](https://openaccess.thecvf.com/content_ECCV_2018/html/Lele_Chen_Lip_Movements_Generation_ECCV_2018_paper.html)
[4] [You Said That?: Synthesising Talking Faces from Audio](https://link.springer.com/article/10.1007/s11263-019-01150-y)
[5] [Realistic Speech-Driven Facial Animation with GANs](https://link.springer.com/article/10.1007/s11263-019-01251-8)
[6] [GANimation: One-Shot Anatomically Consistent Facial Animation](https://link.springer.com/article/10.1007/s11263-019-01210-3)
[7] [Few-Shot Adversarial Learning of Realistic Neural Talking Head Models](https://openaccess.thecvf.com/content_ICCV_2019/html/Zakharov_Few-Shot_Adversarial_Learning_of_Realistic_Neural_Talking_Head_Models_ICCV_2019_paper.html)
[8] [Makelttalk: Speaker-Aware Talking-Head Animation](https://dl.acm.org/doi/abs/10.1145/3414685.3417774)
[9] [FReeNet: Multi-Identity Face Reenactment](https://openaccess.thecvf.com/content_CVPR_2020/html/Zhang_FReeNet_Multi-Identity_Face_Reenactment_CVPR_2020_paper.html)
[10] [Neural Voice Puppetry: Audio-driven Facial Reenactment](https://justusthies.github.io/posts/neural-voice-puppetry/)
[11] [Rotate-and-Render: Unsupervised Photorealistic Face Rotation from Single-View Images](https://arxiv.org/abs/2003.08124)
[12] [Write-a-speaker: Text-based Emotional and Rhythmic Talking-head Generation](https://ojs.aaai.org/index.php/AAAI/article/view/16286)
[13] [Pose-Controllable Talking Face Generation by Implicitly Modularized Audio-Visual Representation](https://openaccess.thecvf.com/content/CVPR2021/html/Zhou_Pose-Controllable_Talking_Face_Generation_by_Implicitly_Modularized_Audio-Visual_Representation_CVPR_2021_paper.html)
[14] [Audio-Driven Emotional Video Portraits](https://openaccess.thecvf.com/content/CVPR2021/html/Ji_Audio-Driven_Emotional_Video_Portraits_CVPR_2021_paper.html)
[15] [BEAT: the Behavior Expression Animation Toolkit](https://link.springer.com/chapter/10.1007/978-3-662-08373-4_8)
[16] [Robot behavior toolkit: Generating effective social behaviors for robots](https://ieeexplore.ieee.org/document/6249556/)
[17] [Learning Individual Styles of Conversational Gesture](https://openaccess.thecvf.com/content_CVPR_2019/html/Ginosar_Learning_Individual_Styles_of_Conversational_Gesture_CVPR_2019_paper.html)
[18] [SEEG: Semantic Energized Co-Speech Gesture Generation](https://openaccess.thecvf.com/content/CVPR2022/html/Liang_SEEG_Semantic_Energized_Co-Speech_Gesture_Generation_CVPR_2022_paper.html)
[19] [Analyzing Input and Output Representations for Speech-Driven Gesture Generation](https://dl.acm.org/doi/abs/10.1145/3308532.3329472)
[20] [Evaluation of Speech-to-Gesture Generation Using Bi-Directional LSTM Network](https://dl.acm.org/doi/abs/10.1145/3267851.3267878)
[21] [To React or not to React: End-to-End Visual Pose Forecasting for Personalized Avatar during Dyadic Conversations](https://dl.acm.org/doi/abs/10.1145/3340555.3353725)
[22] [Style-Controllable Speech-Driven Gesture Synthesis Using Normalising Flows](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.13946)
[23] [Gesticulator: A Framework For Semantically-Aware Speech-Driven Gesture Generation](https://dl.acm.org/doi/abs/10.1145/3382507.3418815)
[24] [Style Transfer for Co-Speech Gesture Animation: A Multi-Speaker Conditional-Mixture Approach](https://arxiv.org/abs/2007.12553)
[25] [Example-Based Automatic Music-Driven Conventional Dance Motion Synthesis](https://ieeexplore.ieee.org/document/5753889)
[26] [Learn2dance: Learning Statistical Music-to-dance Mappings for Choreography Synthesis](http://home.ku.edu.tr/~yyemez/IEEETrMultimedia12.pdf)
[27] [Music Similarity-based Approach to Generating Dance Motion Sequence](https://link.springer.com/article/10.1007/s11042-012-1288-5)
[28] [Dance with Melody: An LSTM-autoencoder Approach to Music-oriented Dance Synthesis](https://dl.acm.org/doi/abs/10.1145/3240508.3240526)
[29] [Dancing to Music](https://proceedings.neurips.cc/paper/2019/hash/7ca57a9f85a19a6e4b9a248c1daca185-Abstract.html)
[30] [Dance Revolution: Long-Term Dance Generation with Music via Curriculum Learning](https://arxiv.org/abs/2006.06119)
[31] [AI Choreographer: Music Conditioned 3D Dance Generation With AIST++](https://openaccess.thecvf.com/content/ICCV2021/html/Li_AI_Choreographer_Music_Conditioned_3D_Dance_Generation_With_AIST_ICCV_2021_paper.html)
[32] [Genre-Conditioned Long-Term 3D Dance Generation Driven by Music](https://ieeexplore.ieee.org/abstract/document/9747838/)
[33] [Audio to Body Dynamics](https://openaccess.thecvf.com/content_cvpr_2018/html/Shlizerman_Audio_to_Body_CVPR_2018_paper.html)
[34] [Sound-guided Semantic Image Manipulation](https://openaccess.thecvf.com/content/CVPR2022/papers/Lee_Sound-Guided_Semantic_Image_Manipulation_CVPR_2022_paper.pdf)
[35] [Learning Visual Styles from Audio-Visual Associations](https://arxiv.org/abs/2205.05072)
