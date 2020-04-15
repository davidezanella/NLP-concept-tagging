# LUS midterm project

Midterm project for the **Language Understand System** course 2019/2020 @ UniTN.

Concept tagging for the movie domain. The models were trained and performed using the following dataset: [NL2SparQL4NLU](https://github.com/esrel/NL2SparQL4NLU).

### Results - SCLM
| Baseline | Remove of OoS | Use of POS tags | Normalization | F1-score | Accuracy | Precision | Recall |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| *None* | | | | **0.7238** | 0.9158 | 0.7532 | 0.6966 |
| *Random path* | | | | **0.0197** | 0.3951 | 0.0139 | 0.0339 |
| *Output symbol priors* | | | | **0.1260** | 0.6535 | 0.1361 | 0.1173 |
| *MLE* | | | | **0.7233** | 0.9154 | 0.7181 | 0.7286 |
| *MLE* | :ballot_box_with_check: | | | **0.8058** | 0.9405 | 0.7852 | 0.8276 |
| *MLE* | :ballot_box_with_check: | :ballot_box_with_check: | | **0.8112** | 0.9422 | 0.8050 | 0.8175 |
| *MLE* | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check: | **0.8117** | 0.9404 | 0.8094 | 0.8139 |
