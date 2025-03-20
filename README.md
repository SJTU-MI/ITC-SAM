# ITC-SAM
Physical-based and data-driven hybrid protocol for optimizing thermal transport across solid-water interfaces with self-assembled monolayers

## Description
Thermal transport across the solid-water interface in self-assembled monolayer (SAM) is crucial for thermal management applications. However, the vast number of end groups options and the scarcity of thermal property data make the SAM design challenging. To this end, here we have developed and proposed a machine learning (ML) assisted SAM design strategy for tuning the interfacial thermal conductance (ITC) considering various end groups. We first built a SAM thermal transport database with 300 different end groups via the high-throughput molecular dynamics (MD) simulations, with the ITC values ranging from 38.93 to 240.31 MW/m²K. The physical design framework based on MD incorporating 135 descriptors is then proposed, which significantly improves the performance of ML models for ITC prediction. Furthermore, the feature analysis based on data-driven approaches shows that as compared to features such as vibrational spectral coupling strength and SAM length, interfacial interactions are the core factor influencing interfacial thermal transport. Building on this, we use grid-based symbolic regression to generate several simple and interpretable descriptors at the Pareto front of nearly 30,000 fitting formulas. In contrast to relying on a single interfacial interaction metric, the new descriptors facilitate the identification of high-ITC SAMs. The framework and results presented in this work fill the knowledge gap in tuning interfacial thermal transport under complex SAM end group designs, providing both data and theoretical support for related applications.

### Files loading:
To download, clone this repository:<br>
````
git clone https://github.com/SJTU-MI/ITC-SAM.git
````

## Authors

| **AUTHORS** |Shengluo Ma, Shenghong Ju            |
|:-------------:|--------------------------------------------------|
| **VERSION** | V1.0 / November,2024                               |
| **EMAILS**  | shenghong.ju@sjtu.edu.cn                         |
| **GROUP HOME**  | https://ju.sjtu.edu.cn/en/                         |

## Attribution
This work is under BSD-2-Clause License. Please, acknowledge use of this work with the appropiate citation to the repository and research article.
