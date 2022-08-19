# Motivation
In the computer vision field, action recognition is a widely studied task, and it aims to discriminate different human activities based on the video. Researchers have employed many visually relevant modalities for action recognition. For example, depth modality owns spatial information and skeleton modality reveals structural information of subject pose. But these modalities are all limited to reflecting visual information although with different emphases. In contrast, the audio modality is promising to serve as complementary information in semantics. Firstly, plenty of action categories company with sound. Secondly, audio can reflect the discriminative information of similar actions in visual. For example, the actions of eatboxing and singing in Kinetics-700. Thirdly, audio can capture the out-of-screen or visually hard to observe actions (e.g.,csniffing). Thus, audio-visual action recognition is introduced to perceive actions with more views.


# Demo
![action.mp4](content/videos/action.mp4)

[Video Source](https://www.youtube.com/watch?v=VzoaKsDvv1o)

# Overview of the field
- Among the audio-visual action recognitoin studies, decision fusion and late fusion are commonly used to combine the audio-visual information [1,2]. 
- More recently, more fine-grained mid-level fusion methods are proposed to fully explore the audio-visual consistency in temporal [3,4]. Kazakos et al. [3] presented the Temporal Binding Network to aggregate RGB, Flow and Audio information temporally at mid-level. 
- In these years, the flourish of transformer has inspired the transformer-based mechanism that both considers self-attention and cross-modal attention [5]. 
- What's more, since videos often contain action-irrelevant segments, resulting in unnecessary computation cost and even possibly interfering with the prediction, audio modality is used to reduce redundancy segments of videos [6,7]. Similarly, the modality selection [8] and dropout [9] strategies are adopted for efficient video recognition. 
- Apart from the above methods that fusing multiple information, some researchers consider the audio modality as the assistance for the domain generalization in visual, alleviating the domain shift problem in action recognition across scenes [10,11,12]. 
- Overall, the introducing of audio enhances the action recognition task from different perspectives, including richer information, more efficient training, and better generalization. 


[1] [Exploring Multimodal Video Representation For Action Recognition](https://ieeexplore.ieee.org/abstract/document/7727435)
[2] [The ActivityNet Large-Scale Activity Recognition Challenge 2018 Summary](https://arxiv.org/abs/1808.03766)
[3] [EPIC-Fusion: Audio-Visual Temporal Binding for Egocentric Action Recognition](https://openaccess.thecvf.com/content_ICCV_2019/html/Kazakos_EPIC-Fusion_Audio-Visual_Temporal_Binding_for_Egocentric_Action_Recognition_ICCV_2019_paper.html)
[4] [Audiovisual SlowFast Networks for Video Recognition](https://arxiv.org/abs/2001.08740)
[5] [MM-ViT: Multi-Modal Video Transformer for Compressed Video Action Recognition](https://openaccess.thecvf.com/content/WACV2022/html/Chen_MM-ViT_Multi-Modal_Video_Transformer_for_Compressed_Video_Action_Recognition_WACV_2022_paper.html)
[6] [SCSampler: Sampling Salient Clips From Video for Efficient Action Recognition](https://openaccess.thecvf.com/content_ICCV_2019/html/Korbar_SCSampler_Sampling_Salient_Clips_From_Video_for_Efficient_Action_Recognition_ICCV_2019_paper.html)
[7] [Listen to Look: Action Recognition by Previewing Audio](https://openaccess.thecvf.com/content_CVPR_2020/html/Gao_Listen_to_Look_Action_Recognition_by_Previewing_Audio_CVPR_2020_paper.html)
[8] [AdaMML: Adaptive Multi-Modal Learning for Efficient Video Recognition](https://openaccess.thecvf.com/content/ICCV2021/html/Panda_AdaMML_Adaptive_Multi-Modal_Learning_for_Efficient_Video_Recognition_ICCV_2021_paper.html)
[9] [Learnable Irrelevant Modality Dropout for Multimodal Action Recognition on Modality-Specific Annotated Videos](https://openaccess.thecvf.com/content/CVPR2022/html/Alfasly_Learnable_Irrelevant_Modality_Dropout_for_Multimodal_Action_Recognition_on_Modality-Specific_CVPR_2022_paper.html)
[10] [Cross-Domain First Person Audio-Visual Action Recognition through Relative Norm Alignment](https://arxiv.org/abs/2106.01689)
[11] [Domain Generalization Through Audio-Visual Relative Norm Alignment in First Person Action Recognition](https://openaccess.thecvf.com/content/WACV2022/html/Planamente_Domain_Generalization_Through_Audio-Visual_Relative_Norm_Alignment_in_First_Person_WACV_2022_paper.html)
[12] [Audio-Adaptive Activity Recognition Across Video Domains](https://openaccess.thecvf.com/content/CVPR2022/html/Zhang_Audio-Adaptive_Activity_Recognition_Across_Video_Domains_CVPR_2022_paper.html)