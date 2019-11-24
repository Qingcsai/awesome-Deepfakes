# Deepfakes相关资料整理

## Table of Contents

* [1.Deepfakes社会性发展调研报告](#1.Deepfakes社会性发展调研报告)
* [Deepfakes datasets](#2Deepfakes datasets)
* [Deepfake Creation](#3 Deepfake Creation)
* [3.1 Face-swapping methods](#3.1 Face-swapping methods)
 * [3.2 Face reenactment methods](#3.2 Face reenactment methods)
* [4 Deepfake Detection](#4 Deepfake Detection)
 * [4.1 Fake image detection](#4.1 Fake image detection)
 * [4.2 Fake video detection](#4.2 Fake video detection)
  * [4.2.1 Temporal features across frames based ones](#4.2.1 Temporal features across frames based ones)

## 1.Deepfakes社会性发展调研报告

* 荷兰初创公司[Deeptrace](https://deeptracelabs.com/)发布两个年度（2018年和2019年）[Deepfakes发展状况调研报告](https://github.com/Qingcsai/Deepfakes-Zoo/tree/master/the-state-of-deepfakes)

## 2 Deepfakes datasets

Datasets|Year|Ratio<br>tampered:original|Total videos|Source|Participants Consent|Tools
:-------:|:----:|:-----------:|:----:|:---:|:-----:|:--:
[UADFV](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8630787)|2018|1 : 1.00|98|YouTube|N|FakeAPP
[FaceForensics](https://arxiv.org/abs/1803.09179)|2018|1 : 1.00|2008|YouTube|N|Face2Face
[Deepfake-TIMIT](https://www.idiap.ch/dataset/deepfaketimit)|2019|1 : 1.00|620|Vid-TIMIT|N|faceswap-GAN 
[FaceForensics++](https://github.com/ondyari/FaceForensics)|2019|1 : 0.25|5000|YouTube|N|faceswap <br> DeepFake <br> Face2Face <br> NeuralTextures
[DeepFakeDetection<br>(part of FaceForensics++)](https://deepfakedetectionchallenge.ai/dataset)|2019|1 : 0.12|3363|Actors|Y
[Celeb-DF](http://www.cs.albany.edu/~lsw/celeb-deepfakeforensics.html)|2019|1 : 0.51|1203|YouTube|N|a refined version of the DeepFake
[DFDC Preview Dataset](https://deepfakedetectionchallenge.ai/dataset)|2019|1 : 0.28|5214|Actors|Y|Unkonwn

## 3 Deepfake Creation

### 3.1 Face-swapping methods

* Open-source code
  * [Deepfakes](https://github.com/deepfakes/faceswap) [Star27.6k]
  * [Faceswap-GAN](https://github.com/shaoanlu/faceswap-GAN) [Star2.5k]
  * [FaceSwap](https://github.com/MarekKowalski/FaceSwap) [Star300+]
  * [DeepFaceLab](https://github.com/iperov/DeepFaceLab) [Star11.1k]
  * [DFaker](https://github.com/dfaker/df) [Star300+]
  * [DeepFake-tf](https://github.com/StromWine/DeepFake_tf) [Star<10]

* Paper
  * 2017 ICCV [Fast Face-swap Using CNN](http://openaccess.thecvf.com/content_iccv_2017/html/Korshunova_Fast_Face-Swap_Using_ICCV_2017_paper.html)
  * 2018 FG [On Face Segmentation, Face Swapping, and Face Perception](https://ieeexplore.ieee.org/abstract/document/8373817/)
  * 2019 ICCV [FSGAN](http://openaccess.thecvf.com/content_ICCV_2019/papers/Nirkin_FSGAN_Subject_Agnostic_Face_Swapping_and_Reenactment_ICCV_2019_paper.pdf)

### 3.2 Face reenactment methods

* 2014 ICPR [Face Anti-spoofing Based on General Image Quality Assessment](https://ieeexplore.ieee.org/abstract/document/6976921)
* 2015 TIFS [Face spoof detection with image distortion analysis.](https://ieeexplore.ieee.org/abstract/document/7031384)
* 2016 CVPR [face2face](http://openaccess.thecvf.com/content_cvpr_2016/html/Thies_Face2Face_Real-Time_Face_CVPR_2016_paper.html)
* 2018 [HeadOn: Real-time Reenactment of Human Portrait Videos](http://niessnerlab.org/papers/2018/7headon/headon_preprint.pdf)
* 2017 CVPR [Lip reading sentences in the wild](https://ieeexplore.ieee.org/abstract/document/8099850)
* 2017 TOG [Synthesizing Obama](https://dl.acm.org/citation.cfm?id=3073640)
* 2017 TOG [Bringing portraits to life](https://dl.acm.org/citation.cfm?id=3130818)
* 2018 EUSIPCO [Speaker inconsistency detection in tampered video](https://ieeexplore.ieee.org/abstract/document/8553270)
* 2018 TOG [Deep video portraits](https://dl.acm.org/citation.cfm?id=3201283)
* 2018 arxiv [Generative Adversarial Talking Head](https://.org/abs/1803.07716)
* 2019 arxiv [Few-Shot Adversarial Learning of Realistic Neural Talking Head Models](https://arxiv.org/abs/1905.08233https://arxiv.org/abs/1905.08233)
* 2019 arxiv [Deferred Neural Rendering: Image Synthesis using Neural Textures](https://arxiv.org/abs/1904.12356)
* 2019 AAAI Oral MMLAB-CUHK [Talking Face Generation by Adversarially Disentangled Audio-Visual Representation](https://arxiv.org/abs/1807.07860)

### 4 Deepfake Detection

#### 4.1 Fake image detection

* 2017 ICSIP [Automated face swapping and its detection](https://ieeexplore.ieee.org/abstract/document/8124497)
* 2018 IHMS Workshop [Fake Faces Identification via Convolutional Neural Network](https://dl.acm.org/citation.cfm?id=3206009)
* 2018 MIPR [Detection of GAN-Generated Fake Images over Social Networks](https://ieeexplore.ieee.org/abstract/document/8397040/)
* 2018 ISCCC [Learning to Detect Fake Face Images in the Wild](https://ieeexplore.ieee.org/abstract/document/8644886/)
* 2019 CCBR [On the Generalization of GAN Image Forensics](https://link.springer.com/chapter/10.1007/978-3-030-31456-9_15)
* 2019 [Limits of Deepfake Detection: A Robust Estimation Viewpoint](https://arxiv.org/abs/1905.03493)
* 2019 [Deep Fake Image Detection based on Pairwise Learning](https://www.preprints.org/manuscript/201905.0013/v1)
* 2019 [Multi-task learning for detecting and segmenting manipulated facial images and videos](https://arxiv.org/abs/1906.06876)

#### 4.2 Fake video detection

##### 4.2.1 Temporal features across frames based ones

Year|Publicatidfons|Classifiers/<br>Techniques
:--:|:-------------|:---:
2018 AVSS|[Intra-frame and temporal inconsistencies](https://ieeexplore.ieee.org/abstract/document/8639163)|CNN and LSTM
2018 WIFS|[Eye blinking](https://ieeexplore.ieee.org/abstract/document/8630787)|LRCN
2019 CVPR Workshop|[Rsing spatiotemporal features](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Sabir_Recurrent_Convolutional_Strategies_for_Face_Manipulation_Detection_in_Videos_CVPRW_2019_paper.pdf)|RCN

##### 4.2.2 Visual artifacts within video frame based methods

###### 4.2.2.1 Deep classifiers

Year|Publicatidfons|Classifiers/<br>Techniques
:--:|:-------------|:--------------------:
2017 CVPR Workshop|[Two-Stream Neural Networks for Tampered Face Detection](https://ieeexplore.ieee.org/abstract/document/8014963)|Two-Stream
2018 WIFS|[MesoNet: a Compact Facial Video Forgery Detection Network](https://ieeexplore.ieee.org/abstract/document/8630761)|CNN
2019 CVPR Workshop|[Exposing DeepFake Videos By Detecting Face Warping Artifacts](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Li_Exposing_DeepFake_Videos_By_Detecting_Face_Warping_Artifacts_CVPRW_2019_paper.pdf)|VGG16 ResNet50, 101 or 152
2019 ICASSP|[Capsule-forensics: Using Capsule Networks to Detect Forged Images and Videos](https://ieeexplore.ieee.org/abstract/document/8682602)|Capsule networks

###### 4.2.2.2 Shallow classifiers

Year|Publications|Classifiers/<br>Techniques
:--:|:-------------|:--------------------:
2019 ICASSP|[Exposing Deep Fakes Using Inconsistent Head Poses](https://ieeexplore.ieee.org/abstract/document/8683164)|SVM
2019 WACVW|[Exploiting Visual Artifacts to Expose Deepfakes and Face Manipulations](https://ieeexplore.ieee.org/abstract/document/8638330)|Logistic regression and neural network
2018 IMVIP|[Detection of Deepfake Video Manipulation](https://www.researchgate.net/profile/Zeno_Geradts/publication/329814168_Detection_of_Deepfake_Video_Manipulation/links/5c1bdf7da6fdccfc705da03e/Detection-of-Deepfake-Video-Manipulation.pdf)|PRNU
2019 IEEE Access|[Combating Deepfake Videos Using Blockchain and Smart Contracts](https://ieeexplore.ieee.org/abstract/document/8668407)|Blockchain
2019 CVPR Workshops|[Protecting World Leaders Against Deep Fakes](https://pdfs.semanticscholar.org/ac1f/84cc50f31b2ae7775820242d7c71f1c3f42a.pdf)|svm, OpenFace2
