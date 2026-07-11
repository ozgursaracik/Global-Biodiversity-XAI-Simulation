Explaining Global Biodiversity: XAI & Policy Simulation 🌍

A data-driven machine learning framework designed to estimate national biodiversity index values from multidimensional factors (economic development, natural resources, and climate). This project goes beyond standard prediction by integrating Explainable AI (SHAP), unsupervised anomaly detection, and a counterfactual Policy Simulator.

🎯 Objective

To provide a robust, transparent, and actionable modeling pipeline that helps understand the complex drivers of global biodiversity. The system evaluates the ecological sensitivity of different regions through "what-if" policy scenarios (e.g., assessing the impact of a 30% reduction in forest area).

⚙️ Methodology & Tech Stack

Machine Learning Benchmarking: Comprehensive evaluation of 6 diverse architectures including XGBoost, Deep Neural Networks (DNN), Random Forest, K-Nearest Neighbors (KNN), Multi-Layer Perceptron (MLP/ANN), and Stacking Regressors.

Unsupervised Representation Learning: Implementation of an Autoencoder to identify features associated with ecological divergence in outlier nations and to extract causal roots.

Explainable AI (XAI): Utilization of SHAP (SHapley Additive exPlanations) for global feature importance and local interaction analysis, revealing non-linear associations between climatic zones and geographic metrics.

Validation Strategy: Spatial Group K-Fold cross-validation over geographic macro-regions to ensure strict spatial transferability and prevent data leakage.

Tech Stack: Python, PyTorch (DNN & Autoencoders), XGBoost, Scikit-Learn, SHAP, Pandas, Matplotlib.

📂 Repository Structure

notebooks/: Contains the core experimental Jupyter Notebooks.

XGBoost.ipynb, DNN.ipynb, RandomForest.ipynb, StackingLR.ipynb, KNN.ipynb, ANN_Improved.ipynb: Model training, hyperparameter tuning, and evaluation.

AutoEconder - CausalRoot.ipynb: Unsupervised anomaly attribution and policy simulation engine.

data/: Sample dataset structure (sensitive/proprietary data omitted).

src/: Core Python modules for SHAP analysis and the counterfactual policy simulation logic.

🚀 Key Findings

The XGBoost-based explanatory pipeline achieved the highest stability in spatial transferability.

National biodiversity is highly sensitive to specific non-linear interactions between forest area retention and regional climatic classifications.

The Autoencoder successfully isolated anomalous ecological behaviors in outlier countries, providing a secondary layer of validation for the predictive models.
