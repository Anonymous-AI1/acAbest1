# CoT-BERT: Enhancing Unsupervised Sentence Representation through Chain-of-Thought  

## Results

|             Model             | STS12 | STS13 | STS14 | STS15 | STS16 | STSb  | SICK-R | Avg.  |
| :---------------------------: | :---: | :---: | :---: | :---: | :---: | :---: | :----: | :---: |
|  Unsupervised CoT-BERT-base   | 72.56 | 85.53 | 77.91 | 85.05 | 80.94 | 82.40 | 71.41  | 79.40 |
| Unsupervised CoT-RoBERTa-base | 75.43 | 85.47 | 78.74 | 85.64 | 82.21 | 83.40 | 73.46  | 80.62 |

- Our Checkpoints

  - CoT-BERT-base Checkpoint

    https://drive.google.com/file/d/1cwSNuAw8EJnqIAHDOjMGMFFHMr0qdh2d/view?usp=sharing

  - CoT-RoBERTa-base Checkpoint

    https://drive.google.com/file/d/1uEE2tVH1D5c4h4VPzRCT7Nf3HDr1_HZc/view?usp=sharing

## Setup

- Install Dependencies

  ```sh
  pip install -r requirements.txt
  ```

- Download Data

  ```sh
  cd SentEval/data/downstream/
  bash download_dataset.sh
  cd -
  cd ./data
  bash download_wiki.sh
  bash download_nli.sh
  cd -
  ```

- Train with BERT-base

  ```sh
  cd code-for-BERT
  python train.py
  ```

- Train with RoBERTa-base

  ```sh
  cd code-for-RoBERTa
  python train.py
  ```
