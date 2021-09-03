#  BUG Dataset <img src="https://user-images.githubusercontent.com/6629995/132018898-038ec717-264d-4da3-a0b8-651b851f6b64.png" width="30" /><img src="https://user-images.githubusercontent.com/6629995/132017358-dea44bba-1487-464d-a9e1-4d534204570c.png" width="30" /><img src="https://user-images.githubusercontent.com/6629995/132018731-6ec8c4e3-12ac-474c-ae6c-03c1311777f4.png" width="30" />
A Large-Scale Gender Bias Dataset for Coreference Resolution and Machine Translation, Levy et al., Findings of EMNLP 2021.

## Setup

1. Unzip data.tar.gz
2. Setup a python 3.x environment and install requirements: `pip install -r requirements.txt`

## Dataset Partitions


### <img src="https://user-images.githubusercontent.com/6629995/132018898-038ec717-264d-4da3-a0b8-651b851f6b64.png" width="20" /> Full BUG

### <img src="https://user-images.githubusercontent.com/6629995/132017358-dea44bba-1487-464d-a9e1-4d534204570c.png" width="20" /> Gold BUG 

### <img src="https://user-images.githubusercontent.com/6629995/132018731-6ec8c4e3-12ac-474c-ae6c-03c1311777f4.png" width="20" /> Balanced BUG


## Evaluations
See below instructions for reproducing our evaluations on BUG.

### Coreference
1. Download the Spanbert predictions from [this link](https://drive.google.com/file/d/1i24T1YT_0ByxttrCRR7qxEnt8UWyEJ7R/view?usp=sharing).
2. Unzip and put `coref_preds.jsonl` in in the `predictions/` folder.
3. From `src/evaluations/`, run `python evaluate_coref.py --in=../../predictions/coref_preds.jsonl --out=../../visualizations/delta_s_by_dist.png`.
4. This should reproduce the [coreference evaluation figure](visualizations/delta_s_by_dist.png).



## Citing


