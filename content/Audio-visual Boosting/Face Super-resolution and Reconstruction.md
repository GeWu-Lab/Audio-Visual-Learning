# Motivation
Voice and face own consistent personality identities. Therefore, it is achievable to estimate important facial attributes such as gender, age as well as ethnicity based on someone's voice. Hence, audio can be the assistance in image processing when the visual information is blurred or missing, like face super-resolution and reconstruction.

# Demo
![face.jpg](content/images/face.jpg)

[Image Source](https://openaccess.thecvf.com/content_CVPR_2020/html/Meishvili_Learning_to_Have_an_Ear_for_Face_Super-Resolution_CVPR_2020_paper.html)


# Overview of the field
- Face super-resolution is the task which aims to recover details of a limited resolution image. Meishvili et al. [1] introduced the audio signal that carries facial attributes to recover a plausible face with higher resolution, where the facial-aware audio embedding is fused with the visual ones.
- In addition, the deepfake attack, which aims to automatically manipulate the face in a video, has been with a broader research interest recently. The face-voice consistency in personality identity provides a solution for defending against this attack. Kong et al. [2] leveraged the joint information of face and voice to reconstruct the authentic face given the fake face as well as the voice signal. 
- Overall, the correlation between voice and face makes it promising to enhance visual information with the aid of audio.


[1] [Learning to Have an Ear for Face Super-Resolution](https://openaccess.thecvf.com/content_CVPR_2020/html/Meishvili_Learning_to_Have_an_Ear_for_Face_Super-Resolution_CVPR_2020_paper.html)
[2] [Appearance Matters, So Does Audio: Revealing the Hidden Face via Cross-Modality Transfer](https://ieeexplore.ieee.org/abstract/document/9349088)