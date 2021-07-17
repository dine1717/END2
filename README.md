

# Glove

GloVe is an unsupervised learning algorithm for obtaining vector representations for words. Training is performed on aggregated global word-word co-occurrence statistics from a corpus, and the resulting representations showcase interesting linear substructures of the word vector space.

1. Nearest neighbors

The Euclidean distance (or cosine similarity) between two word vectors provides an effective method for measuring the linguistic or semantic similarity of the corresponding words. Sometimes, the nearest neighbors according to this metric reveal rare but relevant words that lie outside an average human's vocabulary. For example, here are the closest words to the target word frog:
        frogs
        toad
        litoria
        leptodactylidae
        rana
        lizard
        eleutherodactylus


2. Linear substructures

The similarity metrics used for nearest neighbor evaluations produce a single scalar that quantifies the relatedness of two words. This simplicity can be problematic since two given words almost always exhibit more intricate relationships than can be captured by a single number. For example, man may be regarded as similar to woman in that both words describe human beings; on the other hand, the two words are often considered opposites since they highlight a primary axis along which humans differ from one another.


In order to capture in a quantitative way the nuance necessary to distinguish man from woman, it is necessary for a model to associate more than a single number to the word pair. A natural and simple candidate for an enlarged set of discriminative numbers is the vector difference between the two word vectors. GloVe is designed in order that such vector differences capture as much as possible the meaning specified by the juxtaposition of two words.

![image](https://user-images.githubusercontent.com/73247157/126044795-27429990-0b23-46a7-8bf5-0765fc8ace8d.png)
![image](https://user-images.githubusercontent.com/73247157/126044799-2eeb3f1b-b779-42bd-97f3-e4c8ed81666f.png)

The underlying concept that distinguishes man from woman, i.e. sex or gender, may be equivalently specified by various other word pairs, such as king and queen or brother and sister. To state this observation mathematically, we might expect that the vector differences man - woman, king - queen, and brother - sister might all be roughly equal. This property and other interesting patterns can be observed in the above set of visualizations.

3. Training

The GloVe model is trained on the non-zero entries of a global word-word co-occurrence matrix, which tabulates how frequently words co-occur with one another in a given corpus. Populating this matrix requires a single pass through the entire corpus to collect the statistics. For large corpora, this pass can be computationally expensive, but it is a one-time up-front cost. Subsequent training iterations are much faster because the number of non-zero matrix entries is typically much smaller than the total number of words in the corpus.


The tools provided in this package automate the collection and preparation of co-occurrence statistics for input into the model. The core training code is separated from these preprocessing steps and can be executed independently.

4. Model Overview
5. 
GloVe is essentially a log-bilinear model with a weighted least-squares objective. The main intuition underlying the model is the simple observation that ratios of word-word co-occurrence probabilities have the potential for encoding some form of meaning. For example, consider the co-occurrence probabilities for target words ice and steam with various probe words from the vocabulary. Here are some actual probabilities from a 6 billion word corpus:

![image](https://user-images.githubusercontent.com/73247157/126044821-91321e62-0896-47df-b20d-2c21d748cd64.png)

As one might expect, ice co-occurs more frequently with solid than it does with gas, whereas steam co-occurs more frequently with gas than it does with solid. Both words co-occur with their shared property water frequently, and both co-occur with the unrelated word fashion infrequently. Only in the ratio of probabilities does noise from non-discriminative words like water and fashion cancel out, so that large values (much greater than 1) correlate well with properties specific to ice, and small values (much less than 1) correlate well with properties specific of steam. In this way, the ratio of probabilities encodes some crude form of meaning associated with the abstract concept of thermodynamic phase.

The training objective of GloVe is to learn word vectors such that their dot product equals the logarithm of the words' probability of co-occurrence. Owing to the fact that the logarithm of a ratio equals the difference of logarithms, this objective associates (the logarithm of) ratios of co-occurrence probabilities with vector differences in the word vector space. Because these ratios can encode some form of meaning, this information gets encoded as vector differences as well. For this reason, the resulting word vectors perform very well on word analogy tasks, such as those examined in the word2vec package.







# Training Logs 

        1m 12s (- 16m 53s) (5000 6%) 3.4134
        2m 21s (- 15m 20s) (10000 13%) 2.7728
        3m 30s (- 14m 3s) (15000 20%) 2.4286
        4m 40s (- 12m 50s) (20000 26%) 2.1855
        5m 50s (- 11m 40s) (25000 33%) 1.9397
        6m 59s (- 10m 29s) (30000 40%) 1.7791
        8m 8s (- 9m 18s) (35000 46%) 1.6084
        9m 18s (- 8m 8s) (40000 53%) 1.5126
        10m 28s (- 6m 59s) (45000 60%) 1.3562
        11m 39s (- 5m 49s) (50000 66%) 1.2694
        12m 49s (- 4m 39s) (55000 73%) 1.2186
        13m 59s (- 3m 29s) (60000 80%) 1.1403
        15m 9s (- 2m 19s) (65000 86%) 1.0582
        16m 19s (- 1m 9s) (70000 93%) 0.9928
        17m 31s (- 0m 0s) (75000 100%) 0.9518
        
        
         > i m cultured .
        = je suis cultive .
        < je suis cultive . <EOS>

        > he s not working much at the moment .
        = il ne travaille pas beaucoup en ce moment .
        < il n travaille pas en train de la . <EOS>

        > you re the teacher .
        = c est toi la professeur .
        < c es toi l enseignant . <EOS>

        > we re retiring .
        = nous partons a la retraite .
        < nous sur la . <EOS>

        > you are on the wrong train .
        = tu es dans le mauvais train .
        < tu es sur le mauvais . <EOS>


# Traing Logs with Glove Emdeddings

<img width="511" alt="image" src="https://user-images.githubusercontent.com/73247157/126046007-faf2904d-ce0e-45a4-adcc-7578eed67c79.png">


<img width="475" alt="image" src="https://user-images.githubusercontent.com/73247157/126046016-ee2231b6-2bd5-40a6-a311-226902962c72.png">







