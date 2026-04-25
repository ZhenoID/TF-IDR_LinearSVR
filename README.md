Dataset Sensitivity Check for Story Point Estimation

The experiment checks whether a simple TF-IDF + LinearSVR model performs consistently across two story point datasets: Bamboo and Duracloud.

Each dataset is split into:

- 70% training data
- 15% validation data
- 15% test data

The model is trained and tested in four settings:

- Bamboo → Bamboo
- Bamboo → Duracloud
- Duracloud → Duracloud
- Duracloud → Bamboo

The experiment is repeated using five random seeds

The reported metrics are:

- MAE Mean
- MAE Std.
- Median Baseline MAE
- Standardized Accuracy (SA)
- ΔMAE
