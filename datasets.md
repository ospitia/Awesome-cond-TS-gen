# Datasets for Conditioned Time Series Generation

A reference of datasets used across the papers in this list. Paper IDs match those in [README.md](README.md).

**Key:**
- `[N]` — paper IDs from the papers sections

---

## Dataset Summary Table

| Domain | Dataset | Dimensions | Seq Length | Native Missing | Exp. Missing | Used in Papers | Download                                                                                           |
|--------|---------|------------|------------|----------------|--------------|----------------|----------------------------------------------------------------------------------------------------|
| **Healthcare** | **PhysioNet 2012** | 35–42 | 48 | ~80% | 10–90% | [1][4][6][11] SAITS | [Link](https://physionet.org/content/challenge-2012/1.0.0/)                                        |
| **Healthcare** | **PhysioNet 2019** | 40+ | 48–72 | High | 50–90% | [2] | [Link](https://physionet.org/content/challenge-2019/1.0.0/)                                        |
| **Healthcare** | **MIMIC-III** | Many | Variable | High | Variable | [2][3] | [Link](https://physionet.org/content/mimiciii/1.4/)                                                |
| **Healthcare** | **PTB-XL** | 12-lead ECG | 10s | 0% | Variable | [5] | [Link](https://physionet.org/content/ptb-xl/1.0.3/)                                                |
| **Healthcare** | **Indicators of Heart Disease** | Multiple | Variable | Varies | Variable | [11] | [CDC/Kaggle](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease) |
| **Healthcare** | **Breast Cancer Wisconsin** | 30 | Variable | Varies | Variable | [11] | [UCI](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)                   |
| **Healthcare** | **Diabetes Health Indicators** | Multiple | Variable | Varies | Variable | [11] | [CDC/Kaggle](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)        |
| **Healthcare** | **COVID-19 Pre-condition** | Multiple | Variable | Varies | Variable | [11] | Public                                                                                             |
| **Healthcare** | **fMRI** | 50 | Variable | 0% | Variable | [8] | Simulated                                                                                          |
| **Energy** | **ETTh1/h2** | 7 | 48–256 | 0% | 10–90% | [8][9] | [Link](https://github.com/zhouhaoyi/ETDataset)                                                     |
| **Energy** | **ETTm1** | 7 | Variable | 0% | Variable | [5] | [Link](https://github.com/zhouhaoyi/ETDataset)                                                     |
| **Energy** | **Appliances Energy** | 28 | 48–256 | 0% | 10–90% | [8] | [Link](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction)                       |
| **Energy** | **ECL (Electricity)** | 321 | Hourly | 0% | Variable | [9] | [Link](https://archive.ics.uci.edu/dataset/321/electricityloaddiagrams20112014)                    |
| **Energy** | **Solar** | Multiple | 168+24 | 0% | Variable | [5][8] | [NREL](https://www.nrel.gov/grid/solar-power-data.html)                                            |
| **Traffic** | **PEMS-BAY** | 325 sensors | 5-min | Sparse | Variable | [5] | [Link](https://github.com/liyaguang/DCRNN)                                                         |
| **Traffic** | **METR-LA** | 207 sensors | 5-min | Sparse | Variable | [5] | [Link](https://github.com/liyaguang/DCRNN)                                                         |
| **Traffic** | **I-24 MOTION** | Grid | Spatial-temp | Sparse | 5–20% | [12] | [Link](https://i24motion.org/)                                                                     |
| **Traffic** | **CARGO** | airfreight tracking | Variable | Sparse | Variable | [14] | [Link](https://www.kaggle.com/datasets/crawford/cargo-2000-dataset)                                                                                           |
| **Environment** | **Air Quality (Beijing)** | ~10 | Variable | ~13% | Blackout | [4][6] | [Link](https://archive.ics.uci.edu/dataset/381/beijing+pm2+5+data)                                 |
| **Environment** | **AQS Data Sets** | Air quality | Variable | Varies | Variable | [14] | [EPA](https://aqs.epa.gov/aqsweb/documents/data_api.html)                                          |
| **Environment** | **Weather** | Multiple | Variable | 0% | Variable | [9] | [Link](https://www.bgc-jena.mpg.de/wetter/)                                                        |
| **Environment** | **Climate Records (NOAA)** | Multiple | Daily/Monthly | Varies | Variable | — | [Link](https://www.osti.gov/biblio/1394920)                                                        |
| **Environment** | **Weather stations** | 2D spatial grid | Km-scale | Sparse | Variable | [17] | —                                                                                                  |
| **Activity** | **UCI Human Activity** | 9 | Variable | 0% | Variable | [Kim+] | [Link](https://archive.ics.uci.edu/dataset/196/localization+data+for+person+activity)              |
| **Finance** | **Stocks** | 6 | 24–48 | 0% | 10–90% | [8] | In repos                                                                                           |
| **Synthetic** | **MuJoCo** | 14 | 100–200 | 0% | 70–90% | [5][6][8] | Simulator                                                                                          |
| **Synthetic** | **Sines** | 5 | 24–100 | 0% | Variable | [8] | Generated                                                                                          |
| **Synthetic** | **Chaotic Systems** | Variable | Variable | 0% | 20–100% | [7] | [Link](https://zenodo.org/records/15237226)                                                        |
| **Synthetic** | **Sprites** | Video | Variable | 0% | Variable | [1] | [Link](https://github.com/YingzhenLi/Sprites)                                                      |
| **Benchmark** | **GIFT-Eval** | Multiple | Variable | 0% | Variable | [10] | [Link](https://huggingface.co/spaces/Salesforce/GIFT-Eval)                                         |
| **Benchmark** | **LOTSA Data** | Multiple | Variable | Varies | Variable | [10] | [Link](https://huggingface.co/datasets/Salesforce/lotsa_data)                                      |

---

For complete paper details including links and code repositories, see the main [README.md](README.md).
