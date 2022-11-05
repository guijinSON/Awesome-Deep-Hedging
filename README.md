# Awesome-Deep-Hedging
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)  
__A curated list of resources dedicated to Deep Hedging.__  

<img src="https://raw.githubusercontent.com/guijinSON/Awesome-Deep-Hedging/main/assets/logo.jpg" width="600">  

__Last Updated: 2021.12.27__
## Contents
* [Introduction to Deep Hedging](#introduction-to-deep-hedging)  
* [Curated Papers](#curated-papers)
    - [Sequence Modeling Approach](#sequence-modeling-approach)
    - [Reinforcement Learning Approach](#reinforcement-learning-approach)
    - [Others](#others)
* [Curated Github Repos & Blogs](#curated-github-repos)
* [Relavent Journals](#relavent-journals)

## Introduction to Deep Hedging
[Back to Top](#contents)  

Hedging refers to a risk managment strategy employed to minimize risk by taking adversial postions to a set asset. Commonly, hedging is adopted using derivatves such as options, swaps, futures and forward contracts. Though a vast majority of present-day hedging strategies still heavily rely on analytical methods, several recent works aim to outperform such traditional methods by leveraging ML/DL technologies. In this repository we provided a curated list of modern neural approaches to derivative hedging, also known as __Deep Hedging.__

The problem of hedging shows a highly nonlinear connection with various parameters such as volatility, time to maturity, interest rate, and asset price. As modern ML/DL technology have shown outstanding results in approximating nonlinear functions, ML/DL researchers are making effort to tackle the problem of hedging as well. However, at the best of our knowledge most deep hedging research use simulated data for both training and validation, which leaves a question: _Can ML/DL algorithms acquire knowledge in real-word hedging through fake data?_  
Which we hope to be resolved in future literatures. 

## Curated Papers
[Back to Top](#contents)
### Sequence Modeling Approach 

* [Deep Neural Network Framework Based on Backward Stochastic Differential Equations for Pricing and Hedging American Options in High Dimensions](https://arxiv.org/pdf/1909.11532v1.pdf)  
A chronological neural model for high-dimensional American option problems. The paper notes that their proposal outperforms the Longstaff-Schwartz algorithm when d ≥ 20.

* [Data-driven Hedging of Stock Index Options via Deep Learning](https://arxiv.org/pdf/2111.03477v1.pdf)  
This work leverage a sentiment score(VIX) and a GRU model to enhance the hedging capability of deep neural networks.

* [Neural Networks for Delta Hedging](https://arxiv.org/pdf/2112.10084.pdf)  
Preprint(Work in progress). Suggests that teaching neural networks about traditional hedging strategies prior to training with simulated data, helps to stabilize the training process and help them to generate deltas with better quality.

### Reinforcement Learning Approach
* [Deep Hedging of Derivatives Using Reinforcement Learning](https://arxiv.org/pdf/2103.16409.pdf)  
The paper demonstrates the production of an optimal hedging strategy when a particular stochastic process has been specified. Unlike past works the authors put great emphasis on accounting the impact of trading costs. 

* [Deep Hedging, Generative Adversarial Networks, and Beyond](https://arxiv.org/ftp/arxiv/papers/2103/2103.03913.pdf)  
The paper suggests a methodoloy to pair Generative Adversarial Networks(GAN) with RL-based hedging framweorks. Also, instead of using traditional methods to simulate data, the paper suggests that the usage of AI-based models may show better performance. 

* [Deep Hedging: Hedging Derivatives Under Generic Market Frictions Using Reinforcement Learning](https://smallake.kr/wp-content/uploads/2019/10/SSRN-id3355706.pdf)  
Work done by J.P Morgan. Though trained on simulated data it has been reported to help _"hedge ite exposures faster, and quote higher volumes as a result"_ according to [Beacon Platform](https://www.risk.net/derivatives/6691696/jp-morgan-turns-to-machine-learning-for-options-hedging). 

* [Reinforced learning for hedging: transfer learning at work](https://probability.nl/wp-content/uploads/2021/06/WP-Reinforced-learning-for-hedging-transfer-learning-at-work.pdf)   
A shortened version of [Giurca and Borovkova (2021)](https://www.semanticscholar.org/paper/Delta-Hedging-of-Derivatives-using-Deep-Learning-Giurca-Borovkova/e451a57d9d4213d14e9315cf4037adc655884bfd) which reports that knowledge acquired by training on simulated data can be transfered to real-time markets.  

* [Deep Hedging: Continuous Reinforcement Learning for Hedging of General Portfolios across Multiple Risk Aversions](https://arxiv.org/abs/2207.07467?context=stat.ML)  
Second work regarding deep hedging from J.P.Morgan. They present a method for finding optimal hedging policies for arbitrary initial portfolios and market states. The paper develop a novel actor-critic algorithm for solving general risk-averse stochastic control problems and use it to learn hedging strategies across multiple risk aversion levels simultaneously.

### Others
* [No-Transaction Band Network: A Neural Network Architecture for Efficient Deep Hedging](https://arxiv.org/pdf/2103.01775.pdf)  
This paper proposes _No-Transaction Band Strategy_ using the clamp function and reports to outperform vanilla linear models. 

* [Neural networks for option pricing and hedging: a literature review](http://eprints.lse.ac.uk/104341/1/Ruf_Wang_Literature_Review.pdf)  
A survey paper on deep hedging literatures. Provide comparison in terms of input features, output variables, benchmark models, performance measures, data partition methods, and underlying assets.

## Curated Github Repos 
[Back to Top](#contents)

- [YuMan-Tam/deep-hedging](https://github.com/YuMan-Tam/deep-hedging)  
  A TensorFlow implementation of deep hedging using simple neural networks. 
- [pfnet-research/NoTransactionBandNetwork](https://github.com/pfnet-research/notransactionbandnetwork)  
  A minimal implementation of _"No-Transaction Band Network: A Neural Network Architecture for Efficient Deep Hedging"_
- [pfnet-research/pfhedge](https://github.com/pfnet-research/pfhedge)  
  PyTorch based framework for hedging financial derivatives which provide a diverse set of models and instrunments. Well integrated with PyTorch and supports effortless extensions.
  
### Relavent Journals
* [International Journal of Financial Markets and Derivatives](https://www.inderscience.com/jhome.php?jcode=ijfmd#:~:text=IJFMD%20addresses%20the%20advancement%20of,of%20international%20markets%20and%20derivatives.)
* [Intelligent Systems in Accounting, Finance & Management](https://onlinelibrary.wiley.com/journal/21600074)
* [Physica A: Statistical Mechanics and its Applications](https://www.journals.elsevier.com/physica-a-statistical-mechanics-and-its-applications)
* [Expert Systems with Applications](https://www.journals.elsevier.com/expert-systems-with-applications)
* [Quantitative Finance](https://www.tandfonline.com/journals/rquf20?gclid=Cj0KCQiAwqCOBhCdARIsAEPyW9lBT2BmuXeWnWSp-tSCcoAsFDhqabqgh35kTC3U_3keqgmbtarm_3YaAj6HEALw_wcB&)
* [International Journal of Theoretical and Applied Finance](https://www.worldscientific.com/worldscinet/ijtaf)
