

1. Implement the following metrics (either on separate models or same, your choice):
Recall, Precision, and F1 Score
2. BLEU 
3. Perplexity (explain whether you are using bigram, trigram, or something else, what does your PPL score represent?)
4. BERTScore (here are 1 (Links to an external site.) 2 (Links to an external site.) examples)



## Preplexity

In general, perplexity is a measurement of how well a probability model predicts a sample. In the context of Natural Language Processing, perplexity is one way to evaluate language models.

<img width="1043" alt="image" src="https://user-images.githubusercontent.com/73247157/125182154-3c694300-e229-11eb-91c6-be818ac780e8.png">


Less entropy (or less disordered system) is favorable over more entropy. Because predictable results are preferred over randomness. This is why people say low perplexity is good and high perplexity is bad since the perplexity is the exponentiation of the entropy (and you can safely think of the concept of perplexity as entropy).

### Traingig logs:

![image](https://user-images.githubusercontent.com/73247157/125182167-5acf3e80-e229-11eb-966c-3b74d42b37d0.png)

