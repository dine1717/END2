Goal

The goal is to build a sentiment analysis model using StanfordSentimentAnalysis Dataset.

Use "Back Translate", "random_swap" and "random_delete" to augment the data.

Download the StanfordSentimentAnalysis Dataset from this link (http://nlp.stanford.edu/~socherr/stanfordSentimentTreebank.zip) and unzipo the files.


> datasetSentences.txt -> Contains the sentence index, followed by the sentence string separated by a tab. These are the sentences of the train/dev/test sets.

> datasetSplit.txt -> Contains the sentence index (corresponding to the index in datasetSentences.txt file) followed by the set label separated by a comma:
	1 = train
	2 = test
	3 = dev
> dictionary.txt -> Contains all phrases and their IDs, separated by a vertical line.
>original_rt_snipeets.txt -> Contains 10,605 processed snippets from the original pool of Rotten Tomatoes HTML files. Please note that some snippet may contain multiple sentences.
>sentiments_labels.txt -> Contains all phrase ids and the corresponding sentiment labels, separated by a vertical line.
Note that you can recover the 5 classes by mapping the positivity probability using the following cut-offs:
[0, 0.2], (0.2, 0.4], (0.4, 0.6], (0.6, 0.8], (0.8, 1.0]
for very negative, negative, neutral, positive, very positive, respectively.

>SOStr.tx -> Encode the structure of the parse trees. 
>Stree.txt -> Encode the structure of the parse trees. 

Data Extraction:

dataSentence.txt  and Sentiment_lables.txt files are used for loading data.

Mapping Sentiments from pharses to senteces



