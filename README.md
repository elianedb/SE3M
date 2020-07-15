# SE3M
This repository contains the source codes and data set used in the experiments at the article entitled "SE3M: A model for estimating software effort using pre-trained embeddings models" (FÁVERO et al., 2020).

FÁVERO, Eliane M.; CASANOVA, Dalcimar; PIMENTEL, Andrey Ricardo. SE3M: A Model for Software Effort Estimation Using Pre-trained Embedding Models. arXiv preprint arXiv:2006.16831, 2020.


1. Conjunto de dados (histórias de usuário) rotulado [1], usado para treino e testes do modelo de inferência.
   https://github.com/morakotch/datasets/tree/master/storypoint/IEEE%20TSE2018/dataset
   
   - Correspondem a um conjunto de arquivos .CSV correpondentes a cada um dos projetos utilizados. 

2. Modelos de embeddings pré-treinados (genéricos). 
   - Disponíveis na pasta "pretrain_model"
     - word2vec_base
     - BERT_base

3. Conjunto de dados (histórias de usuário) não-rotulado, utilizado no processo de ajuste fino dos modelos de embeddings pré-treinados.
      https://github.com/morakotch/datasets/tree/master/storypoint/IEEE%20TSE2018/pretrain%20data
   
   - Correspondem a um conjunto de arquivos .CSV correpondentes a cada um dos projetos utilizados. 

4. Modelos de embeddings pré-treinados (ajustados):
  - word2vec_SE
  - BERT_SE


References:

[1] M. Choetkiertikul, HK Dam, T. Tran, TTM Pham, A. Ghose e T. Menzies, "Um modelo de aprendizado profundo para estimar pontos da história", IEEE Trans. Softw. Eng. Vol. PP, não. 99, p. 1, 2018.





















