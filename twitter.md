## Tweet Generator

**Project description:** The aim of this project was to implement an artificial neural network that generates tweets for six different german political parties in the election 2017. I realized the project with two friends. Unfortunately the Github repository is in german, but I will try to give a short description of what we've done here.
We were interested in finding out whether our rather simple models for language generation could pick up on the linguistic differences between the political parties. Therefore, we chose the six most relevant parties in the german election in 2017 and trained a seperate model for each of them, which was then used to generate new tweets that resemble the original ones.
Particularly interesting was the difference between the party from the far right compared to the parties from the left wing. The right parties used way more aggressive language and repeated a lot of mantra-like statements, while the left parties were more concentrated in giving actual content and relevant information.

### 1. The Process

In this project, we implemented two different neural nets to generate the tweets. One was a simple recurrent neural network (RNN) and the other one a long-short-term memory network (LSTM).
A big part of the project was to gather and clean the twitter data, which was more challenging than anticipated before hand. Without the preprocessing the vocabulary was very large, on parts because a word and the same word with a punctuation sign was counted seperately. The same happened for different spellings, abbreviations and so forth.
After the dataset was constructed, the two models, the simple RNN and the more complex LSTM, where trained with the datasets from each party and new tweets were generated.

### 2. The Results

Surprisingly, the simpler RNN yielded better results in many cases compared to the LSTM. The reason for that is that the LSTM was faster to get stuck in local minima and therefore often produced tweets with repeating words.
The dataset was to small for the model to learn grammatical structures. Therefore, the tweets are mostly not good enough to be mistaken for an origianl tweet. Nonetheless, the results are very interesting to examine, because even in these small sample results one can find differences in the vocabulary and type of language between the different parties.

### 3. Personal Summary

This project was my first endeavour into the world of artificial neural networks. Hence, I learned a lot about the theoretical background and the implementation of machine learning algorithms. Additionally, I learned how important (and difficult to get) nice and clean data is and that the preprocessing should never be underestimated.
