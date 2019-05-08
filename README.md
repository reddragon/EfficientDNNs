# EfficientDNNs
A collection of recent methods on DNN compression and acceleration. There are mainly 5 kinds of methods for efficient DNNs:
- neural architecture re-designing or searching
  - maintain accuracy, less cost (e.g., #Params, #FLOPs, etc.): MobileNet, ShuffleNet etc.
  - maintain cost, more accuracy: Inception, ResNeXt, Xception etc.
- pruning (including structured and unstructured)
- quantization
- matrix decomposition
- knowledge distillation

> About abbreviation: In the list below, `o` for oral, `w` for workshop, `s` for spotlight, `b` for best paper.

## Papers
- 2011-JMLR-[Learning with Structured Sparsity](http://www.jmlr.org/papers/v12/huang11b.html)
- 2013-NIPS-[Predicting Parameters in Deep Learning](http://papers.nips.cc/paper/5025-predicting-parameters-in-deep-learning)
- 2014-BMVC-[Speeding up convolutional neural networks with low rank expansions](https://arxiv.org/abs/1405.3866)
- 2014-NIPS-[Exploiting Linear Structure Within Convolutional Networks for Efficient Evaluation](http://papers.nips.cc/paper/5544-exploiting-linear-structure-within-convolutional-networks-for-efficient-evaluation)
- 2014-NIPS-[Do deep neural nets really need to be deep](http://papers.nips.cc/paper/5484-do-deep-nets-really-need-to-be-deep)
- 2015-ICML-[Compressing neural networks with the hashing trick](http://proceedings.mlr.press/v37/chenc15.pdf)
- 2015-INTERSPEECH-[A Diversity-Penalizing Ensemble Training Method for Deep Learning](https://www.isca-speech.org/archive/interspeech_2015/papers/i15_3590.pdf)
- 2015-BMVC-[Data-free parameter pruning for deep neural networks](https://arxiv.org/abs/1507.06149)
- 2015-NIPS-[Learning both Weights and Connections for Efficient Neural Network](http://papers.nips.cc/paper/5784-learning-both-weights-and-connections-for-efficient-neural-network)
- 2015_NIPSw-[Distilling Intractable Generative Models](http://homepages.inf.ed.ac.uk/s1459647/papers/distilling_generative_models.pdf)
- 2015-CVPR-[Efficient and Accurate Approximations of Nonlinear Convolutional Networks](https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Zhang_Efficient_and_Accurate_2015_CVPR_paper.html) [2016 TPAMI version: [Accelerating Very Deep Convolutional Networks for Classification and Detection](https://ieeexplore.ieee.org/abstract/document/7332968)]
- 2016-ICLRb-[Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding](https://arxiv.org/abs/1510.00149)
- 2016-ICLR-[All you need is a good init](https://arxiv.org/abs/1511.06422) [[Code](https://github.com/ducha-aiki/LSUVinit)]
- 2016-ICLR-[Convolutional neural networks with low-rank regularization](https://arxiv.org/abs/1511.06067)
- 2016-ICLR-[Diversity networks](https://pdfs.semanticscholar.org/3f08/1a7d2dbdcd10d71d0340721e4857a73ed7ee.pdf)
- 2016-EMNLP-[Sequence-Level Knowledge Distillation](https://arxiv.org/abs/1606.07947)
- 2016-CVPR-[Inverting Visual Representations with Convolutional Networks](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Dosovitskiy_Inverting_Visual_Representations_CVPR_2016_paper.html)
- 2016-NIPS-[Learning Structured Sparsity in Deep Neural Networks](http://papers.nips.cc/paper/6503-learning-structured-sparsity-in-deep-neural-networks)
- 2016-NIPS-[Dynamic Network Surgery for Efficient DNNs](http://papers.nips.cc/paper/6165-dynamic-network-surgery-for-efficient-dnns)
- 2016.10-[Deep model compression: Distilling knowledge from noisy teachers](https://arxiv.org/abs/1610.09650)
- 2017-ICLR-[Pruning Convolutional Neural Networks for Resource Efficient Inference](https://openreview.net/forum?id=SJGCiw5gl&noteId=SJGCiw5gl)
- 2017-ICLR-[Incremental Network Quantization: Towards Lossless CNNs with Low-Precision Weights](https://arxiv.org/abs/1702.03044)
- 2017-ICLR-[Do Deep Convolutional Nets Really Need to be Deep and Convolutional?](https://arxiv.org/abs/1603.05691)
- 2017-ICML-[Variational dropout sparsifies deep neural networks](https://arxiv.org/pdf/1701.05369.pdf)
- 2017-CVPR-[Learning deep CNN denoiser prior for image restoration](http://openaccess.thecvf.com/content_cvpr_2017/html/Zhang_Learning_Deep_CNN_CVPR_2017_paper.html)
- 2017-CVPR-[Deep roots: Improving cnn efficiency with hierarchical filter groups](http://openaccess.thecvf.com/content_cvpr_2017/html/Ioannou_Deep_Roots_Improving_CVPR_2017_paper.html)
- 2017-CVPR-[All You Need is Beyond a Good Init: Exploring Better Solution for Training Extremely Deep Convolutional Neural Networks with Orthonormality and Modulation](http://openaccess.thecvf.com/content_cvpr_2017/html/Xie_All_You_Need_CVPR_2017_paper.html)
- 2017-CVPR-ResNeXt-[Aggregated Residual Transformations for Deep Neural Networks](http://openaccess.thecvf.com/content_cvpr_2017/html/Xie_Aggregated_Residual_Transformations_CVPR_2017_paper.html)
- 2017-CVPR-[Xception: Deep learning with depthwise separable convolutions](http://openaccess.thecvf.com/content_cvpr_2017/html/Chollet_Xception_Deep_Learning_CVPR_2017_paper.html)
- 2017-ICCV-[Channel pruning for accelerating very deep neural networks](http://openaccess.thecvf.com/content_iccv_2017/html/He_Channel_Pruning_for_ICCV_2017_paper.html) [[Code](https://github.com/yihui-he/channel-pruning)]
- 2017-ICCV-[Learning efficient convolutional networks through network slimming](http://openaccess.thecvf.com/content_iccv_2017/html/Liu_Learning_Efficient_Convolutional_ICCV_2017_paper.html) [[Code](https://github.com/liuzhuang13/slimming/)]
- 2017-ICCV-[ThiNet: A filter level pruning method for deep neural network compression](http://openaccess.thecvf.com/content_iccv_2017/html/Luo_ThiNet_A_Filter_ICCV_2017_paper.html) [[Project](http://lamda.nju.edu.cn/luojh/project/ThiNet_ICCV17/ThiNet_ICCV17.html)]
- 2017-ICCV-[Interleaved group convolutions](http://openaccess.thecvf.com/content_iccv_2017/html/Zhang_Interleaved_Group_Convolutions_ICCV_2017_paper.html)
- 2017-NIPS-[Net-trim: Convex pruning of deep neural networks with performance guarantee](http://papers.nips.cc/paper/6910-net-trim-convex-pruning-of-deep-neural-networks-with-performance-guarantee)
- 2017-NIPS-[Learning to Prune Deep Neural Networks via Layer-wise Optimal Brain Surgeon](http://papers.nips.cc/paper/7071-learning-to-prune-deep-neural-networks-via-layer-wise-optimal-brain-surgeon)
- 2017-NNs-[Nonredundant sparse feature extraction using autoencoders with receptive fields clustering](https://www.sciencedirect.com/science/article/pii/S0893608017300928)
- 2017.02-[The Power of Sparsity in Convolutional Neural Networks](https://arxiv.org/abs/1702.06257)
- 2018-AAAI-[Auto-balanced Filter Pruning for Efficient Convolutional Neural Networks](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16450/16263)
- 2018-AAAI-[Deep Neural Network Compression with Single and Multiple Level Quantization](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16479/16742)
- 2018-ICML-[On the Optimization of Deep Networks: Implicit Acceleration by Overparameterization](https://arxiv.org/abs/1802.06509)
- 2018-ICMLw-[Assessing the Scalability of Biologically-Motivated Deep Learning Algorithms and Architectures](https://openreview.net/forum?id=SyPicjbWQ)
- 2018-ICLRo-[Training and Inference with Integers in Deep Neural Networks](https://openreview.net/forum?id=HJGXzmspb)
- 2018-ICLR-[Rethinking the Smaller-Norm-Less-Informative Assumption in Channel Pruning of Convolution Layers](https://openreview.net/forum?id=HJ94fqApW)
- 2018-ICLR-[N2N learning: Network to Network Compression via Policy Gradient Reinforcement Learning](https://openreview.net/forum?id=B1hcZZ-AW)
- 2018-ICLR-[Model compression via distillation and quantization](https://openreview.net/forum?id=S1XolQbRW)
- 2018-ICLR-[Towards Image Understanding from Deep Compression Without Decoding](https://openreview.net/forum?id=HkXWCMbRW)
- 2018-ICLR-[Deep Gradient Compression: Reducing the Communication Bandwidth for Distributed Training](https://openreview.net/forum?id=SkhQHMW0W)
- 2018-ICLR-[Mixed Precision Training of Convolutional Neural Networks using Integer Operations](https://openreview.net/forum?id=H135uzZ0-)
- 2018-ICLR-[Apprentice: Using Knowledge Distillation Techniques To Improve Low-Precision Network Accuracy](https://openreview.net/forum?id=B1ae1lZRb)
- 2018-ICLR-[Loss-aware Weight Quantization of Deep Networks](https://openreview.net/forum?id=BkrSv0lA-)
- 2018-ICLR-[Alternating Multi-bit Quantization for Recurrent Neural Networks](https://openreview.net/forum?id=S19dR9x0b)
- 2018-ICLR-[Adaptive Quantization of Neural Networks](https://openreview.net/forum?id=SyOK1Sg0W)
- 2018-ICLR-[Variational Network Quantization](https://openreview.net/forum?id=ry-TW-WAb)
- 2018-ICLR-[Learning Sparse Neural Networks through L0 Regularization](https://arxiv.org/abs/1712.01312)
- 2018-ICLR-[Efficient sparse-winograd convolutional neural networks](https://arxiv.org/pdf/1802.06367.pdf)
- 2018-ICLRw-[To Prune, or Not to Prune: Exploring the Efficacy of Pruning for Model Compression](https://openreview.net/forum?id=Sy1iIDkPM) (Similar topic: [2018-NIPSw-nip in the bud](https://openreview.net/forum?id=r1lbgwFj5m), [2018-NIPSw-rethink](https://openreview.net/forum?id=r1eLk2mKiX))
- 2018-ICLRw-[Systematic Weight Pruning of DNNs using Alternating Direction Method of Multipliers](https://openreview.net/forum?id=B1_u3cRUG)
- 2018-ICLRw-[Weightless: Lossy weight encoding for deep neural network compression](https://openreview.net/forum?id=rJpXxgaIG)
- 2018-ICLRw-[Variance-based Gradient Compression for Efficient Distributed Deep Learning](https://openreview.net/forum?id=Sy6hd7kvM)
- 2018-ICLRw-[Stacked Filters Stationary Flow For Hardware-Oriented Acceleration Of Deep Convolutional Neural Networks](https://openreview.net/forum?id=HkeAoQQHM)
- 2018-ICLRw-[Training Shallow and Thin Networks for Acceleration via Knowledge Distillation with Conditional Adversarial Networks](https://openreview.net/forum?id=BJbtuRRLM)
- 2018-ICLRw-[Accelerating Neural Architecture Search using Performance Prediction](https://openreview.net/forum?id=HJqk3N1vG)
- 2018-ICLRw-[Nonlinear Acceleration of CNNs](https://openreview.net/forum?id=HkNpF_kDM)
- 2018-CVPR-[Context-Aware Deep Feature Compression for High-Speed Visual Tracking](http://openaccess.thecvf.com/content_cvpr_2018/papers/Choi_Context-Aware_Deep_Feature_CVPR_2018_paper.pdf)
- 2018-CVPR-[NISP: Pruning Networks using Neuron Importance Score Propagation](https://arxiv.org/pdf/1711.05908.pdf)
- 2018-CVPR-[“Learning-Compression” Algorithms for Neural Net Pruning](http://openaccess.thecvf.com/content_cvpr_2018/html/Carreira-Perpinan_Learning-Compression_Algorithms_for_CVPR_2018_paper.html)
- 2018-CVPR-[Deep Image Prior](http://openaccess.thecvf.com/content_cvpr_2018/html/Ulyanov_Deep_Image_Prior_CVPR_2018_paper.html) [[Code](https://dmitryulyanov.github.io/deep_image_prior)]
- 2018-CVPR-[Condensenet: An efficient densenet using learned group convolutions](http://openaccess.thecvf.com/content_cvpr_2018/html/Huang_CondenseNet_An_Efficient_CVPR_2018_paper.html)
- 2018-CVPR-[Shift: A zero flop, zero parameter alternative to spatial convolutions](http://openaccess.thecvf.com/content_cvpr_2018/html/Wu_Shift_A_Zero_CVPR_2018_paper.html)
- 2018-CVPR-[Interleaved structured sparse convolutional neural networks](http://openaccess.thecvf.com/content_cvpr_2018/html/Xie_Interleaved_Structured_Sparse_CVPR_2018_paper.html)
- 2018-IJCAI-[Efficient DNN Neuron Pruning by Minimizing Layer-wise Nonlinear Reconstruction Error](https://www.ijcai.org/proceedings/2018/0318.pdf)
- 2018-IJCAI-[Soft Filter Pruning for Accelerating Deep Convolutional Neural Networks](https://arxiv.org/abs/1808.06866)
- 2018-IJCAI-[Where to Prune: Using LSTM to Guide End-to-end Pruning](https://www.ijcai.org/proceedings/2018/0445.pdf)
- 2018-IJCAI-[Accelerating Convolutional Networks via Global & Dynamic Filter Pruning](https://www.ijcai.org/proceedings/2018/0336.pdf)
- 2018-IJCAI-[Optimization based Layer-wise Magnitude-based Pruning for DNN Compression](http://staff.ustc.edu.cn/~chaoqian/ijcai18-olmp.pdf)
- 2018-IJCAI-[Progressive Blockwise Knowledge Distillation for Neural Network Acceleration](https://www.ijcai.org/proceedings/2018/0384.pdf)
- 2018-IJCAI-[Complementary Binary Quantization for Joint Multiple Indexing](https://www.ijcai.org/proceedings/2018/0292.pdf)
- 2018-ECCV-[A Systematic DNN Weight Pruning Framework using Alternating Direction Method of Multipliers](http://openaccess.thecvf.com/content_ECCV_2018/papers/Tianyun_Zhang_A_Systematic_DNN_ECCV_2018_paper.pdf)
- 2018-ECCV-[Coreset-Based Neural Network Compression](http://openaccess.thecvf.com/content_ECCV_2018/papers/Abhimanyu_Dubey_Coreset-Based_Convolutional_Neural_ECCV_2018_paper.pdf)
- 2018-ECCV-[Data-Driven Sparse Structure Selection for Deep Neural Networks](http://openaccess.thecvf.com/content_ECCV_2018/papers/Zehao_Huang_Data-Driven_Sparse_Structure_ECCV_2018_paper.pdf) [[Code](https://github.com/TuSimple/sparse-structure-selection)]
- 2018-BMVCo-[Structured Probabilistic Pruning for Convolutional Neural Network Acceleration](http://bmvc2018.org/contents/papers/0870.pdf)
- 2018-BMVC-[Efficient Progressive Neural Architecture Search](http://bmvc2018.org/contents/papers/0291.pdf)
- 2018-BMVC-[Igcv3: Interleaved lowrank group convolutions for efficient deep neural networks](https://arxiv.org/abs/1806.00178)
- 2018-NIPS-[Discrimination-aware Channel Pruning for Deep Neural Networks](http://papers.nips.cc/paper/7367-discrimination-aware-channel-pruning-for-deep-neural-networks.pdf)
- 2018-NIPS-[Frequency-Domain Dynamic Pruning for Convolutional Neural Networks](http://papers.nips.cc/paper/7382-frequency-domain-dynamic-pruning-for-convolutional-neural-networks.pdf)
- 2018-NIPS-[ChannelNets: Compact and Efficient Convolutional Neural Networks via Channel-Wise Convolutions](http://papers.nips.cc/paper/7766-channelnets-compact-and-efficient-convolutional-neural-networks-via-channel-wise-convolutions.pdf)
- 2018-NIPS-[DropBlock: A regularization method for convolutional networks](http://papers.nips.cc/paper/8271-dropblock-a-regularization-method-for-convolutional-networks)
- 2018-NIPS-[Constructing fast network through deconstruction of convolution](http://papers.nips.cc/paper/7835-constructing-fast-network-through-deconstruction-of-convolution)
- 2018-NIPS-[Learning Versatile Filters for Efficient Convolutional Neural Networks](https://papers.nips.cc/paper/7433-learning-versatile-filters-for-efficient-convolutional-neural-networks) [[Code](https://github.com/NoahEC/Versatile-Filters)]
- 2018-NIPSw-[Pruning neural networks: is it time to nip it in the bud?](https://openreview.net/forum?id=r1lbgwFj5m)
- 2018-NIPSwb-[Rethinking the Value of Network Pruning](https://openreview.net/forum?id=r1eLk2mKiX) [[2019 ICLR version](https://openreview.net/forum?id=rJlnB3C5Ym)]
- 2018-NIPSw-[Structured Pruning for Efficient ConvNets via Incremental Regularization](https://openreview.net/forum?id=S1e_xM7_iQ) [[2019 IJCNN version](https://arxiv.org/abs/1804.09461)]
- 2018-NIPSw-[Adaptive Mixture of Low-Rank Factorizations for Compact Neural Modeling](https://openreview.net/forum?id=B1eHgu-Fim)
- 2018.05-[Compression of Deep Convolutional Neural Networks under Joint Sparsity Constraints](https://arxiv.org/abs/1805.08303)
- 2018.05-[AutoPruner: An End-to-End Trainable Filter Pruning Method for Efficient Deep Model Inference](https://arxiv.org/abs/1805.08941)
- 2018.11-[Second-order Optimization Method for Large Mini-batch: Training ResNet-50 on ImageNet in 35 Epochs](https://arxiv.org/abs/1811.12019)
- 2018.11-[Rethinking ImageNet Pre-training](https://arxiv.org/abs/1811.08883) (Kaiming He)
- 2019-ICLR-[Defensive Quantization: When Efficiency Meets Robustness]()
- 2019-ICLR-[ProxylessNAS: Direct Neural Architecture Search on Target Task and Hardware]()
- 2019-ICLRo-[The Lottery Ticket Hypothesis: Finding Sparse, Trainable Neural Networks](https://openreview.net/forum?id=rJl-b3RcF7) (best paper!)
- 2019-AAAIo-[A layer decomposition-recomposition framework for neuron pruning towards accurate lightweight networks](https://arxiv.org/abs/1812.06611)
- 2019-CVPR-[All You Need is a Few Shifts: Designing Efficient Convolutional Neural Networks for Image Classification](https://arxiv.org/abs/1903.05285)
- 2019-CVPR-[HetConv Heterogeneous Kernel-Based Convolutions for Deep CNNs](https://arxiv.org/abs/1903.04120)
- 2019-CVPR-[Fully Learnable Group Convolution for Acceleration of Deep Neural Networks](https://arxiv.org/abs/1904.00346)
- 2019-CVPR-[Towards Optimal Structured CNN Pruning via Generative Adversarial Learning](https://arxiv.org/abs/1903.09291)
- 2019-CVPR-[Centripetal SGD for Pruning Very Deep Convolutional Networks with Complicated Structure](https://arxiv.org/abs/1904.03837)
- 2019-CVPRo-[HAQ: hardware-aware automated quantization](https://arxiv.org/pdf/1811.08886.pdf)
- 2019-
- 2019-BigComp-[Towards Robust Compressed Convolutional Neural Networks](https://ieeexplore.ieee.org/abstract/document/8679132)
- 2019-PR-[Filter-in-Filter: Improve CNNs in a Low-cost Way by Sharing Parameters among the Sub-filters of a Filter](https://www.sciencedirect.com/science/article/abs/pii/S0031320319300640)
- 2019-PRL-[BDNN: Binary Convolution Neural Networks for Fast Object Detection](https://www.sciencedirect.com/science/article/abs/pii/S0167865519301096)
- 2019.03-[MetaPruning: Meta Learning for Automatic Neural Network Channel Pruning](https://arxiv.org/abs/1903.10258) (Face++)
- 2019.04-[Data-Free Learning of Student Networks](https://arxiv.org/abs/1904.01186) (Huawei)
- 2019.04-[Resource Efficient 3D Convolutional Neural Networks](https://arxiv.org/abs/1904.02422)
- 2019.04-[Meta Filter Pruning to Accelerate Deep Convolutional Neural Networks](https://arxiv.org/abs/1904.03961)
- 2019.04-[Knowledge Squeezed Adversarial Network Compression](https://arxiv.org/abs/1904.05100)



### Papers-Arithmetic
- 2015-ICCV-[An Exploration of Parameter Redundancy in Deep Networks with Circulant Projections](https://www.cv-foundation.org/openaccess/content_iccv_2015/html/Cheng_An_Exploration_of_ICCV_2015_paper.html)
- 2017-ICCV-[Interleaved Group Convolutions for Deep Neural Networks](https://arxiv.org/abs/1707.02725)

### Papers-Advesarial Attacks
- 2019-CVPR-[ComDefend: An Efficient Image Compression Model to Defend Adversarial Examples](https://arxiv.org/abs/1811.12673) [[Code](https://github.com/jiaxiaojunQAQ/Comdefend)]

### Papers-Interpretability
- 2010-JMLR-[How to explain individual classification decisions](http://www.jmlr.org/papers/v11/baehrens10a.html)
- 2015-PLOS ONE-[On Pixel-Wise Explanations for Non-Linear Classifier Decisions by Layer-Wise Relevance Propagation](http://heatmapping.org/)
- 2015-CVPR-[Learning to generate chairs with convolutional neural networks](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Dosovitskiy_Learning_to_Generate_2015_CVPR_paper.pdf)
- 2015-CVPR-[Understanding deep image representations by inverting them](https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Mahendran_Understanding_Deep_Image_2015_CVPR_paper.html) [2016 IJCV version: [Visualizing deep convolutional neural networks using natural pre-images](https://link.springer.com/content/pdf/10.1007%2Fs11263-016-0911-8.pdf)]
- 2016-KDD-["Why Should I Trust You?": Explaining the Predictions of Any Classifier](https://arxiv.org/abs/1602.04938) (LIME)
- 2017-ICMLw-[The Mythos of Model Interpretability](https://arxiv.org/abs/1606.03490)
- 2017-DSP-[Methods for interpreting and understanding deep neural networks](https://arxiv.org/abs/1706.07979)
- 2018-ICML-[Interpretability Beyond Feature Attribution: Quantitative Testing with Concept Activation Vectors](https://arxiv.org/abs/1711.11279) (TCAV)
- 2018-NIPSs-[Sanity Checks for Saliency Maps](https://arxiv.org/abs/1810.03292)
- 2018-NIPSs-[Human-in-the-Loop Interpretability Prior](https://arxiv.org/abs/1805.11571)
- 2018-NIPS-[To Trust Or Not To Trust A Classifier](https://arxiv.org/abs/1805.11783) [[Code](https://github.com/google/TrustScore)]
- 2019-AISTATS-[Interpreting Black Box Predictions using Fisher Kernels](https://arxiv.org/abs/1810.10118)
- 2017-NIPSw-[The (Un)reliability of saliency methods](https://arxiv.org/abs/1711.00867)


### Papers-Knowledge Distillation
- 1996-[Born again trees](ftp://ftp.stat.berkeley.edu/pub/users/breiman/BAtrees.ps) (proposed compressing neural networks and multipletree predictors by approximating them with a single tree)
- 2006-SIGKDD-[Model compression](https://dl.acm.org/citation.cfm?id=1150464)
- 2010-ML-[A theory of learning from different domains](https://link.springer.com/content/pdf/10.1007%2Fs10994-009-5152-4.pdf)
- 2014-NIPS-[Do deep nets really need to be deep?](https://arxiv.org/abs/1312.6184)
- 2014-NIPSw-[Distilling the Knowledge in a Neural Network](https://arxiv.org/pdf/1503.02531.pdf) (coined the name "knowledge distillation" and "dark knowledge") [[Code](https://github.com/peterliht/knowledge-distillation-pytorch)]
- 2015-NIPS-[Bayesian dark knowledge](http://papers.nips.cc/paper/5965-bayesian-dark-knowledge.pdf)
- 2016-ICLR-[Net2net: Accelerating learning via knowledge transfer](https://arxiv.org/abs/1511.05641) (Tianqi Chen and Goodfellow)
- 2016-ECCV-[Accelerating convolutional neural networks with dominant convolutional kernel and knowledge pre-regression](https://www.researchgate.net/publication/308277663_Accelerating_Convolutional_Neural_Networks_with_Dominant_Convolutional_Kernel_and_Knowledge_Pre-regression)
- 2017-ICLR-[Paying more attention to attention: Improving the performance of convolutional neural networksvia attention transfer](http://arxiv.org/abs/1612.03928)
- 2017-ICLR-[Do deep convolutional nets really need to be deep and convolutional?](https://arxiv.org/pdf/1603.05691.pdf)
- 2017-CVPR-[A gift from knowledge distillation: Fast optimization, network minimization and transfer learning](http://openaccess.thecvf.com/content_cvpr_2017/papers/Yim_A_Gift_From_CVPR_2017_paper.pdf)
- 2017-NIPS-[Sobolev training for neural networks](http://papers.nips.cc/paper/7015-sobolev-training-for-neural-networks.pdf)
- 2017-NIPSw-[Data-Free Knowledge Distillation for Deep Neural Networks](https://arxiv.org/abs/1710.07535) [[Code](https://github.com/iRapha/replayed_distillation)]
- 2017.07-[Like What You Like: Knowledge Distill via Neuron Selectivity Transfer](https://arxiv.org/pdf/1707.01219.pdf)
- 2017.10-[Knowledge Projection for Deep Neural Networks](https://arxiv.org/abs/1710.09505)
- 2017.11-[Distilling a Neural Network Into a Soft Decision Tree](https://arxiv.org/abs/1711.09784)
- 2017.12-[Data Distillation: Towards Omni-Supervised Learning](https://arxiv.org/abs/1712.04440) (Kaiming He)
- 2018.03-[Interpreting Deep Classifier by Visual Distillation of Dark Knowledge](https://arxiv.org/abs/1803.04042)
- 2018.11-[Dataset Distillation](https://arxiv.org/abs/1811.10959) [[Code](https://github.com/SsnL/dataset-distillation)]
- 2018.12-[Learning Student Networks via Feature Embedding](https://arxiv.org/abs/1812.06597)
- 2018.12-[Few Sample Knowledge Distillation for Efficient Network Compression](https://arxiv.org/abs/1812.01839)
- 2018-AAAI-[DarkRank: Accelerating Deep Metric Learning via Cross Sample Similarities Transfer](https://arxiv.org/abs/1707.01220)
- 2018-ICML-[Born-Again Neural Networks](https://arxiv.org/pdf/1805.04770.pdf)
- 2018-NIPSw-[Transparent Model Distillation](https://arxiv.org/pdf/1801.08640.pdf)
- 2019-AAAI-[Knowledge Distillation with Adversarial Samples Supporting Decision Boundary](https://arxiv.org/abs/1805.05532)
- 2019-AAAI-[Knowledge Transfer via Distillation of Activation Boundaries Formed by Hidden Neurons](https://arxiv.org/abs/1811.03233)


## People (in alphabeta order)
- [Been Kim](https://beenkim.github.io/) @ Google Brain (Interpretability)
- [Elliot Crowley](http://homepages.inf.ed.ac.uk/ecrowley/) @ Edinburgh
- [Gao Huang](http://www.gaohuang.net/) @ Tsinghua
- [Mingjie Sun](https://scholar.google.com.vn/citations?user=XVvI7mAAAAAJ&hl=en&oi=ao) @ BUAA
- [Naiyan Wang](http://www.winsty.net/) @ TuSimple
- [Jianguo Li](https://sites.google.com/site/leeplus/) @ Intel
- [Miguel Carreira-Perpinan](https://scholar.google.com/citations?hl=en&user=SYdYhxgAAAAJ) @ UC Merced
- [Song Han](https://songhan.mit.edu/) @ MIT
- [Yang He](https://scholar.google.com.vn/citations?user=vvnFsIIAAAAJ&hl=en&oi=sra) @ University of Technology Sydney 
- [Yihui He](http://yihui-he.github.io/) @ CMU
- [Yunhe Wang](http://www.wangyunhe.site/) @ Huawei
- [Zhuang Liu](https://liuzhuang13.github.io/) @ UC Berkeley


## Venues
- [OpenReview](https://openreview.net/)
- [CVPR & ICCV](http://openaccess.thecvf.com/menu.py)
- [ECCV](https://link.springer.com/conference/eccv)
- [2017-ICML Tutorial](http://people.csail.mit.edu/beenkim/icml_tutorial.html): interpretable machine learning
- [2018-AAAI](https://aaai.org/Conferences/AAAI-18/wp-content/uploads/2017/12/AAAI-18-Accepted-Paper-List.Web_.pdf)
- [2018-ICLR](https://iclr.cc/Conferences/2018/Schedule)
- [2018-ICML](https://icml.cc/Conferences/2018/Schedule)
- [2018-ICML Workshop](https://openreview.net/group?id=ICML.cc/2018/ECA): Efficient Credit Assignment in Deep Learning and Reinforcement Learning
- [2018-IJCAI](https://www.ijcai-18.org/accepted-papers/)
- [2018-BMVC](http://bmvc2018.org/programmedetail.html)
- [2018-NIPS](https://nips.cc/Conferences/2018/Schedule)
- CDNNRIA workshop: Compact Deep Neural Network Representation with Industrial Applications [[1st: 2018 NIPSw](https://openreview.net/group?id=NIPS.cc/2018/Workshop/CDNNRIA)] [[2nd: 2019 ICMLw](https://sites.google.com/view/icml2019-on-device-compact-dnn)]
- LLD Workshop: Learning with Limited Data [[1st: 2017 NIPSw](https://lld-workshop.github.io/2017/)] [[2nd: 2019 ICLRw](https://lld-workshop.github.io/)]
- WHI: Worshop on Human Interpretability in Machine Learning [[1st: 2016 ICMLw](https://sites.google.com/site/2016whi/)] [[2nd: 2017 ICMLw](https://sites.google.com/view/whi2017/home)] [[3rd: 2018 ICMLw](https://sites.google.com/view/whi2018)]
- 


## News
- [VALSE 2018年度进展报告 | 深度神经网络加速与压缩 (in Chinese)](https://mp.weixin.qq.com/s?__biz=MzIxOTczOTM4NA==&mid=2247485375&idx=1&sn=a066fe6f57e6d152719b8815af87e819&chksm=97d7e228a0a06b3e5be18face8716e1ad41d598c2676429a1d174659a384e5f0d5a9be2204ee#rd)
- [机器之心-腾讯AI Lab PocketFlow (in Chinese)](https://www.jiqizhixin.com/articles/2018-09-17-6)
- [阿里开源首个移动AI项目，淘宝同款推理引擎 (in Chinese)](https://mp.weixin.qq.com/s/5lfXehtK3VPlB6Ex2KdTDw)
- [精度无损，体积压缩70%以上，百度PaddleSlim为你的模型瘦身 (in Chinese)](https://mp.weixin.qq.com/s/oJr5fx6uF5rsguK2rOpVoQ). Its [github project](https://github.com/PaddlePaddle/models/tree/v1.4/PaddleSlim).