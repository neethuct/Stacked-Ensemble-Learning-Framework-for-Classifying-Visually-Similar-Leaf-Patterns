# Project tittle : 
A Stacked Ensemble Learning Framework for Classifying Visually Similar Leaf Patterns of Popular Indian Hevea Clones Using Shape Descriptive Features
## Project description:
Accurate identification of popular Indian Hevea clones, namely, RRII 105, RRII
414, RRII 417, RRII 422, and RRII 430, is crucial for rubber growers, as
the use of spurious planting materials results in reduced yields and significant
economic losses. Despite its importance, manual identification based on morphological
traits remains the primary method, which is time-consuming and prone
to human error due to the morphological similarity among hybrid clones. Currently,
there is no known automated, reliable system available for identifying
popular Indian Hevea clones, highlighting a significant gap in the management
of rubber plantations. This study addresses this gap by proposing an AI-driven
learning framework specifically tailored for the automated classification of visually
similar leaf patterns of Indian Hevea clones. A custom dataset is curated
under expert supervision at the Rubber Research Institute of India (RRII). A
major innovation of this work is the application of dynamic time warping (DTW)
to capture subtle, spatially dependent leaf border features, providing a robust
representation of fine boundary variations and sequential information beyond
the capability of conventional shape descriptors. Shape-descriptive features were
extracted and ranked using ANOVA F-scores, with a cumulative F-score strategy
selecting an optimal 21-dimensional subset. Multiple classifiers, including SVM,
XGBoost, and DNN, were evaluated, and three models were selected based on
their classification accuracy, generalization capability, and diversity of learning
paradigms. Stacked ensemble of selected models, with logistic regression as the
meta-learner, achieved an accuracy of 82%. SHAP-based interpretability analysis
further identified the most influential features driving the model’s predictions.

data/
│
├── train.csv       # 28 feature columns + 1 'label' column (clone name)
├── test.csv        # Similar structure as train.csv
└── feature_info.txt
HeveaStackedLeaf/
│
├── 1_feature_importance.py   # Feature importance via mutual info, permutation, SHAP
├── 2_feature_selection.py    # Sequential & RFECV-based feature optimization
├── 3_model_training.ipynb    # Base model training and hyperparameter tuning
├── 4_ensemble_framework.ipynb# Stacked ensemble formation and evaluation
├── 5_shap_analysis.ipynb     # SHAP summary + feature importance visualization
└── utils/
    ├── preprocessing.py
    ├── metrics_plotter.py
results/
├── feature_rank.png
├── confusion_matrix.png
├── shap_summary.png
├── metrics_summary.csv
└── ensemble_performance.xlsx
