# Physical-Properties-Prediction-in-Thermal-Insulation-Material-and-GDL-materials
Collaboration between healthhub.kr and Hyundai-Kia Motors R&amp;D Center
# Physical Properties Prediction for Thermal Insulation & GDL Materials

**Collaboration between HealthHub.kr & Hyundai-Kia Motors R&D Center**

---

## 📘 Project Overview

This repository encapsulates the research and analysis from internal reports and presentations on predicting **physical properties** of **thermal insulation materials** and **Gas Diffusion Layer (GDL) materials**.  
Because the source code is withheld for privacy, this README summarizes the methodology, data pipeline, experiments, and key findings based entirely on published PDFs and slide decks.

The main goals:

- Predict material-level properties (e.g. thermal conductivity, mechanical strength) from structural and morphological features  
- Compare different modeling strategies (linear, tree, neural)  
- Understand which features are most informative  
- Provide reproducible experiments, figures, and analysis via the archived PDF deliverables


These deliverables contain:

- Problem formulation  
- Data descriptions & feature definitions  
- Modeling and evaluation results  
- Analysis, visualizations, and discussion  

---

## 📄 Methodology Summary

Below is a distilled overview of the approach as documented in your PDFs:

### 1. **Data & Feature Engineering**

- Use experimental datasets of **thermal insulation** and **GDL** samples  
- Extract structural, morphological, and geometric features (e.g. porosity, thickness, pore size distribution, microstructure metrics)  
- Clean and preprocess data (missing values, normalization, outlier removal)  

### 2. **Modeling Approaches**

Several modeling pipelines were explored:

- **Linear models & regularization** (Lasso, Ridge) for baseline  
- **Tree-based ensembles** (Random Forest, XGBoost)  
- **Neural networks / MLPs** to capture nonlinear relationships  

Cross-validation and hyperparameter tuning were used to select best models. Model performance metrics include RMSE, R², MAE, etc.

### 3. **Evaluation & Interpretability**

- Evaluate generalization on held-out test folds  
- Analyze **feature importance** or coefficients to find dominant predictors  
- Compare model transferability between **insulation** vs **GDL** materials  
- Diagnose error patterns and domain-specific deviations  

### 4. **Presentation & Reporting**

The final deliverables include:

- A **WBS1 Hyundai Motors** slide deck summarizing business-facing insights  
- A **Final Report WBS2** PDF with methods, results, tables, and charts  
- **WBS3 presentation** for external stakeholders  

These files include visualizations (scatterplots, residual graphs, importance bar plots) and contextual discussion.

---

## 🧮 Key Findings

Some of the notable observations documented:

- **Porosity**, **material thickness**, and **microstructure features** tend to dominate in predictive importance  
- Linear methods work reasonably well as a baseline, but ensemble and neural models capture additional variance  
- Transfer learning or cross-material generalization (insulation → GDL or vice versa) is challenging due to structural differences  
- Errors are higher in edge cases (e.g. extremely porous or very dense samples)  

---

## 🛠 Guidance for Future Use

Although code is not public in this repo, future users can replicate the pipeline by:

1. Reconstructing feature extraction modules from the feature definitions in the PDFs  
2. Following the described modeling strategies and hyperparameter ranges  
3. Reproducing cross-validation splits and evaluation metrics  
4. Regenerating comparable visualizations and reporting formats  



