# ITC-SAM
Physical-based and data-driven hybrid protocol for optimizing thermal transport across solid-water interfaces with self-assembled monolayers

## Description
Thermal transport across the solid-water interface in self-assembled monolayer (SAM) is crucial for thermal management applications. However, the vast number of end groups options and the scarcity of thermal property data make the SAM design challenging. To this end, here we have developed and proposed a machine learning (ML) assisted SAM design strategy for tuning the interfacial thermal conductance (ITC) considering various end groups. We first built a SAM thermal transport database with 300 different end groups via the high-throughput molecular dynamics (MD) simulations, with the ITC values ranging from 38.93 to 240.31 MW/m²K. The physical design framework based on MD incorporating 135 descriptors is then proposed, which significantly improves the performance of ML models for ITC prediction. Furthermore, the feature analysis based on data-driven approaches shows that as compared to features such as vibrational spectral coupling strength and SAM length, interfacial interactions are the core factor influencing interfacial thermal transport. Building on this, we use grid-based symbolic regression to generate several simple and interpretable descriptors at the Pareto front of nearly 30,000 fitting formulas. In contrast to relying on a single interfacial interaction metric, the new descriptors facilitate the identification of high-ITC SAMs. The framework and results presented in this work fill the knowledge gap in tuning interfacial thermal transport under complex SAM end group designs, providing both data and theoretical support for related applications.

### Files loading:
To download, clone this repository:<br>
````
git clone https://github.com/SJTU-MI/ITC-SAM.git
````

## Try the desired parts of the project:

### Code in the HTPS4HTTEMOs folder
**1_data4PF**: Power factor (PF) data collection and initial descriptor creation.
- 1_MP_api_features: Descriptors retrieved from the MP database
- 2_Xenonpy_features: Descriptors retrieved from Xenonpy
- 3_data4PF: The PF data and initial descriptor.

**2_featurefiltering**: Feature down-selection process.
- 1_lowvar: Screening features through variance.
- 2_corfilter: Screening features through correlation coefficient.

**3_featurecreation_bySR**: Feature creation process by symbolic regression (SR).
- 1_PC: Feature creation based on Pearson correlation (PC).
- 2_SC: Feature creation based on Spearman correlation (SC).
- 3_DC: Feature creation based on Distance correlation (DC).

**4_PFmodel**: PF prediction model training.
- 1_RF: Random Forest model training.
- 2_XG: XGBoost model training.
- 3_MLP: Multi-Layer Perceptron model training.

**5_SHAPanalysis**: SHAP analysis for the PF prediction model.
- 1_featureimportance: Feature importance calculation.
- 2_beeswarm_plot: Beeswarm plot on SHAP.
- 3_dependence_plot: Dependence plot on SHAP.

**6_meltingpointAPI**: API for the [melting point prediction model](https://www.pnas.org/doi/10.1073/pnas.2209630119).
- 1_prepare4API: Prepare the API json file from MP database for melting point prediction.
- 2_meltingpoint_predict: Melting point prediction.
- 3_meltingpoint_result: Melting point prediction results.

**7_HTP_virtualscreening**: Virtual screening for High-Temperature Thermoelectric Metal Oxides.
- 1_MPscreening: High-Throughput Screening based on MP database.
- 2_MLprediction: PF prediction of three ML models.

**8_PF_calresults**: The PF results by High-Throughput (HTP) DFT calculations.

## Authors

| **AUTHORS** |Shengluo Ma, Shenghong Ju            |
|:-------------:|--------------------------------------------------|
| **VERSION** | V1.0 / November,2023                               |
| **EMAILS**  | shenghong.ju@sjtu.edu.cn                         |
| **GROUP HOME**  | https://ju.sjtu.edu.cn/en/                         |

## Attribution
This work is under BSD-2-Clause License. Please, acknowledge use of this work with the appropiate citation to the repository and research article.
