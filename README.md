# Awesome System for AI Resources
Here is a collection of valuable machine learning / deep learning resources, including courses, publications, and projects. Quick notes and highlights of the materials are annotated if possible. 

## Overview and principles 

- [CS 329S: Machine Learning Systems Design](https://stanford-cs329s.github.io/syllabus.html) (Stanford'21)
- [CS 294: Machine Learning Systems (Fall 2019)](https://ucbrise.github.io/cs294-ai-sys-fa19/) (UCBRISE'19)
- [EECS 598: Systems for AI (W'21)](https://github.com/mosharaf/eecs598/tree/w21-ai) (hosted by [Mosharaf Chowdhury](https://www.mosharaf.com/))
  > very good collections of concepts and key ideas (papers) of a wide area of this topic
## Deep Learning Compiling

### Kernel optimization and generation
- [**UNIT: Unifying Tensorized Instruction Compilation**](https://arxiv.org/abs/2101.08458) (CGO'21)
- [taco: A Tool to Generate Tensor Algebra Kernels](http://tensor-compiler.org/taco-tools.pdf) (ASE'17, [following works](http://tensor-compiler.org/publications.html), [code](https://github.com/tensor-compiler/taco))
- [**Sparse GPU Kernels for Deep Learning**](https://arxiv.org/abs/2006.10901) (SC20)
  > this paper presents practical and efficient techniques to optimize a general-purpose sparse kernel, esp. for SpMM.

### Related researchers
- [Tony Nowatzki](http://web.cs.ucla.edu/~tjn//03-publications/) (Assistant Professor of Computer Science @UCLA)

## Model Compression
It is important to reduce the redundance of the over-parameterized DNN models before real deployment. Pruning (structure or unstructured) and quantization are widely adopted compressing methods. There are actually two problems to address in this area, how to identify the redundance (algorithmic) and how to leverage the redundance to speedup (systemic).

### Surveys
- [MingSun-Tse/EfficientDNNs](https://github.com/MingSun-Tse/EfficientDNNs)
  > Collection of recent methods on DNN compression and acceleration
- [awesome-fast-attention](https://github.com/Separius/awesome-fast-attention)


### Compress transformers

- [Compressed Transformer](https://github.com/khakhulin/compressed-transformer)
- [**SpAtten: Efficient Sparse Attention Architecture with Cascade Token and Head Pruning**](https://spatten.mit.edu/) (HPCA'21) 
    > This paper talks about both *algorithmic optimization* and the *hardware architecture* fitted to it. The proposed algorithms includes pruning (Cascade Token/Head Pruning) and quantization (Progressive Quantization). 
### Recent works from [Song Han](https://songhan.mit.edu/)'s team

- [SpArch: Efficient Architecture for Sparse Matrix Multiplication](https://sparch.mit.edu/)(HPCA'20)
- [APQ: Joint Search for Network Architecture, Pruning and Quantization Policy](https://openaccess.thecvf.com/content_CVPR_2020/papers/Wang_APQ_Joint_Search_for_Network_Architecture_Pruning_and_Quantization_Policy_CVPR_2020_paper.pdf) (CVPR'20, [code](https://github.com/mit-han-lab/apq))
- [Once for All: Train One Network and Specialize it for Efficient Deployment](https://arxiv.org/abs/1908.09791) (ICLR'20, [code](https://github.com/mit-han-lab/once-for-all))
- [ProxylessNAS: Direct Neural Architecture Search on Target Task and Hardware](https://arxiv.org/pdf/1812.00332.pdf) (ICLR’19)
- [AMC: AutoML for Model Compression and Acceleration on Mobile Devices](https://arxiv.org/pdf/1802.03494.pdf) (ECCV’18)
- [HAQ: Hardware-Aware Automated Quantization](https://arxiv.org/pdf/1811.08886.pdf)  (CVPR’19, oral)
- [Defenstive Quantization: When Efficiency Meets Robustness](https://openreview.net/pdf?id=ryetZ20ctX) (ICLR'19)

## Machine Learning Systems in Wide
Building production level machine learning applications is much more than training a neural network model. This section collects the principles and methodologies as the technical / engineering guideline for it.

### Handbooks
- [Machine Learning Yearning](https://www.deeplearning.ai/programs/) ([chinese version](https://github.com/deeplearning-ai/machine-learning-yearning-cn))
- [Approaching (Almost) Any Machine Learning Problem](https://github.com/abhishekkrthakur/approachingalmost)
- [Machine Learning Engineering for Production (MLOps) Specialization](https://www.coursera.org/specializations/machine-learning-engineering-for-production-mlops) (Coursera by Andrew Ng, [talk](https://www.deeplearning.ai/wp-content/uploads/2021/06/MLOps-From-Model-centric-to-Data-centric-AI.pdf))

### Tools and best practices
- [EthicalML/awesome-production-machine-learning](https://github.com/EthicalML/awesome-production-machine-learning)
  > A curated list of awesome open source libraries to deploy, monitor, version and scale your machine learning
- [alirezadir/Production-Level-Deep-Learning](https://github.com/alirezadir/Production-Level-Deep-Learning)
  > A guideline for building practical production-level deep learning systems to be deployed in real world applications

### Blogs and articles
- [Machine learning system design](https://medium.com/acing-ai/machine-learning-system-design-c3a35c7df07d)
  > A primer for machine learning system design interviews published in [medium](medium.com). The author lists some valuable question to ask when designing a practical ML system.

## Carbon efficient AI

- [Energy and Policy Considerations for Deep Learning in NLP](https://arxiv.org/pdf/1906.02243.pdf)
  > it firstly reports that a single deep learning model can generate up to 626,155 pounds of CO2 emissions—roughly equal to the total lifetime carbon footprint of five cars
- [Green AI](https://arxiv.org/abs/1907.10597) 
- [ML CO2 Impact](https://mlco2.github.io/impact/)
