# LUS midterm project

Midterm project for the **Language Understanding System** course 2019/2020 @ UniTN.

Concept tagging for the movie domain. The models were trained and performed using the following dataset: [NL2SparQL4NLU](https://github.com/esrel/NL2SparQL4NLU).

### Results - SCLM
| Baseline | Remove of OoS | Use of POS tags | Normalization | F1-score | Accuracy | Precision | Recall |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| *Output symbol priors* | | | | **0.0036** | 0.0255 | 0.0036 | 0.0036 |
| *Random path* | | | | **0.0268** | 0.4982 | 0.0218 | 0.0348 |
| *None* | | | | **0.7269** | 0.9165 | 0.7600 | 0.6966 |
| *MLE* | | | | **0.7223** | 0.9127 | 0.7197 | 0.7250 |
| *MLE* | :ballot_box_with_check: | | | **0.7466** | 0.9055 | 0.6883 | 0.8157 |
| *MLE* | :ballot_box_with_check: | :ballot_box_with_check: | | **0.8119** | 0.9421 | 0.8046 | 0.8194 |
| *MLE* | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check: | **0.8021** | 0.9380 | 0.7960 | 0.8084 |

### Results - HMM
| Estimator | Remove of OoS | Use of POS tags | Normalization | F1-score | Accuracy | Precision | Recall |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| *Laplace* | | | | **0.6326** | 0.8871 | 0.7237 | 0.5618 |
| *ELE* | | | | **0.6948** | 0.9050 | 0.7406 | 0.6544 |
| *Lindstone 0.05* | | | | **0.7078** | 0.9074 | 0.7062 | 0.7094 |
| *Lindstone 0.15* | | | | **0.7093** | 0.9099 | 0.7129 | 0.7057 |
| *Witten Bell* | | | | **0.7159** | 0.9124 | 0.7512 | 0.6837 |
| *MLE* | | | | **0.7173** | 0.9086 | 0.7719 | 0.6700 |
| *Lindstone 0.1* | | | | **0.7213** | 0.9130 | 0.7213 | 0.7213 |
| *Witten Bell* + *Witten Bell* | :ballot_box_with_check: | | | **0.7862** | 0.9326 | 0.7821 | 0.7873 |
| *Witten Bell* + *Witten Bell* + *Witten Bell* | :ballot_box_with_check: | :ballot_box_with_check: | | **0.7576** | 0.9277 | 0.7618 | 0.7534 |
| *Witten Bell* + *Witten Bell* + *Witten Bell* + *Witten Bell* | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check: | **0.7311** | 0.9178 | 0.7318 | 0.7305 |
