# COMP90051 Project 2
Jiehuang Shi
Hongyi Gu
Yuxin Zhao

## Overview
The task discussed in the report is to solve an authorship attribution problem by predicting prolific authors for each academic paper given a set of training and test data.  

## Requirements
* [Tensorflow](version >= 2.4.1)
* [tensorflow_addons](version >= 0.15.0)
* [scikit-learn]
* [scikit-skmultilearn]
* [gensim]

## Data Preparation
test.json and test.json files are provided. It just needs to be in the same root as the py script.

project 2
  |--train.json
  |--test.json
```

## Getting Started (Training & Testing)

### Training with BinaryRelevance:
```
python project2.py --model BinaryRelevance --epochs 50 --batch_size 32 --lr 0.001
```
### Training with ClassifierChain:
```
python project2.py --model ClassifierChain --epochs 50 --batch_size 32 --lr 0.001
```
### Training with LabelPowerset:
```
python project2.py --model LabelPowerset --epochs 50 --batch_size 32 --lr 0.001
```
### Training with MLP:
- MLP Testing
```
python project2.py --model mlp --test
```
###- Training with LSTM:
- LSTM Testing:
```
python project2.py --model lstm --test
```
- LSTM training with full dataset and Testing
```
python project2.py --model lstm --full_data --test
```
- LSTM Testing and plot
```
python project2.py --model lstm --test_saved_csv_name result.csv --test --plot_acc_loss 
```
