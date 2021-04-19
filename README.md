# All about Deepfakes

## Catalogue

* [1 Deepfakes社会性发展调研报告](#1-Deepfakes社会性发展调研报告)
* [2 Deepfakes Datasets](#2-Deepfakes-datasets)
* [3 Deepfake Creation](#3-Deepfake-Creation)  
  * [3.1 Face-swapping methods](#31-Face-swapping-methods)
  * [3.2 Face reenactment methods](#32-Face-reenactment-methods)
* [4 Deepfake Detection](#4-Deepfake-Detection)  
  * [4.1 Fake image detection](#41-Fake-image-detection)
  * [4.2 Fake video detection](#42-Fake-video-detection)
    * [4.2.1 Temporal features across frames based ones](#421-Temporal-features-across-frames-based-ones)
    * [4.2.2 Visual artifacts within video frame based methods](#422-Visual-artifacts-within-video-frame-based-methods)

## 1 Deepfakes survey

* 2018 arxiv [DeepFakes: a New Threat to Face Recognition? Assessment and Detection](https://arxiv.org/abs/1812.08685)
* 2019 arXiv [Deep Learning for Deepfakes Creation and Detection](https://arxiv.org/abs/1909.11573)
* 2020 arXiv [DeepFakes and Beyond: A Survey of Face Manipulation and Fake Detection](https://arxiv.org/abs/2001.00179)
* 2020 arXiv [Media Forensics and DeepFakes: an overview](https://www.semanticscholar.org/paper/Media-Forensics-and-DeepFakes%3A-an-overview-Verdoliva/10e19c22877621990f64ec7190364e63c0dcda68)
* 2021 ACM Computing Surveys [The Creation and Detection of Deepfakes: A Survey](https://dl.acm.org/doi/abs/10.1145/3425780)
* 荷兰初创公司[Deeptrace](https://deeptracelabs.com/)发布两个年度（2018年和2019年）[Deepfakes发展状况调研报告](https://github.com/Qingcsai/Deepfakes-Zoo/tree/master/the-state-of-deepfakes)

## 2 Deepfakes Datasets

Datasets|Year|Ratio<br>tampered:original|Total videos|Source|Participants Consent|Tools
:-------:|:----:|:-----------:|:----:|:---:|:-----:|:--:
[UADFV](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8630787)|2018|1 : 1.00|98|YouTube|N|FakeAPP
[FaceForensics](https://arxiv.org/abs/1803.09179)|2018|1 : 1.00|2008|YouTube|N|Face2Face
[Deepfake-TIMIT](https://www.idiap.ch/dataset/deepfaketimit)|2019|1 : 1.00|620|Vid-TIMIT|N|faceswap-GAN 
[FaceForensics++](https://github.com/ondyari/FaceForensics)|2019|1 : 0.25|5000|YouTube|N|faceswap <br> DeepFake <br> Face2Face <br> NeuralTextures
[DeepFakeDetection<br>(part of FaceForensics++)](https://deepfakedetectionchallenge.ai/dataset)|2019|1 : 0.12|3363|Actors|Y
[Celeb-DF](http://www.cs.albany.edu/~lsw/celeb-deepfakeforensics.html)|2019|1 : 0.51|1203|YouTube|N|a refined version of the DeepFake
[DFDC Preview Dataset](https://deepfakedetectionchallenge.ai/dataset)|2019|1 : 0.28|5214|Actors|Y|Unkonwn
[KoDF](https://arxiv.org/abs/2103.10094)|2021| | | | 
[Face Forensics in the Wild](https://arxiv.org/abs/2103.16076) | 2021 CVPR | | | |

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

Year|Publications|Authors
:--:|:-------------:|:-----:
2017 ICCV | [Fast Face-Swap Using Convolutional Neural Networks](http://openaccess.thecvf.com/content_iccv_2017/html/Korshunova_Fast_Face-Swap_Using_ICCV_2017_paper.html) |Iryna Korshunova, Wenzhe Shi, Joni Dambre, Lucas Theis
2018 IEEE FG | [On Face Segmentation, Face Swapping, and Face Perception](https://ieeexplore.ieee.org/abstract/document/8373817/) |Yuval Nirkin; Iacopo Masi; Anh Tran Tuan; Tal Hassner; Gerard Medioni
2019 ICCV | [FSGAN: Subject Agnostic Face Swapping and Reenactment](https://openaccess.thecvf.com/content_ICCV_2019/html/Nirkin_FSGAN_Subject_Agnostic_Face_Swapping_and_Reenactment_ICCV_2019_paper.html) | Yuval Nirkin, Yosi Keller, Tal Hassner
2020 CVPR(Oral) | [FaceShifter: Towards High Fidelity And Occlusion Aware Face Swapping](http://lingzhili.com/FaceShifterPage/) |Lingzhi Li, Jianmin Bao, Hao Yang, Dong Chen, Fang Wen

### 3.2 Face reenactment methods

Year|Publications
:--:|:-------------:
2014 ICPR | [Face Anti-spoofing Based on General Image Quality Assessment](https://ieeexplore.ieee.org/abstract/document/6976921)
2015 TIFS | [Face spoof detection with image distortion analysis.](https://ieeexplore.ieee.org/abstract/document/7031384)
2016 CVPR | [Face2Face: Real-Time Face Capture and Reenactment of RGB Videos](http://openaccess.thecvf.com/content_cvpr_2016/html/Thies_Face2Face_Real-Time_Face_CVPR_2016_paper.html)
2018 TOG | [HeadOn: Real-time Reenactment of Human Portrait Videos](https://dl.acm.org/doi/abs/10.1145/3197517.3201350)
2017 CVPR | [Lip reading sentences in the wild](https://ieeexplore.ieee.org/abstract/document/8099850)
2017 TOG | [Synthesizing Obama: learning lip sync from audio](https://dl.acm.org/citation.cfm?id=3073640)
2017 TOG | [Bringing portraits to life](https://dl.acm.org/citation.cfm?id=3130818)
2018 EUSIPCO | [Speaker inconsistency detection in tampered video](https://ieeexplore.ieee.org/abstract/document/8553270)
2018 TOG | [Deep video portraits](https://dl.acm.org/citation.cfm?id=3201283)
2018 arxiv | [Generative adversarial talking head: Bringing portraits to life with a weakly supervised neural network](https://arxiv.org/abs/1803.07716)
2019 ICCV | [Few-Shot Adversarial Learning of Realistic Neural Talking Head Models](https://openaccess.thecvf.com/content_ICCV_2019/html/Zakharov_Few-Shot_Adversarial_Learning_of_Realistic_Neural_Talking_Head_Models_ICCV_2019_paper.html)
2019 TOG | [Deferred Neural Rendering: Image Synthesis using Neural Textures](https://arxiv.org/abs/1904.12356)
2019 AAAI Oral MMLAB-CUHK | [Talking Face Generation by Adversarially Disentangled Audio-Visual Representation](https://arxiv.org/abs/1807.07860)

### 4 Deepfake Detection

#### 4.1 Fake image detection

Year|Publications|Authors
:--:|:-------------:|:--:
2017 ICSIP | [Automated face swapping and its detection](https://ieeexplore.ieee.org/abstract/document/8124497) | Ying Zhang; Lilei Zheng; Vrizlynn L. L. Thing
2018 IHMS Workshop | [Fake Faces Identification via Convolutional Neural Network](https://dl.acm.org/citation.cfm?id=3206009) |Huaxiao Mo, Bolin Chen, Weiqi  Luo
2018 MIPR | [Detection of GAN-Generated Fake Images over Social Networks](https://ieeexplore.ieee.org/abstract/document/8397040/) |Francesco Marra; Diego Gragnaniello; Davide Cozzolino; Luisa Verdoliva
2018 ISCCC | [Learning to Detect Fake Face Images in the Wild](https://ieeexplore.ieee.org/abstract/document/8644886/)| Chih-Chung Hsu; Chia-Yen Lee; Yi-Xiu Zhuang
2019 CCBR | [On the Generalization of GAN Image Forensics](https://link.springer.com/chapter/10.1007/978-3-030-31456-9_15)
2019 aXiv | [Limits of Deepfake Detection: A Robust Estimation Viewpoint](https://arxiv.org/abs/1905.03493) |Sakshi Agarwal, Lav R. Varshney
2019 MDPI AG | [Deep Fake Image Detection based on Pairwise Learning](https://www.mdpi.com/2076-3417/10/1/370) |Chih-Chung Hsu, Yi-Xiu Zhuang and Chia-Yen Lee 
2019 IEEE BTAS | [Multi-task learning for detecting and segmenting manipulated facial images and videos](https://ieeexplore.ieee.org/abstract/document/9185974) |Huy H. Nguyen; Fuming Fang; Junichi Yamagishi; Isao Echizen
2021 CVPR | [Multi-attentional Deepfake Detection](https://arxiv.org/abs/2103.02406) |Hanqing Zhao, Wenbo Zhou, Dongdong Chen, Tianyi Wei, Weiming Zhang, Nenghai Yu
2021 CVPR | [Spatial-Phase Shallow Learning: Rethinking Face Forgery Detection in Frequency Domain](https://arxiv.org/abs/2103.01856) |Honggu Liu, Xiaodan Li, Wenbo Zhou, Yuefeng Chen, Yuan He, Hui Xue, Weiming Zhang, Nenghai Yu
2021 CVPR | [Improving the Efficiency and Robustness of Deepfakes Detection through Precise Geometric Features](https://arxiv.org/abs/2104.04480) | Zekun Sun, Yujie Han, Zeyu Hua, Na Ruan, Weijia Jia
2021 CVPR | [Frequency-aware Discriminative Feature Learning Supervised by Single-Center Loss for Face Forgery Detection](https://arxiv.org/abs/2103.09096) |Jiaming Li, Hongtao Xie, Jiahong Li, Zhongyuan Wang, Yongdong Zhang
2021 CVPR | [MagDR: Mask-guided Detection and Reconstruction for Defending Deepfakes](https://arxiv.org/abs/2103.14211) | Zhikai Chen, Lingxi Xie, Shanmin Pang, Yong He, Bo Zhang


#### 4.2 Fake video detection 
##### 4.2.1 Temporal features across frames based ones

Year|Publications|Classifiers/<br>Techniques
:--:|:-------------|:---:
2018 AVSS|[Intra-frame and temporal inconsistencies](https://ieeexplore.ieee.org/abstract/document/8639163)|CNN and LSTM
2018 WIFS|[In Ictu Oculi: Exposing AI Created Fake Videos by Detecting Eye Blinking](https://ieeexplore.ieee.org/abstract/document/8630787)|LRCN
2019 CVPR Workshop|[Recurrent Convolutional Strategies for Face Manipulation Detection in Videos](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Sabir_Recurrent_Convolutional_Strategies_for_Face_Manipulation_Detection_in_Videos_CVPRW_2019_paper.pdf)|RCN

##### 4.2.2 Visual artifacts within video frame based methods
Year|Publications|Classifiers/<br>Techniques
:--:|:-------------|:--------------------:
2017 CVPR Workshop|[Two-Stream Neural Networks for Tampered Face Detection](https://ieeexplore.ieee.org/abstract/document/8014963)|Two-Stream
2018 WIFS|[MesoNet: a Compact Facial Video Forgery Detection Network](https://ieeexplore.ieee.org/abstract/document/8630761)|CNN
2018 IMVIP|[Detection of Deepfake Video Manipulation](https://www.researchgate.net/profile/Zeno_Geradts/publication/329814168_Detection_of_Deepfake_Video_Manipulation/links/5c1bdf7da6fdccfc705da03e/Detection-of-Deepfake-Video-Manipulation.pdf)|PRNU
2019 CVPR Workshop|[Exposing DeepFake Videos By Detecting Face Warping Artifacts](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Li_Exposing_DeepFake_Videos_By_Detecting_Face_Warping_Artifacts_CVPRW_2019_paper.pdf)|VGG16 ResNet50, 101 or 152
2019 ICASSP|[Capsule-forensics: Using Capsule Networks to Detect Forged Images and Videos](https://ieeexplore.ieee.org/abstract/document/8682602)|Capsule networks
2019 ICASSP|[Exposing Deep Fakes Using Inconsistent Head Poses](https://ieeexplore.ieee.org/abstract/document/8683164)|SVM
2019 WACVW|[Exploiting Visual Artifacts to Expose Deepfakes and Face Manipulations](https://ieeexplore.ieee.org/abstract/document/8638330)|Logistic regression and neural network
2019 IEEE Access|[Combating Deepfake Videos Using Blockchain and Smart Contracts](https://ieeexplore.ieee.org/abstract/document/8668407)|Blockchain
2019 CVPR Workshops|[Protecting World Leaders Against Deep Fakes](https://pdfs.semanticscholar.org/ac1f/84cc50f31b2ae7775820242d7c71f1c3f42a.pdf)|svm, OpenFace2
