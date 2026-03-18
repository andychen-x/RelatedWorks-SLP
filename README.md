# RelatedWorks-SLP
A list of excellent works on various stages of Sign Language Production (SLP) (automatic translation from spoken sentences to sign language sequences). It contains an extensive literature review on the field of deep learning-based sign language generation, sign language synthesis, sign language avatar recovery, pose estimation, and all related publications.

I am gathering these papers as literature for my PhD, and thought others may be interested. If you have any updates, please feel free to contribute or email me at [2021111446@mail.hfut.edu.cn](2021111446@mail.hfut.edu.cn).

# What about Sign Language Production?
Sign Language Production (SLP) is a research and technology field dedicated to automatically generating sign language from text (spoken language). Its output is a visual representation of sign language, which may appear as pose sequences, avatar animations, or synthesized videos of real signers. Using pose sequences as the output, common research pipelines for sign language production are as follows:

- The first baseline adopts a fully end-to-end model that directly maps the input text $x=\{x_1 ,⋯,x_I\}$ to sign pose sequences $y=\{y_1,⋯,y_J\}$ without relying on any intermediate gloss $g=\{g_1,⋯,g_K\}$ annotations.

- The second baseline decomposes sign generation into two stages: text-to-gloss (T2G) translation and gloss-to-pose (G2P) generation.

- The third baseline explores a non-neural approach for the G2P stage by replacing the G2P module with a dictionary-based pose synthesizer $\mathcal{D}$.



## Review 
- SLRTP2025 Sign Language Production Challenge: Methodology, Results, and Future Work [2025 CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2025W/SLRTP/papers/Walsh_SLRTP2025_Sign_Language_Production_Challenge_Methodology_Results_and_Future_Work_CVPRW_2025_paper.pdf)]
- A survey on recent advances in Sign Language Production [2024 ESA-ccfc][[Paper](https://pdf.sciencedirectassets.com/271506/1-s2.0-S0957417423X00360/1-s2.0-S0957417423033481/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjENj%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJGMEQCIDPb8mf8VmRC6CuzvE86GUjfPakr5c1LW%2FGyBFcusp88AiAoQ5%2FmpwcW%2FEg5%2FsnQDUm6XdPbARwrIFFHPcmZzAZ%2BEiq8BQiB%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAUaDDA1OTAwMzU0Njg2NSIM16db2OUELjdnXoYZKpAFAaM%2BsBxw%2FtSiJQQ8oJgmLsdJe%2Bi5wibNkx23UhyRp0KUlaDZVP9uJQQjVHtekEBhy3sHRQRi%2B64C%2F1iUJQTCvZ1l%2BRKMMTDCfmrsJ7FxpwtpLhnmhhXSJixKHOLqYCSMXKrbIM0YORzPc7DK2kRHF8Ei2GVkbOd8QHNnTZreWvvcD1jKh8qJUNGvzmxW%2BkHdegRGYWHZ%2BjGSXh4iNtD3LXUYpMLLXig8QA5hYoPIs7X6Y80psCyMFWlDgPFzRTDScUD4p2Sj9fQ3VkKRJYIdLzUx90ygIdVaNsFhkmX8AIrnO6oYwEzgeln0srZ12Ld37aCsyl9i0YujsrybDAap9Gln1%2FGNAbCJ%2Blpj1O5FqTf%2FgU9HqT6zi%2FWjvnE5ZOmJXI7F5U0JkXVF%2BgFlp7NF%2Fmsx1X3NA9IjHOAvd8d4wjiLwCz0bxsjoMKeqIJMIhyYFvTeJR3nRryMO30rFMPmLdlBKWdNzsZf56idg7bN0hMwmE4ZWPtS6wne%2BfhO8rtykVAdCQfNzwUv8se2y0XlpyR2wa4STj3%2BoOPpCCbTR3r9vRWtfvJr1vWqQoez8GQSdKn2Ms9XrIlIrrWbE%2FeeaboCwjLJzKGmP2QxlUNVBYeNzwQe%2BvBe5Fg%2BvqC%2FujbtSulN%2FD5QP%2BORDe5p03EtpNQwrUYBcpti1BNkrP5nEAGoM1auLLo7zng%2BnkEW6KqFqpCCw4gmOsw79c4JPAuqrTqL2EHHNLm77PKHi8jHOSX%2BOyuVq7ut639MoBPlN0ApYYW0eZqj4iEjxOnAedp1N33cT2zl6qSLZPJqAnlNvj%2BGCumYjptCA4nfpyZlqAAYZ%2F1e3UkwM4ZKHGVFcZCafwf3MJYY2kmIxiulhkLMXmIwqOnAxwY6sgH6KtCG%2FAFg%2BecCC4ryvA%2Fgov0J5Ox8di6hqc9MwhqJj%2B1fr5oTXKZQtNjA5j8Feh%2FvdIvfsUU%2FZpAuSQzYLWG7JtVWwF2jjhrTdyRpTFuoIdtz6wy%2BG5ibCxFqfH7kxbOx6GP2AJr6W71eQOxjo%2FfizVPAH6%2BJJ%2B3tACTpmI3%2BYPXRWUvbOWhlp5pO3o1IvhgtwhMzI4p%2BW0wbpxKmQcwIYF5Z%2FZwUoo%2B4GgEwcbkUlvge&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20251016T003626Z&X-Amz-SignedHeaders=host&X-Amz-Expires=299&X-Amz-Credential=ASIAQ3PHCVTYVP2FBSOU%2F20251016%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=8bd5cb7c8f37652dea6b3395c9e812a052fa58696839ae86d7e1affe401ec0f8&hash=70a6b640ef143b3eae2eec3874d861902434ae51dee4261193673d2e4795d73b&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0957417423033481&tid=spdf-c56b1392-cb93-480b-9e58-098ad3e258b5&sid=c7d292931cb66649474a524-1f90f9be0dffgxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=0e135c5b095d58055601&rr=98f37b5c6afaa3ab&cc=tw&kca=eyJrZXkiOiJyUVFueFgzMGdFSG9Wd2FBbTRMVE9uK2w4cXhLTTczQXBZV3ZjNzQ5NGZSOXNpMzErMitlWitVMjBqMThac01kNEE1VUlGbXBDR3lrSkUyNWNaSHBMczlKdm5rSUFzZkYyRjVacXlyQ2VnT2hpOTRYZFBOT0ZwMmlXRnlSREMrUXF1V0oyOGJQcUFPMU8xRVFBdzFscUFlTDJuNXRPT1d2SFBzUU82TG9FZXA3d2l3bHFRPT0iLCJpdiI6ImYxMzc3YzgyYjZkYjQ2YWNkOWU1ZTQ4NzBhODJlYWY4In0=_1760575167412)]
- Sign Language Production: A Review [2021 CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2021W/ChaLearn/papers/Rastgoo_Sign_Language_Production_A_Review_CVPRW_2021_paper.pdf)]

## Sign Language Production
### 2025
- Diffusion-Based Continuous Sign Language Generation with Cluster-Specific Fine-Tuning and Motion-Adapted Transformer. [CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2025W/SLRTP/papers/Rastgoo_Diffusion-Based_Continuous_Sign_Language_Generation_with_Cluster-Specific_Fine-Tuning_and_Motion-Adapted_CVPRW_2025_paper.pdf)]
- Sign-Mamba: Advanced Mamba-Based Sign Language Generation. [ICASSP-ccfb][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10890373)]

