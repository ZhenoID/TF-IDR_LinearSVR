Dataset Sensitivity Check for Story Point Estimation

The experiment checks whether a simple TF-IDF + LinearSVR model performs consistently across two story point datasets: Bamboo and Duracloud.

Each dataset is split into:

- 85% training data
- 15% test data

The pipeline has fixed hyperparameters so no tuning is required. Therefore no validation split
The model is trained and tested in four settings:

- Bamboo → Bamboo
- Bamboo → Duracloud
- Duracloud → Duracloud
- Duracloud → Bamboo

The experiment is repeated using five random seeds (7, 21, 42, 123, 2026) for variance  

The reported metrics are:

- MAE Mean
- MAE Std.
- Median Baseline MAE
- Standardized Accuracy (SA)
- ΔMAE
