# Master Semester Project

## Dueling Chinese Couplet using Sequence to Sequence Model

#### Pre-requisites
To run the project, you will need python3 along with the libraries *numpy*, *matplotlib*, and *torch*. The codes are tested on *Python 3.7.3*.

### Datasets
*vocab.txt* contains all vocabularies extracted from couplet datasets.
*in.txt* contains couplet input for the training process.
*out.txt* contains couplet input for the training process.
*test_in.txt* contains couplet input for the evaluation process.
*test_out.txt* contains couplet input for the evaluation process.


### Structure of the codes
This repo contains several files both for training and evaluating. 

##### - run_training.py
This file is used to train the sequence to sequence model. The trained model will be save into *models* folder.
The following command was used for training in this project.
```
python run_training.py -a True -ep 204
```
More hyperparameters can be tuned. Please refer to *help* for further information.

##### - evaluation.ipynb
The obatined model from *run_training.py* can be used in "evaluation.ipynb" in order to evaluate the model.
##### - encoderRNN.py
This file contains codes for encoder.
##### - attention_II.py
This file contains codes for attention.
##### - attnDecoderRNN_II.py
This file contains codes for decoder with attention mechanism.
##### - utils.py
This file contains helper functions.

### Resources
Seq2seq trainslation tutorial:https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html

Attention: https://pytorchnlp.readthedocs.io/en/latest/_modules/torchnlp/nn/attention.html

Chinese Couplet dataset: https://github.com/wb14123/couplet-dataset
