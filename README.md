# SE3M
This repository contains the source codes and data set used in the experiments at the article entitled "SE3M: A model for estimating software effort using pre-trained embeddings models" (FÁVERO et al., 2020).

FÁVERO, Eliane M.; CASANOVA, Dalcimar; PIMENTEL, Andrey Ricardo. SE3M: A Model for Software Effort Estimation Using Pre-trained Embedding Models. arXiv preprint arXiv:2006.16831, 2020.


1. Data set (user story) labeled [1], used for training and testing the inference model.
   https://github.com/morakotch/datasets/tree/master/storypoint/IEEE%20TSE2018/dataset
   
   - Correspond to a set of .CSV files for each of the projects used.

2. Pre-trained embeddings (generic). 
   - Available in the folder "pretrain_model"
     - word2vec_base
     - BERT_base

3. Unlabeled data set (user story) used in the fine-tuning process of pre-trained embeddings.
      https://github.com/morakotch/datasets/tree/master/storypoint/IEEE%20TSE2018/pretrain%20data

4. The pre-processing of the data used to perform the fine-tuning process with BERT, as well as fine-tuning, used the methods provided by the BERT model in its official repository at https://github.com/google-research/bert 
   - For data pre-processing: create_pretraining_data.py 
      - Standard parameters were used, changing only the following::
         -input_file= (inform file .txt containing all the textual requirements provided in item 2)
         -output_file=./tf_examples.tfrecord \
         -vocab_file= (inform file .txt corresponding to the vocabulary of the pre-trained model used, ex./uncased_L-12/vocab.txt) 


4. Pre-trained embeddings (fine-tuned) models for the specific domain of software engineering (SE):
   - word2vec_SE
   - BERT_SE

5. The "SE3M_model.ipynb" file contains a deep learning of architecture used as an inference model for estimating software effort by analogy. Is a Google Colab notebook, simply replacing the paths of the files used.


References:

[1] M. Choetkiertikul, HK Dam, T. Tran, TTM Pham, A. Ghose e T. Menzies, "Um modelo de aprendizado profundo para estimar pontos da história", IEEE Trans. Softw. Eng. Vol. PP, não. 99, p. 1, 2018.





















