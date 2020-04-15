# LUS midterm project

Midterm project for the **Language Understand System** course 2019/2020 @ UniTn.

Concept tagging for the movie domain. The models were trained and performed using the following dataset: [NL2SparQL4NLU](https://github.com/esrel/NL2SparQL4NLU)

### Results
| Baseline | Remove of OoS | Use of POS | Normalization | F1-score | Accuracy | Precision | Recall |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| *None* | | | | **0.723** | 0.915 | 0.751 | 0.696 |
| *Random path* | | | | **0.019** | 0.395 | 0.014 | 0.033 |
| *Output symbol priors* | | | | **0.126** | 0.653 | 0.136 | 0.117 |
| *MLE* | | | | **0.723** | 0.915 | 0.718 | 0.728 |
| *MLE* | :ballot_box_with_check: | | | **0.805** | 0.940 | 0.785 | 0.827 |
| *MLE* | :ballot_box_with_check: | :ballot_box_with_check: | | **0.811** | 0.942 | 0.805 | 0.817 |
