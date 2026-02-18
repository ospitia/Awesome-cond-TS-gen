# Awesome Conditioned Time Series Generation
[![Awesome Lists](https://srv-cdn.himpfen.io/badges/awesome-lists/awesomelists-flat.svg)]()
[![Paper Count](https://img.shields.io/badge/Papers-19-blue)]()
[![Dataset Count](https://img.shields.io/badge/Datasets-31-blue)]()

> A curated list of resources for conditioned time series generation 
> focused on probabilistic approaches and real applications.

## keywords
- *Conditional TS generation*
- *Probabilistic TS generation*
- *TS imputation*


## Contents

- [Methods](#methods)
  - [GP-Based Models](#gp-based-models)
  - [Encoder-Decoder Based Models](#encoder-decoder-based-models)
  - [Diffusion-Based Models](#diffusion-based-models)
  - [Foundation/Generative Models](#foundationgenerative-models)
- [Applications](#applications)
  - [Healthcare & Medical](#healthcare--medical)
  - [Transportation & Traffic](#transportation--traffic)
  - [Industrial & IoT](#industrial--iot)
  - [Climate & Weather](#climate--weather)
  - [Aviation](#aviation)
- [Datasets](#datasets)
- [Evaluation metrics](#evaluation--metrics)
- [Related Awesome Lists](#related-awesome-lists)
- [License](#license)

## Methods

### GP-Based Models

Methods based on Gaussian Processes for modeling temporal dependencies and uncertainties.

- **[1] GP-VAE: Deep probabilistic time series imputation.**
  Fortuin, Vincent, et al. International Conference on Artificial Intelligence and Statistics. PMLR.  
  2020 | [Paper](https://proceedings.mlr.press/v108/fortuin20a/fortuin20a.pdf) | [Code](https://github.com/ratschlab/GP-VAE)  

- **[1b] Probabilistic imputation for time-series classification with missing data.** 
  Kim, SeungHyun, Hyunsu Kim, Eunggu Yun, Hwangrae Lee, Jaehun Lee, and Juho Lee.
  International Conference on Machine Learning, PMLR.  
  2023 | [Paper](https://proceedings.mlr.press/v202/kim23m/kim23m.pdf)

### Encoder-Decoder Based Models

Methods using encoder-decoder architectures, including transformers and VAEs.

- **[2] Heteroscedastic temporal variational autoencoder for irregularly sampled time series.**
  Shukla, Satya Narayan, and Benjamin Marlin. International Conference on Learning Representations. ICLR.  
  2022 | [Paper](https://openreview.net/pdf?id=Az7opqbQE-3) | [Code](https://github.com/reml-lab/hetvae)  


- **[3] Tripletformer for probabilistic interpolation of irregularly sampled time series.**
  Yalavarthi, Vijaya Krishna, Johannes Burchert, and Lars Schmidt-Thieme. IEEE International Conference on Big Data (BigData). IEEE.  
  2023 | [Paper](https://arxiv.org/pdf/2210.02091) | [Code](https://github.com/yalavarthivk/tripletformer)  


### Diffusion-Based Models

Methods leveraging diffusion models for conditional generation and imputation.

- **[4] CSDI: Conditional score-based diffusion models for probabilistic time series imputation.**
  Tashiro, Yusuke, Jiaming Song, Yang Song, and Stefano Ermon. Advances in Neural Information Processing Systems 34. NeurIPS.  
  2021 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2021/file/cfe8504bda37b575c70ee1a8276f3486-Paper.pdf) | [Code](https://github.com/ermongroup/CSDI)

- **[5] SSSD: Diffusion-based time series imputation and forecasting with structured state space models.**
  Lopez Alcaraz, Juan Miguel, and Nils Strodthoff. Transactions on Machine Learning Research.  
  2022 | [Paper](https://arxiv.org/abs/2208.09399) | [Code](https://github.com/AI4HealthUOL/SSSD)

- **[6] SSD-TS: Exploring the potential of linear state space models for diffusion models in time series imputation.**
  Gao, Hongfan, et al. Proceedings of the 31st ACM SIGKDD Conference on Knowledge Discovery and Data Mining.  
  2025 | [Paper](https://arxiv.org/abs/2410.13338) | [Code](https://github.com/decisionintelligence/SSD-TS)
### Foundation/Generative Models

Foundation models, flow-based models, and other generative approaches.

- **[7] Reconstructing dynamics from sparse observations with no training on target system.**
  Zhai, Z. M., Huang, J. Y., Stern, B. D., & Lai, Y. C. Nature Communications 16.1.  
  2024 | [Paper](https://www.nature.com/articles/s41467-025-63019-8) | [Code](https://github.com/Zheng-Meng/Dynamics-Reconstruction-ML)  

- **[8] FM-TS (FlowTS): Flow matching for time series generation.**
  Hu, Y., Wang, X., Wu, L., Zhang, H., Li, S. Z., Wang, S., & Chen, T.  
  2024 | [Paper](https://arxiv.org/abs/2411.07506) | [Code](https://github.com/UNITES-Lab/FlowTS)  

- **[9] NuwaTS: A foundation model mending every incomplete time series.**
  Cheng, Jinguo, et al. arXiv preprint arXiv:2405.15317.  
  2024 | [Paper](https://arxiv.org/abs/2405.15317) | [Code](https://github.com/Chengyui/NuwaTS)  

- **[10] Are time-indexed foundation models the future of time series imputation?**
  Le Naour, Etienne, et al. arXiv preprint arXiv:2511.05980.  
  2024 | [Paper](https://arxiv.org/abs/2511.05980)  

## Applications

Real-world applications of conditioned time series generation across various domains.

### Healthcare & Medical

- **[11] MED-Diffusion: Diffusion model-based imputation of multimodal sensor data for surgical patients.**
  Cheng, Z., Zhang, B., Hu, Y., Du, Y., Liu, T., Zhang, Z., ... & Cui, Z. Sensors.  
  2025 | [Paper](https://www.mdpi.com/1424-8220/25/19/6175)
  - *Method*: diffusion (Unet backbone) + tokenization
  - *Application*: Surgical patient monitoring with multimodal sensors

### Transportation & Traffic

- **[12] PMA-Diffusion: A physics-guided mask-aware diffusion framework for traffic state estimation from sparse observations.**
  Liu, Lindong, et al. arXiv preprint arXiv:2512.06183.  
  2025 | [Paper](https://arxiv.org/abs/2512.06183)

  - *Method*: Diffusion (UNet backbone) + constrained posterior sampling
  - *Application*: Highway traffic state estimation from sparse loop detector and probe vehicle data.

- **[13] Traffic state estimation from vehicle trajectories with anisotropic Gaussian processes.**
  Wu, F., Cheng, Z., Chen, H., Qiu, Z., & Sun, L. Transportation Research Part C: Emerging Technologies.  
  2024 | [Paper](https://www.sciencedirect.com/science/article/pii/S0968090X24001670) | [Code](https://github.com/Lucky-Fan/GP_TSE)  
  - *Method*: Gaussian process regression
  - *Application*: Reconstruct traffic state from sparse vehicle trajectories
 
### Industrial & IoT

- **[14] Lightweight window-portion-based multiple imputation for extreme missing gaps in IoT systems.**
  Adhikari, D., Jiang, W., Zhan, J., Assefa, M., Khorshidi, H. A., Aickelin, U., & Rawat, D. B. 
  IEEE Internet of Things Journal.
  - *Method*: Lightweight Gradient Boosting Machine (LGBM) regression.
  - *Application*: TS generation for extreme missing gaps (due to faulty sensors, unstable network communications, power failures, device failures, and network attacks) and high missing rates in data from IoT sensors.
  
  2024 | [Paper](https://ieeexplore.ieee.org/document/10250789)

- **[15] Blackout missing data recovery in industrial time series based on masked former hierarchical imputation framework.**
  Liu, D., Wang, Y., Liu, C., Wang, K., Yuan, X., & Yang, C. IEEE Transactions on Automation Science and Engineering.  
  2023 | [Paper](https://ieeexplore.ieee.org/abstract/document/10163894)
  - *Method*: Two-step encoder (conv-based sub-windows coarse, temporal-focused transformer encoding) with a reconstruction head.
  - *Application*: Industrial time series. Blackout missingness due to hardware failures, communication issues or maintenance downtime. 

- **[16] Quality aware industrial data imputation with self-supervised recovery for process soft sensor development.**
  Dai, Yun, Chao Yang, Kaixin Liu, Yi Liu, and Yuan Yao. Computers & Chemical Engineering.  
  - *Method*: adds losses to CSDI. CSDI imputes missing values and an LSTM module predicts quality variables from the reconstruction (supervised).
  - *Application*: Chemical manufacturing - soft sensor development - models to estimate quality variables like purity from available process data like temperature or pressure.
    
  2025 | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0098135425003308)

### Climate & Weather

- **[17] Generative data assimilation of sparse weather station observation at kilometre scales.**
  *Details to be added*  
  [Paper](#) | [Code](#)

### Aviation

- **[18] Deep generative modelling of aircraft trajectories in terminal manoeuvring areas.**
  Krauth, Timothé, Adrien Lafage, Jérôme Morio, Xavier Olive, and Manuel Waltert.
  Machine Learning with Applications.  
  2023 | [Paper](https://www.sciencedirect.com/science/article/pii/S2666827022001219) | [Code](https://github.com/kruuZHAW/deep-traffic-generation-paper)  
  - *Method*: VAE + Temporal convolutional networks (backbone) + Variational Mixture of Posteriors (VampPrior)
  - *Application*: Generate realistic aircraft trajectories in Terminal Manoeuvre Area with few observations available



## Datasets

A survey of datasets in conditioned time series generation research.

### Dataset Summary Table

| Domain | Dataset | Dimensions | Seq Length | Native Missing | Exp. Missing | Used in Papers | Download |
|--------|---------|------------|------------|----------------|--------------|----------------|----------|
| **Healthcare** | **PhysioNet 2012** | 35-42 | 48 | ~80% | 10-90% | [1,2,3,4,6,11] | [Link](https://physionet.org/content/challenge-2012/1.0.0/) |
| **Healthcare** | **PhysioNet 2019** | 40+ | 48-72 | High | 50-90% | [2] | [Link](https://physionet.org/content/challenge-2019/1.0.0/) |
| **Healthcare** | **MIMIC-III** | Many | Variable | High | Variable | [1b,2,3] | [Link](https://physionet.org/content/mimiciii/1.4/)* |
| **Healthcare** | **PTB-XL** | 12-lead ECG | 10s | 0% | Variable | [5] | Public ECG |
| **Healthcare** | **Indicators of Heart Disease** | Multiple | Variable | Varies | Variable | [11] | CDC/Kaggle |
| **Healthcare** | **Breast Cancer Wisconsin** | 30 features | Variable | Varies | Variable | [11] | UCI/Kaggle |
| **Healthcare** | **Diabetes Health Indicators** | Multiple | Variable | Varies | Variable | [11] | CDC/Kaggle |
| **Healthcare** | **COVID-19 Pre-condition** | Multiple | Variable | Varies | Variable | [11] | Public |
| **Healthcare** | **fMRI** | 50 | Variable | 0% | Variable | [8] | Simulated |
| **Energy** | **ETTh** | 7 | 48-256 | 0% | 10-90% | [8,9] | [Link](https://github.com/zhouhaoyi/ETDataset) |
| **Energy** | **ETTm1** | 7 | Variable | 0% | Variable | [5] | [Link](https://github.com/zhouhaoyi/ETDataset) |
| **Energy** | **Energy** | 28 | 48-256 | 0% | 10-90% | [8] | [Link](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction) |
| **Energy** | **ECL (Electricity)** | 321 | Hourly | 0% | Variable | [9] | Public |
| **Energy** | **Solar** | Multiple | 168+24 | 0% | Variable | [5,8] | NREL |
| **Traffic** | **PEMS-BAY** | 325 sensors | 5-min | Sparse | Variable | [5] | California |
| **Traffic** | **METR-LA** | 207 sensors | 5-min | Sparse | Variable | [5] | LA traffic |
| **Traffic** | **I-24 MOTION** | Grid | Spatial-temp | Sparse | 5-20% | [12] | [Link](https://i24motion.org/) |
| **Traffic** | **CARGO** | Freight | Variable | Sparse | Variable | [14] | Public |
| **Environment** | **Air Quality** | ~10 | Variable | ~13% | Blackout | [4,6] | [Link](https://dl.acm.org/doi/pdf/10.1145/2783258.2788573) |
| **Environment** | **AQS Data Sets** | Air quality | Variable | Varies | Variable | [14] | EPA |
| **Environment** | **Weather** | Multiple | Variable | 0% | Variable | [2,9] | Public |
| **Environment** | **Climate Records (NOAA)** | Multiple | Daily/Monthly | Varies | Variable | [2] | [Link](https://www.osti.gov/biblio/1394920) |
| **Activity** | **UCI Human Activity** | 9 | Variable | 0% | Variable | [1b,2] | [Link](https://archive.ics.uci.edu/dataset/196/localization+data+for+person+activity) |
| **Finance** | **Stocks** | 6 | 24-48 | 0% | 10-90% | [8] | In repos |
| **Synthetic** | **MuJoCo** | 14 | 100-200 | 0% | 70-90% | [5,6,8] | Simulator |
| **Synthetic** | **Sines** | 5 | 24-100 | 0% | Variable | [8] | Generated |
| **Synthetic** | **Chaotic Systems** | Variable | Variable | 0% | 20-100% | [7] | [Link](https://zenodo.org/records/15237226) |
| **Synthetic** | **Sprites** | Video | Variable | 0% | Variable | [1] | [Link](https://github.com/YingzhenLi/Sprites) |
| **Benchmark** | **GIFT-Eval** | Multiple | Variable | 0% | Variable | [10] | [Link](https://huggingface.co/spaces/Salesforce/GIFT-Eval) |
| **Benchmark** | **LOTSA Data** | Multiple | Variable | Varies | Variable | [10] | [Link](https://huggingface.co/datasets/Salesforce/lotsa_data) |

\* *Requires credentialing*  
**Paper numbers refer to the Methods [1-10, 1b] and Applications [11-18] sections above**

**Domain Summary:** Healthcare (9) | Energy (5) | Traffic (4) | Environment (4) | Activity (1) | Finance (1) | Synthetic (4) | Benchmark (2)

### Dataset Statistics by Domain

- **Healthcare & Medical**: 9 datasets - High native missingness, clinical time series, patient records
- **Energy & Electricity**: 5 datasets - Regular sampling, infrastructure monitoring, load forecasting
- **Traffic & Transportation**: 4 datasets - Spatial-temporal networks, sparse sensor observations
- **Environment & Climate**: 4 datasets - Weather monitoring, air quality, long-term climate records
- **Activity & Human Behavior**: 1 dataset - Motion sensor data from daily activities
- **Finance**: 1 dataset - Stock market time series
- **Synthetic & Simulation**: 4 datasets - Controlled experiments, physics simulations, known ground truth
- **Multi-Domain Benchmarks**: 2 datasets - Foundation model evaluation suites

**Key Characteristics:**
- **High Native Missingness**: PhysioNet (~80%), MIMIC-III, Air Quality
- **Extreme Sparsity Testing**: MuJoCo (70-90%), I-24 MOTION (5-20%)
- **Multi-Modal**: PTB-XL (ECG), fMRI (brain imaging), Sprites (video)
- **Spatial-Temporal**: PEMS-BAY, METR-LA, I-24 MOTION (sensor networks)

### Common Experimental Setups

- **Missing Rates**: 10%, 30%, 50%, 70%, 80%, 90%
- **Missing Patterns**: Random, blackout, geometric distribution, block missing
- **Sequence Lengths**: Typically 24-256 time steps in experiments
- **Evaluation**: MSE, MAE, CRPS, discriminative/predictive scores

For complete details including:
- Detailed variable descriptions
- Preprocessing protocols
- Experimental configurations
- Conditioning setups
- Download instructions

**See the comprehensive dataset [TBA] guide.**

## Unclassified Papers

Papers that are relevant to conditioned time series generation but not yet categorized:

- **ST-MVL: Filling Missing Values in Geo-Sensory Time Series Data**

- **Provably Convergent Schrödinger Bridge with Applications to Probabilistic Time Series Imputation**

- **Deep Learning for Multivariate Time Series Imputation: A Survey**

- **MTSCI: A Conditional Diffusion Model for Multivariate Time Series Consistent Imputation**


- **SAITS: Self-Attention-based Imputation for Time Series**
 
## Related Awesome Lists

- [Awesome Time Series](https://github.com/cuge1995/awesome-time-series)
- [Awesome Deep Learning for Time Series](https://github.com/Alro10/deep-learning-time-series)
- [Awesome Diffusion Models](https://github.com/diff-usion/Awesome-Diffusion-Models)
- [Awesome Gaussian Processes](https://github.com/ebonilla/awesome-gaussian-processes)


## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-sa.svg)](http://creativecommons.org/licenses/by-sa/4.0/)
