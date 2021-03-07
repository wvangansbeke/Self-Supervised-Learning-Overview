# Self-Supervised Learning

This repo contains a curated list of self-supervised learning papers with a focus on representation learning and clustering.

## Table of Contents
- [Representation Learning](#representation-learning)
  - [Analysis](#analysis)
  - [Image-Level Representations](#image-level-representation-learning)
    - [Contrastive Learning](#contrastive-learning)
    - [Proxy tasks](#proxy-tasks)
    - [Clustering](#clustering)
  - [Dense-Level Representations](#dense-level-representation-learning)
- [Image Clustering](#image-clustering)
- [Geometry](#geometry)
  
## Representation Learning

### Analysis

- R. Geirhos, K. Narayanappa, B. Mitzkus, M. Bethge, F. A. Wichmann, W. Brendel, *[On the surprising similarities between supervised and self-supervised models](https://arxiv.org/abs/2010.08377)*, ICLR, 2021.
- X. Liu, F. Zhang, Z. Hou, L. Mian, Z. Wang, J. Zhang, J. Tang, *[Self-supervised Learning: Generative or Contrastive](https://arxiv.org/abs/2006.08218v4)*, Arxiv, 2020.
- L. Jing, Y. Tian, *[Self-supervised Visual Feature Learning with Deep Neural Networks: A Survey](https://arxiv.org/abs/1902.06162)*, T-PAMI, 2020.
- S. Purushwalkam, A. Gupta, *[Demystifying Contrastive Self-Supervised Learning: Invariances, Augmentations and Dataset Biases](https://arxiv.org/abs/2007.13916)*, NIPS, 2020. 
- Alejandro Newell, Jia Deng, *[How Useful is Self-Supervised Pretraining for Visual Tasks?](https://arxiv.org/abs/2003.14323)*, CVPR, 2020. [[Code](https://github.com/princeton-vl/selfstudy-render)]
- Y. M. Asano, C. Rupprecht, A. Vedaldi, *[A critical analysis of self-supervision, or what we can learn from a single image](https://arxiv.org/abs/1904.13132)*, ICLR, 2020. [[Code](https://github.com/yukimasano/linear-probes)]


### Image-Level Representation Learning

#### Contrastive Learning 

- X. Chen, K. He, *[Exploring Simple Siamese Representation Learning](https://arxiv.org/pdf/2011.10566)*, Arxiv, 2020. 
- J. Grill, F. Strub, F. Altché, C. Tallec, P. H. Richemond, E. Buchatskaya, C. Doersch, B. A. Pires, Z. Guo, M. G. Azar, B. Piot, K. Kavukcuoglu, R. Munos, M. Valko, *[Bootstrap Your Own Latent: A New Approach to Self-Supervised Learning](https://arxiv.org/abs/2006.07733)*, NIPS, 2020. [[Code](https://github.com/deepmind/deepmind-research/tree/master/byol)]
- T. Chen, S. Kornblith, M. Norouzi, G. Hinton, *[A Simple Framework for Contrastive Learning of Visual Representations](https://arxiv.org/abs/2002.05709)*, ICML, 2020. [[Code](https://github.com/google-research/simclr)]
- M. Tschannen, J. Djolonga, P. K. Rubenstein, S. Gelly, M. Lucic, *[On Mutual Information Maximization for Representation Learning](https://arxiv.org/pdf/1907.13625.pdf)*, ICLR, 2020. [[Code](https://github.com/google-research/google-research/tree/master/mutual_information_representation_learning)]
- Y. Tian, D. Krishnan, P. Isola, *[Contrastive Multiview Coding](https://arxiv.org/abs/1906.05849)*, ECCV, 2020. [[Code](https://github.com/HobbitLong/CMC/)]
- K. He, H. Fan, Y. Wu, S. Xie, R. Girshick, *[Momentum Contrast for Unsupervised Visual Representation Learning](https://arxiv.org/pdf/1911.05722.pdf)*, CVPR, 2020. [[Code](https://github.com/facebookresearch/moco)]
- I. Misra, L. Maaten, *[Self-Supervised Learning of Pretext-Invariant Representations](https://arxiv.org/abs/1912.01991)*, CVPR, 2020.
- O. Henaff, A. Razavi, C. Doersch, S. Eslami, A. Oord, *[Data-Efficient Image Recognition with Contrastive Predictive Coding](https://arxiv.org/abs/1905.09272)*, ICML, 2020.
- P. Bachman, R. D. Hjelm, W. Buchwalter, *[Learning Representations by Maximizing Mutual Information Across Views](https://arxiv.org/pdf/1906.00910)*, NIPS, 2019. [[Code](https://github.com/Philip-Bachman/amdim-public)]
- R. D. Hjelm, A. Fedorov, S. Lavoie-Marchildon, K. Grewal, P. Bachman, A. Trischler, Y. Bengio, *[Learning deep representations by mutual information estimation and maximization](https://arxiv.org/abs/1808.06670)*, ICLR, 2019. [[Code](https://github.com/rdevon/DIM)]
- J. Huang, Q. Dong, S. Gong, X. Zhu, *[Unsupervised Deep Learning by Neighbourhood Discovery](http://proceedings.mlr.press/v97/huang19b.html)*, ICML, 2019. [[Code](https://github.com/Raymond-sci/AND)] 
- A. Oord, Y. Li, O. Vinyals, *[Representation Learning with Contrastive Predictive Coding](https://arxiv.org/abs/1807.03748)*, Arxiv, 2018.
- Z. Wu, Y. Xiong and X. Y. Stella, D. Lin, *[Unsupervised Feature Learning via Non-parameteric Instance Discrimination](https://arxiv.org/pdf/1805.01978.pdf)*, CVPR, 2018. [[Code](https://github.com/zhirongw/lemniscate.pytorch)]
- Wang, Xiaolong and He, Kaiming and Gupta, Abhinav, *[Transitive Invariance for Self-supervised Visual Representation Learning](https://arxiv.org/pdf/1708.02901.pdf)*, ICCV, 2017.
- Li, Dong and Hung, Wei-Chih and Huang, Jia-Bin and Wang, Shengjin and Ahuja, Narendra and Yang, Ming-Hsuan, *[Unsupervised Visual Representation Learning by Graph-based Consistent Constraints](http://faculty.ucmerced.edu/mhyang/papers/eccv16_feature_learning.pdf)*, ECCV, 2016. [[Code](https://github.com/dongli12/FeatureLearning)]


#### Clustering

- M. Caron, I. Misra, J. Mairal, P. Goyal, P. Bojanowski, A. Joulin, *[Unsupervised Learning of Visual Features by Contrasting Cluster Assignments](https://arxiv.org/abs/2006.09882)*, NIPS, 2020. [[Code](https://github.com/facebookresearch/swav)]
- Y. M. Asano, C. Rupprecht, A. Vedaldi, *[Self-labelling via simultaneous clustering and representation learning](https://arxiv.org/abs/1911.05371)*, ICLR, 2020. [[Code](https://github.com/yukimasano/self-label)]
- X. Yan, I. Misra, A. Gupta, D. Ghadiyaram, D. Mahajan, *[ClusterFit: Improving Generalization of Visual Representations](https://arxiv.org/abs/1912.03330)*, CVPR, 2020.
- M. Caron, P. Bojanowski, J. Mairal, A. Joulin, *[Unsupervised Pre-Training of Image Features on Non-Curated Data](https://arxiv.org/pdf/1905.01278.pdf)*, ICCV, 2019. [[Code](https://github.com/facebookresearch/DeeperCluster)]    
- M. Caron, P. Bojanowski, A. Joulin, M. Douze, *[Deep Clustering for Unsupervised Learning of Visual Features](https://research.fb.com/wp-content/uploads/2018/09/Deep-Clustering-for-Unsupervised-Learning-of-Visual-Features.pdf)*, ECCV, 2018. [[Code](https://github.com/facebookresearch/deepcluster)]
- J. Yang, D. Parikh, D. Batra, *[Joint Unsupervised Learning of Deep Representations and Image Clusters](https://arxiv.org/pdf/1604.03628.pdf)*, CVPR, 2016. [[Code](https://github.com/jwyang/JULE.torch)]
- J. Xie, R. Girshick, A. Farhadi, *[Unsupervised Deep Embedding for Clustering Analysis](https://arxiv.org/pdf/1511.06335.pdf)*, ICML, 2016. [[Code](https://github.com/piiswrong/dec)]

#### Proxy Tasks
  
- X. Zhan, X. Pan, Z. Liu, D. Lin, C. C. Loy, *[Self-Supervised Learning via Conditional Motion Propagation](<https://arxiv.org/abs/1903.11412>)*, CVPR, 2019. [[Code](https://github.com/XiaohangZhan/conditional-motion-propagation)]
- Z. Feng, C. Xu, D. Tao, *[Self-Supervised Representation Learning by Rotation Feature Decoupling](http://openaccess.thecvf.com/content_CVPR_2019/html/Feng_Self-Supervised_Representation_Learning_by_Rotation_Feature_Decoupling_CVPR_2019_paper.html)*, CVPR, 2019. [[Code](https://github.com/philiptheother/FeatureDecoupling)]
- A. Kolesnikov, X. Zhai, L. Beye, *[Revisiting Self-Supervised Visual Representation Learning](https://arxiv.org/abs/1901.09005)*, CVPR, 2019. [[Code](https://github.com/google/revisiting-self-supervised)]
- T. Chen, X. Zhai, M. Ritter, M. Lucic, N. Houlsby, *[Self-Supervised GANs via Auxiliary Rotation Loss](https://openaccess.thecvf.com/content_CVPR_2019/papers/Chen_Self-Supervised_GANs_via_Auxiliary_Rotation_Loss_CVPR_2019_paper.pdf)*, CVPR, 2019. [[Code](https://github.com/vandit15/Self-Supervised-Gans-Pytorch)]
- L. Zhang, G. Qi, L. Wang, J. Luo, *[AET vs. AED: Unsupervised Representation Learning by Auto-Encoding Transformations rather than Data](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_AET_vs._AED_Unsupervised_Representation_Learning_by_Auto-Encoding_Transformations_Rather_CVPR_2019_paper.pdf)*, CVPR, 2019. [[Code](https://github.com/maple-research-lab/AET)] 
- X. Zhai, A. Oliver, A. Kolesnikov, L. Beyer, *[S4L: Self-Supervised Semi-Supervised Learning](https://openaccess.thecvf.com/content_ICCV_2019/papers/Zhai_S4L_Self-Supervised_Semi-Supervised_Learning_ICCV_2019_paper.pdf)*, ICCV, 2019. [[Code](https://github.com/google-research/s4l)]    
- S. Gidaris, P. Singh, N. Komodakis, *[Unsupervised Representation Learning by Predicting Image Rotations](https://openreview.net/forum?id=S1v4N2l0)*, ICLR, 2018 [[Code](https://github.com/gidariss/FeatureLearningRotNet)]    
- S. Jenni, P. Favaro, *[Self-Supervised Feature Learning by Learning to Spot Artifacts](https://arxiv.org/pdf/1806.05024.pdf)*, CVPR, 2018. [[Code](https://github.com/sjenni/LearningToSpotArtifacts)]
- M. Noroozi, A. Vinjimoor, P. Favaro, H. Pirsiavash, *[Boosting Self-Supervised Learning via Knowledge Transfer](https://www.csee.umbc.edu/~hpirsiav/papers/transfer_cvpr18.pdf)*, CVPR, 2018.
- A. Mahendran, J. Thewlis, A. Vedaldi, *[Cross Pixel Optical-Flow Similarity for Self-Supervised Learning](http://www.robots.ox.ac.uk/~vgg/publications/2018/Mahendran18/mahendran18.pdf)*, ACCV, 2018.
- M. Noroozi, H. Pirsiavash, P. Favaro, *[Representation Learning by Learning to Count](https://arxiv.org/abs/1708.06734)*, ICCV, 2017. [[Code](https://github.com/clvrai/Representation-Learning-by-Learning-to-Count)]
- R. Zhang, P. Isola, A. Efros, *[Split-Brain Autoencoders: Unsupervised Learning by Cross-Channel Prediction](https://arxiv.org/abs/1611.09842)*, CVPR, 2017. [[Code](https://github.com/richzhang/splitbrainauto)]
- D. Pathak, R. Girshick, P. Dollar, T. Darrell, B. Hariharan, *[Learning Features by Watching Objects Move](https://people.eecs.berkeley.edu/~pathak/papers/cvpr17.pdf)*, CVPR, 2017. [[Code](https://people.eecs.berkeley.edu/~pathak/unsupervised_video/)] 
- G. Larsson, M. Maire, G. Shakhnarovich, *[Colorization as a Proxy Task for Visual Understanding](http://arxiv.org/abs/1703.04044)*, CVPR, 2017. [[Code](http://people.cs.uchicago.edu/~larsson/color-proxy/)]
- R. S. Cruz, B. Fernando, A. Cherian, S. Gould, *[DeepPermNet: Visual Permutation Learning](https://arxiv.org/pdf/1704.02729.pdf)*, CVPR, 2017. [[Code](https://github.com/rfsantacruz/deep-perm-net)]
- R. Zhang, P. Isola, A. Efros, *[Split-Brain Autoencoders: Unsupervised Learning by Cross-Channel Prediction](https://arxiv.org/abs/1611.09842)*, CVPR, 2017. [[Code](https://github.com/richzhang/splitbrainauto)]
- H. Lee, J. Huang, M. K. Singh, M. Yang, *[Unsupervised Representation Learning by Sorting Sequences](https://arxiv.org/pdf/1708.01246.pdf)*, ICCV, 2017. [[Code](https://github.com/HsinYingLee/OPN)]
- P. Bojanowski, A. Joulin, *[Unsupervised Learning by Predicting Noise](https://arxiv.org/abs/1704.05310)*, ICML, 2017.  [[Code](https://github.com/facebookresearch/noise-as-targets)]
- M. Noroozi, P. Favaro, *[Unsupervised Learning of Visual Representations by Solving Jigsaw Puzzles](http://arxiv.org/abs/1603.09246)*, ECCV, 2016.
  [[Code](http://www.cvg.unibe.ch/research/JigsawPuzzleSolver.html)]
- G. Larsson, M. Maire, G. Shakhnarovich, *[Learning Representations for Automatic Colorization](http://arxiv.org/pdf/1603.06668.pdf)*, ECCV, 2016. [[Code](http://people.cs.uchicago.edu/~larsson/colorization/)]
- R. Zhang, P. Isola, A. Efros, *[Colorful Image Colorization](https://arxiv.org/abs/1603.08511)*, ECCV, 2016. [[Code](http://richzhang.github.io/colorization/)]
- D. Pathak, P. Krahenbuhl, J. Donahue, T. Darrell, A. Efros, *[Context Encoders: Feature Learning by Inpainting](https://people.eecs.berkeley.edu/~pathak/papers/cvpr16.pdf)*, CVPR, 2016. [[Code](https://people.eecs.berkeley.edu/~pathak/context_encoder/)]
- P. Agrawal, J. Carreira, J. Malik, *[Learning to See by Moving](http://arxiv.org/abs/1505.01596)*, ICCV, 2015. [[Code](https://people.eecs.berkeley.edu/~pulkitag/lsm/lsm.html)]
- C. Doersch, A. Gupta, A. Efros, *[Unsupervised Visual Representation Learning by Context Prediction](https://arxiv.org/abs/1505.05192)*, ICCV, 2015. [[Code](http://graphics.cs.cmu.edu/projects/deepContext/)]

### Dense-Level Representation Learning
- W. Van Gansbeke, S. Vandenhende, S. Georgoulis, L. Van Gool, *[Unsupervised Semantic Segmentation by Contrasting Object Mask Proposals]()*, Arxiv, 2021. [[Code](https://github.com/wvangansbeke/Unsupervised-Semantic-Segmentation)]
- X. Wang, R. Zhang, C. Shen, T. Kong, L. Li, *[Dense Contrastive Learning for Self-Supervised Visual Pre-Training](https://arxiv.org/abs/2011.09157)*, Arxiv, 2020.
- Z. Xie, Y. Lin, Z. Zhang, Y. Cao, S. Lin, H. Hu, *[Propagate Yourself: Exploring Pixel-Level Consistency for Unsupervised Visual Representation Learning](https://arxiv.org/abs/2011.10043)*, Arxiv, 2020. [[Code](https://github.com/lucidrains/pixel-level-contrastive-learning)]
- A. Jabri, A, Owens, A. Efros, *[Space-Time Correspondence as a Contrastive Random Walk](https://arxiv.org/abs/2006.14613)*, NIPS, 2020. [[Code](https://github.com/ajabri/videowalk)]
- P. O. Pinheiro, A. Almahairi, R. Y. Benmalek, F. Golemo, A. Courville, *[Unsupervised Learning of Dense Visual Representations](https://arxiv.org/abs/2011.05499)*, NIPS, 2020. 
- X. Ji, J. F. Henriques, A. Vedaldi, *[Invariant Information Clustering for Unsupervised Image Classification and Segmentation](https://arxiv.org/abs/1807.06653)*, ICCV, 2019. [[Code](https://github.com/xu-ji/IIC)]
- X. Wang, A. Jabri, A. Efros. *[Learning Correspondence from the Cycle-Consistency of
Time](https://arxiv.org/abs/1903.07593)*, CVPR, 2019. [[Code](https://github.com/xiaolonw/TimeCycle)]
- T. Zhou, P. Krahenbuhl, M. Aubry, Q. Huang, A. Efros.*[Learning dense
correspondence via 3d-guided cycle consistency](https://arxiv.org/abs/1604.05383)*, CVPR, 2016.

## Image Clustering
- W. Van Gansbeke, S. Vandenhende, S. Georgoulis, M. Proesmans, L. Van Gool, *[SCAN: Learning to Classify Images without Labels](https://arxiv.org/abs/2005.12320)*, ECCV, 2020. [[Code](https://github.com/wvangansbeke/Unsupervised-Classification)]
- X. Ji, J. F. Henriques, A. Vedaldi, *[Invariant Information Clustering for Unsupervised Image Classification and Segmentation](https://arxiv.org/abs/1807.06653)*, ICCV, 2019. [[Code](https://github.com/xu-ji/IIC)]
- J. Chang, L. Wang, G. Meng, S. Xiang, C. Pan, *[Deep Adaptive Image Clustering](https://openaccess.thecvf.com/content_iccv_2017/html/Chang_Deep_Adaptive_Image_ICCV_2017_paper.html)*, ICCV, 2017. [[Code](https://github.com/vector-1127/DAC)]
- J. Yang, D. Parikh, D. Batra, *[Joint unsupervised learning of deep representations and image clusters](https://arxiv.org/abs/1604.03628)*, CVPR, 2016. [[Code](https://github.com/jwyang/JULE.torch)]
- J. Xie, R. Girshick, A. Farhadi, *[Unsupervised Deep Embedding for Clustering Analysis](https://arxiv.org/pdf/1511.06335.pdf)*, ICML, 2016. [[Code](https://github.com/piiswrong/dec)]

## Geometry
- C. Godard, O. M. Aodha, M. Firman, G. J. Brostow, *[Digging into Self-Supervised Monocular Depth Prediction](https://arxiv.org/abs/1806.01260)*, ICCV, 2019. [[Code](https://github.com/nianticlabs/monodepth2)]
- J. Wang, J. Jiao, L. Bao, S. He, Y. Liu, W. Liu, *[SelFlow: Self-Supervised Learning of Optical Flow](https://arxiv.org/abs/1904.09117)*, CVPR, 2019. [[Code](https://github.com/ppliuboy/SelFlow)]
- C. Godard, O. <. Aodha, G. J. Brostow, *[Unsupervised Monocular Depth Estimation with Left-Right Consistency](https://openaccess.thecvf.com/content_cvpr_2017/papers/Godard_Unsupervised_Monocular_Depth_CVPR_2017_paper.pdf)*, CVPR, 2017. [[Code](https://github.com/mrharicot/monodepth)]
- T. Zhou, M. Brown, N. Snavely, D. G. Lowe, *[Unsupervised Learning of Depth and Ego-Motion from Video](https://arxiv.org/abs/1704.07813)*, CVPR, 2017. [[Code](https://github.com/tinghuiz/SfMLearner)]
