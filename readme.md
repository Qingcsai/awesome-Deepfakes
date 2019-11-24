# Deepfakes相关资料整理

## 1 Deepfakes社会性发展调研报告

* 荷兰初创公司Deeptrace发布两个年度（2018年和2019年）[Deepfakes发展状况调研报告](https://github.com/Qingcsai/Deepfakes-Zoo/tree/master/the-state-of-deepfakes)

## 2 Deepfake Creation

### 2.1 Face-swapping methods

* [Deepfakes](https://github.com/deepfakes/faceswap)
* [Faceswap-GAN](https://github.com/shaoanlu/faceswap-GAN)
* [FaceSwap](https://github.com/MarekKowalski/FaceSwap)
* [On Face Segmentation, Face Swapping, and Face Perception](https://ieeexplore.ieee.org/abstract/document/8373817/)
* [Fast Face-swap Using CNN](http://openaccess.thecvf.com/content_iccv_2017/html/Korshunova_Fast_Face-Swap_Using_ICCV_2017_paper.html)
* [FSGAN](http://openaccess.thecvf.com/content_ICCV_2019/papers/Nirkin_FSGAN_Subject_Agnostic_Face_Swapping_and_Reenactment_ICCV_2019_paper.pdf)
* [DeepFaceLab](https://github.com/iperov/DeepFaceLab)
* [DFaker](https://github.com/dfaker/df)
* [DeepFake-tf](https://github.com/StromWine/DeepFake_tf)

### 2.2 Face reenactment methods

* 2014 ICPR [Face Anti-spoofing Based on General Image Quality Assessment](https://ieeexplore.ieee.org/abstract/document/6976921)
* 2015 TIFS [Face spoof detection with image distortion analysis.](https://ieeexplore.ieee.org/abstract/document/7031384)
* 2016 CVPR [face2face](http://openaccess.thecvf.com/content_cvpr_2016/html/Thies_Face2Face_Real-Time_Face_CVPR_2016_paper.html)
* 2018 [HeadOn](http://niessnerlab.org/papers/2018/7headon/headon_preprint.pdf)
* 2017 CVPR [Lip reading sentences in the wild](https://ieeexplore.ieee.org/abstract/document/8099850)
* 2017 TOG [Synthesizing Obama](https://dl.acm.org/citation.cfm?id=3073640)
* 2017 TOG [*Bringing portraits to life*](https://dl.acm.org/citation.cfm?id=3130818)
* 2018 EUSIPCO [Speaker inconsistency detection in tampered video](https://ieeexplore.ieee.org/abstract/document/8553270)
* 2018 TOG [Deep video portraits](https://dl.acm.org/citation.cfm?id=3201283)
* 2018 [Generative Adversarial Talking Head](https://arxiv.org/abs/1803.07716)
* 2019 [Few-Shot Adversarial Learning of Realistic Neural Talking Head Models](https://arxiv.org/abs/1905.08233https://arxiv.org/abs/1905.08233)
* 2019 [NeuralTexture](https://arxiv.org/abs/1904.12356)
* 2019 AAAI Oral MMLAB-CUHK [Talking Face Generation by Adversarially Disentangled Audio-Visual Representation](https://arxiv.org/abs/1807.07860)

### 3 Deepfake Detection

#### 3.1 Fake image detection

* 2017 ICSIP [Automated face swapping and its detection](https://ieeexplore.ieee.org/abstract/document/8124497)
* 2018 Workshop on IHMS [Fake Faces Identification via Convolutional Neural Network](https://dl.acm.org/citation.cfm?id=3206009)
* 2018 MIPR [Detection of GAN-Generated Fake Images over Social Networks](https://ieeexplore.ieee.org/abstract/document/8397040/)
* 2018 ISCCC [Learning to Detect Fake Face Images in the Wild](https://ieeexplore.ieee.org/abstract/document/8644886/)
* 2019 CCBR [On the Generalization of GAN Image Forensics](https://link.springer.com/chapter/10.1007/978-3-030-31456-9_15)
* 2019 [Limits of Deepfake Detection: A Robust Estimation Viewpoint](https://arxiv.org/abs/1905.03493)
* 2019 [Deep Fake Image Detection based on Pairwise Learning](https://www.preprints.org/manuscript/201905.0013/v1)
* 2019 [Multi-task learning for detecting and segmenting manipulated facial images and videos](https://arxiv.org/abs/1906.06876)

#### 3.2 Fake video detection

#### 3.2.1 Temporal features across frames based ones

Year|Publicatidfons|Classifiers/<br>Techniques|Description|Feature
:--:|:-------------|:---:|:----------|:-------------
2018 AVSS|[Intra-frame and temporal inconsistencies](https://ieeexplore.ieee.org/abstract/document/8639163)|CNN and LSTM|- The generation of Deepfake videos(deepfakes,face2face) is explained in detail.<br> -  CNN is employed to extract framelevel features, which are then fed into the LSTM to create a temporal sequence descriptor.<br> - A fully-connected network is used afterwards for classifying doctored videos from real ones based on the sequence descriptor.<br> - CNN is employed to extract frame-level features, which are distributed to LSTM to construct sequence descriptor useful for classification.|low level
2018 WIFS|[Eye blinking](https://ieeexplore.ieee.org/abstract/document/8630787)|LRCN|- Use LRCN to learn the temporal patterns of eye blinking. <br> - Based on the observation that blinking frequency of deepfakes is much smaller than normal.|by detecting eye blinking.
2019 CVPR Workshop|[Rsing spatiotemporal features](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Sabir_Recurrent_Convolutional_Strategies_for_Face_Manipulation_Detection_in_Videos_CVPRW_2019_paper.pdf)|RCN|-Temporal discrepancies across frames are explored using RCN that integrates convolutional network DenseNet and the gated recurrent unit cells- A deepfake detection method using CNN and LSTM to extract temporal features of a given video sequence, which are  represented via the sequence descriptor. <br> - The detection network consisting of fully-connected layers is employed to take the sequence descriptor as input and calculate probabilities of the frame sequence belonging to either authentic or deepfake class.

#### 3.2.2 Visual artifacts within video frame based methods

##### 3.2.2.1 Deep classifiers

Year|Publicatidfons|Classifiers/<br>Techniques|Description|Feature
:--:|:-------------|:--------------------:|:----------|:-------
2017 CVPR Workshop|[Two-Stream](https://ieeexplore.ieee.org/abstract/document/8014963)||Created a dataset utilizing one iOS app called SwapMe and an open-source face swap application called FaceSwap.|
2018 WIFS|[MesoNet](https://ieeexplore.ieee.org/abstract/document/8630761)|CNN|- The generation of Deepfake videos (deepfakes,face2face) is explained in detail. <br> - Two deep networks, i.e. Meso-4 and MesoInception-4 are introduced to examine deepfake videos at the mesoscopic analysis level.|low level
2019 CVPR Workshop|[Using face warping artifacts](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Li_Exposing_DeepFake_Videos_By_Detecting_Face_Warping_Artifacts_CVPRW_2019_paper.pdf)|VGG16 ResNet50, 101 or 152|Artifacts are discovered using CNN modelsbased on resolution inconsistency between the warped face area and the surrounding context.
2019 ICASSP|[Capsule-forensics](https://ieeexplore.ieee.org/abstract/document/8682602)|Capsule networks|- The proposed method yields the best performance compared to its competing methods in all of these data sets|low level

##### 3.2.2.2 Shallow classifiers

Year|Publications|Classifiers/<br>Techniques|Description|Feature
:--:|:-------------|:--------------------:|:----------|:-------
2019 ICASSP|[Head poses](https://ieeexplore.ieee.org/abstract/document/8683164)|SVM|- by observing the differences between 3D head poses comprising head orientation and position.<br> - Features are extracted using 68 landmarks of the face region. <br> - Use SVM to classify using the extracted features.|using inconsistent head poses
2019 WACVW|[Eye, teach and facial texture](https://ieeexplore.ieee.org/abstract/document/8638330)|Logistic regression and neural network|-The eye feature vector, teeth feature vector and features extracted from the full-face crop are used. <br> - Two classifiers including logistic regression and small neural network are employed to classify the deepfakes from real videos.<br> - Exploit facial texture differences, and missing reflections and details in eye and teeth areas of deepfakes. <br> - Logistic regression and neural network are used for classifying.|low level
2018 IMVIP|[PRNU Analysis](https://www.researchgate.net/profile/Zeno_Geradts/publication/329814168_Detection_of_Deepfake_Video_Manipulation/links/5c1bdf7da6fdccfc705da03e/Detection-of-Deepfake-Video-Manipulation.pdf)|PRNU|- Analysis of noise patterns of light sensitive sensors of digital cameras due to their factory defects. <br> - Explore the differences of PRNU patterns between the authentic and deepfake videos because face swapping is believed to alter the local PRNU patterns.|- The authors created a test data set consisting of 10 authentic videos and 16 manipulated videos where the fake videos were produced from the genuine ones by the DeepFaceLab tool.
2019 IEEE Access|[Blockchain](https://ieeexplore.ieee.org/abstract/document/8668407)|Blockchain|- This approach is generic, and it can be extended to other types of digital content such as images, audios and manuscripts.<br> - This approach is generic, and it can be extended to other types of digital content such as images, audios and manuscripts.
2019 CVPR Workshops|[*Protecting World Leaders*](https://pdfs.semanticscholar.org/ac1f/84cc50f31b2ae7775820242d7c71f1c3f42a.pdf)|svm, OpenFace2|- When individuals speak, they exhibit relatively distinct patterns of facial and head movements. <br>- We use the Pearson correlation to measure the linearity between these features in order to characterize an individual’s motion signature. <br> - We concentrate on the videos of persons of interest(POIs) talking in a formal setting, for example, weekly address, news interview, and public speech.<br> - Faceswap-GAN used for generating fakes.|qwer





