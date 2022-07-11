# Evaluation of the quality of word embedding models for Vietnamese (GloVe, Word2Vec, ELMO, FASTTEXT)
## This is a research project

The main content focuses on evaluating the quality of Words Embedding models Including: **GloVe, Word2Vec, ELMO, FASTTEXT**

Because the problem focuses more on the quality of Words Embedding models. So me and my friends use custom LSTM model for news topic classification problem

The model volume is very large around 800mb -1gb, I won't upload the model here. You can monitor the implementation process through 4 colab files.

To ensure fairness in the process of comparing Word Embeddings models, this project we use **4 custom models**:
- Multi layer perceptron (MLPs)
- LSTM
- Sequential_30 (custom model)
- LSTM + CNN
---
### Accuracy results can refer to the following:

|            Model      |     Fast   Text    	|     GloVe    	|     ELMo     	|     Word2Vec    	|
|----------------------	|--------------------	|--------------	|--------------	|-----------------	|
|     MLPs (custom)    	|     96.55          	|     95.47    	|     95.04    	|     97.37       	|
|     LSTM             	|     96.09          	|     95.67    	|     94.62    	|     94.58       	|
|     CNN + LSTM       	|     97.15          	|     96.15    	|     95.88    	|     95.05       	|
|     Bi - LSTM        	|     96.89          	|     95.85    	|     95.1     	|     95.63       	|

### Or track as the following graph:

![image](https://user-images.githubusercontent.com/55480300/178314087-9fff6ab2-2197-4944-8185-36c7a047d8f9.png)

### We can track the convergence of the model through loss:

__*Figure loss 1: Graph of loss function of word-embedding models compared to the first model MLPs (custom)*__

![image](https://user-images.githubusercontent.com/55480300/178314644-27841aea-c6ef-48bf-9c30-56b22a303fb8.png)

---
__*Figure loss 2: Graph of loss function of word-embedding models compared to the Second model LSTM (custom)*__

![image](https://user-images.githubusercontent.com/55480300/178315348-47599a34-643b-4833-b2a5-5ebc21c93961.png)

---
__*Figure loss 3: Graph of loss function of word-embedding models compared to the third CNN+LSTM (custom)*__
![image](https://user-images.githubusercontent.com/55480300/178315543-df82d6a8-8477-4f75-9617-dedc996b01fd.png)

---
__*Figure loss 4: Graph of loss function of word-embedding models compared to the fourth Bi-LSTM (custom)*__
![image](https://user-images.githubusercontent.com/55480300/178315779-cb390b61-296a-4ef3-9736-a93ff518b455.png)