### 2024
- T2S-GPT: Dynamic Vector Quantization for Autoregressive Sign Language Production from Text. [ACL-ccfa][[Paper](https://aclanthology.org/2024.acl-long.183.pdf)]
- MS2SL: Multimodal Spoken Data-Driven Continuous Sign Language Production. [ACL-ccba][[Paper](https://aclanthology.org/2024.findings-acl.432.pdf)]
- Unsupervised Sign Language Translation and Generation [ACL-ccba][[Paper](https://arxiv.org/pdf/2402.07726)][[Code](https://github.com/ZhengshengGuo/USLNet)]
- Pose Guided Fine-Grained Sign Language Video Generation. [ECCV-ccfb][[Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/09947.pdf)]
- SignGen: End-to-End Sign Language Video Generation with Latent Diffusion. [ECCV-ccfb][[Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06988.pdf)]
- **Semantic-driven diffusion for sign language production with gloss-pose latent spaces alignment**. [CVIU-ccfb][[Paper](https://linkinghub.elsevier.com/retrieve/pii/S1077314224001310)]
- Multi-Channel Spatio-Temporal Transformer for Sign Language Production. [LREC-ccfb][[Paper](https://aclanthology.org/2024.lrec-main.1022.pdf)]
- Attentional bias for hands: Cascade dual‐decoder transformer for sign language production [IETCV-ccfc][[Paper](https://ietresearch.onlinelibrary.wiley.com/doi/epdf/10.1049/cvi2.12273)]
- Select and Reorder: A Novel Approach for Neural Sign Language Production. [LREC-ccfb][[Paper](https://www.semanticscholar.org/reader/e2a56a27010a60fb9820c94adf8e361633d27fe1)] 
- Sign Language Production With Latent Motion Transformer.[WACV 2024][[Paper](https://openaccess.thecvf.com/content/WACV2024/papers/Xie_Sign_Language_Production_With_Latent_Motion_Transformer_WACV_2024_paper.pdf)]
- LLM-based Sign Language Production


### 2023
- SignNet: Single Channel Sign Generation using Metric Embedded Learning. [ICAFGR-ccbc][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10042711)]

### 2022
- Signing at Scale: Learning to Co-Articulate Signs for Large-Scale Photo-Realistic Sign Language Production. [CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Saunders_Signing_at_Scale_Learning_to_Co-Articulate_Signs_for_Large-Scale_Photo-Realistic_CVPR_2022_paper.pdf)]
- G2P-DDM: Generating Sign Pose Sequence from Gloss Sequence with Discrete Diffusion Model. [AAAI-ccfa][[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/28441/28860)]
- Modeling Intensification for Sign Language Generation: A Computational Approach. [ACL-ccfa][[Paper](https://arxiv.org/pdf/2203.09679)][[Code](https://github.com/Merterm/Modeling-Intensification-for-SLG)]
- DualSign: Semi-Supervised Sign Language Production with Balanced Multi-Modal Multi-Task Dual Transformation. [ACM Multimedia-ccfa][[Paper](https://dl.acm.org/doi/pdf/10.1145/3503161.3547957)]
- Gloss Semantic-Enhanced Network with Online Back-Translation for Sign Language Production. [ACM Multimedia-ccfa][[Paper](https://dl.acm.org/doi/pdf/10.1145/3503161.3547830)]


### 2021
- Mixed SIGNals: Sign Language Production via a Mixture of Motion Primitives. [ICCV-ccfa][[Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Saunders_Mixed_SIGNals_Sign_Language_Production_via_a_Mixture_of_Motion_ICCV_2021_paper.pdf)]
- Continuous 3D Multi-Channel Sign Language Production via Progressive Transformers and Mixture Density Networks. [IJCV-ccba][[Paper](https://link.springer.com/article/10.1007/s11263-021-01457-9)]
- Towards Fast and High-Quality Sign Language Production. [ACM Multimedia-ccfa][[Paper](https://dl.acm.org/doi/pdf/10.1145/3474085.3475463)]
- Towards Automatic Speech to Sign Language Generation. [Interspeech-ccfa][[Paper](https://www.semanticscholar.org/reader/c31934f1e4f1efa110afc94878e00315bdcb2780)]
- Non-Autoregressive Sign Language Production with Gaussian Space. [BMVC-ccfc][[Paper](https://www.bmvc2021-virtualconference.com/assets/papers/1102.pdf)]

### 2020
- Text2Sign: Towards Sign Language Production Using Neural Machine Translation and Generative Adversarial Networks. [IJCV-ccba][[Paper](https://link.springer.com/article/10.1007/s11263-019-01281-2)]
- Progressive Transformers for End-to-End Sign Language Production. [ECCV-ccfb][[Paper](https://link.springer.com/chapter/10.1007/978-3-030-58621-8_40)][[Code](https://github.com/BenSaunders27/ProgressiveTransformersSLP)]
- Signsynth: Data-driven sign language video generation [ECCV-ccfb][[Paper](https://link.springer.com/chapter/10.1007/978-3-030-66823-5_21)]
- Skeleton-based Chinese sign language recognition and generation for bidirectional communication between deaf and hearing people. [NN-ccfb][[Paper](https://www.sciencedirect.com/science/article/pii/S089360802030040X)]
- Adversarial Training for Multi-Channel Sign Language Production. [BMVC-ccfc][[Paper](https://arxiv.org/pdf/2008.12405)]

### 2019
- Cross-modal Neural Sign Language Translation [ACM Multimedia-ccfa][[Paper](https://dl.acm.org/doi/pdf/10.1145/3343031.3352587)]
- Deep Gesture Video Generation With Learning on Regions of Interest. [TMM-ccfb][[Paper](https://dl.acm.org/doi/pdf/10.1145/3343031.3352587)]

## Sign Avater 
### 2024
- Neural Sign Actors: A diffusion model for 3D sign language production from text. [CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Baltatzis_Neural_Sign_Actors_A_Diffusion_Model_for_3D_Sign_Language_CVPR_2024_paper.pdf)]
- SignAvatars: A Large-scale 3D Sign Language Holistic Motion Dataset and Benchmark. [ECCV-ccfb][[Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/00653.pdf)]
- A Simple Baseline for Spoken Language to Sign Language Translation with 3D Avatars. [ECCV-ccfb][[paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06499.pdf)]
- SignAvatar: Sign Language 3D Motion Reconstruction and Generation. [ICAFGR-ccfc][[Paper](https://arxiv.org/pdf/2405.07974)]
- A Comparative Study of Video-Based Human Representations for American Sign Language Alphabet Generation. [ICAFGR-ccfc][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10582020)]
- SynthSL: Expressive Humans for Sign Language Image Synthesis [ICAFGR-ccfc][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10582038)]

### 2023
- Reconstructing Signing Avatars from Video Using Linguistic Priors. [CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Forte_Reconstructing_Signing_Avatars_From_Video_Using_Linguistic_Priors_CVPR_2023_paper.pdf)]

### 2022
- There and Back Again: 3D Sign Language Generation from Text Using Back-Translation. [3DV-ccfc][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10044459)]

## Sign LLM
### 2025
- Teach Me Sign: Stepwise Prompting LLM for Sign Language Production. [ICIP][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11084322)]
- 


## Sign Language Understanding
### 2024
- Uncertainty-aware Sign Language Video Retrieval with Probability Distribution Modeling. [ECCV-ccfb][[Paper](https://arxiv.org/pdf/2405.19689)]
- SignCLIP: Connecting Text and Sign Language by Contrastive Learning. [EMNLP-ccfb][[Paper](https://arxiv.org/pdf/2407.01264)]

- SEDS: Semantically Enhanced Dual-Stream Encoder for Sign Language Retrieval [ACM Multimedia][[Paper](https://arxiv.org/pdf/2407.16394)]
  
### 2023
- CiCo: Domain-Aware Sign Language Retrieval via Cross-Lingual Contrastive Learning [CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Bao_CiCo_Domain-Aware_Sign_Language_Retrieval_via_Cross-Lingual_Contrastive_Learning_CVPR_2023_paper.pdf)][[Code](https://github.com/FangyunWei/SLRT)]

### 2021
- PiSLTRc: Position-informed Sign Language Transformer with Content-aware Convolution [TMM-ccfb][[Paper](https://arxiv.org/pdf/2107.12600)]

### Preprint
- Scaling up Multimodal Pre-training for Sign Language Understanding [2024][[Paper](https://arxiv.org/pdf/2408.08544)]
- C2RL: Content and Context RepresentationLearning for Gloss-free Sign Language Translation and Retrieval [2024][[Paper](https://arxiv.org/pdf/2408.09949)]

## Dataset
### CSLR Datasets
- Phoenix-2014T: Please follow [https://www-i6.informatik.rwth-aachen.de/~koller/RWTH-PHOENIX-2014-T/](https://www-i6.informatik.rwth-aachen.de/~koller/RWTH-PHOENIX-2014-T/). After preprocessing dataset, the condensed data set obtained is as follows:
[https://huggingface.co/datasets/phoenix-pre.zip](https://huggingface.co/datasets/SignDiff/phoenix-pre.zip).

- CSL-Daily: Please follow [http://home.ustc.edu.cn/~zhouh156/dataset/csl-daily/](http://home.ustc.edu.cn/~zhouh156/dataset/csl-daily/). After preprocessing dataset, the condensed data set obtained is as follows:
[https://huggingface.co/datasets/How2Sign-pre.zip](https://huggingface.co/datasets/SignDiff/How2Sign-Diff.zip)


### ISLR Datasets
- WLASL: Please follow [https://dxli94.github.io/WLASL/](https://dxli94.github.io/WLASL/).

- MSASL: Please follow [https://www.microsoft.com/en-us/research/project/ms-asl/](https://www.microsoft.com/en-us/research/project/ms-asl/).

## Other SLP Topic
### 2024
- Jointly Harnessing Prior Structures and Temporal Consistency for Sign Language Video Generation. [TOMM-ccfb][[Paper](https://dl.acm.org/doi/pdf/10.1145/3648368)]

### 2023
- Ham2Pose: Animating Sign Language Notation into Pose Sequences. [CVPR-ccfa][[Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Arkushin_Ham2Pose_Animating_Sign_Language_Notation_Into_Pose_Sequences_CVPR_2023_paper.pdf)]

### 2021
- ANONYSIGN: Novel Human Appearance Synthesis for Sign Language Video Anonymisation [ICAFGR-ccbc][[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9666984)]


## Othtrs
- Improving Continuous Sign Language Recognition with Cross-Lingual Signs
- SignVTCL: Multi-Modal Continuous Sign Language Recognition Enhanced by Visual-Textual Contrastive Learning

- Enhancing Sign Language Teaching: A Mixed Reality Approach for Immersive Learning and Multi-Dimensional Feedback.
- Improving Gloss-free Sign Language Translation by Reducing Representation Density
- Learning to Score Sign Language with Two-stage Method

---

# Reference
- [1] https://github.com/BenSaunders27/Awesome-SLP
- [2] https://github.com/VIPL-SLP/awesome-sign-language-processing
- [3] https://github.com/SignDiff/Processed-Data


