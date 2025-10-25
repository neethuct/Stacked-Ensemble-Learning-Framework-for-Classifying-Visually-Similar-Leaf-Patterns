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
