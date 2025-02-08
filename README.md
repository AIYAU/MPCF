# MPCF: 
Multimodal Prototypical Networks with Co-metric Fusion for Few-Shot Hyperspectral lmage Classification
## Requirements
To run this project, you will need to add the following environment variables to your .env file

`python = 3.9.18`

`torch == 1.12.1+cu113`
## Datasets
- source domain dataset
  - Chikusei
    
- target domain datasets
  - Indian Pines
  - Houston
  - Salinas
## Pretrain model
An example pretrain-model folder has the following structure:

```
pretrain-model
└── bert-base-uncased
    ├── config.json
    ├── pytorch_model.bin
    ├── tokenizer.json
    ├── tokenizer_config.json
    └── vocab.txt
```
## Usage
1. Download the required source and target datasets and move to folder `datasets`.
   - If you down the source domain dataset (Chikusei) in mat format, you need to run the script `Chikusei_imdb_128.py` to generate preprocessed source domain data. 
2. Download the required Base Bert pre-trained model and move to folder `pretrain-model`.
3. Run `train_our_IP.py`,`train_our_HT.py`,`train_our_SA.py`.
