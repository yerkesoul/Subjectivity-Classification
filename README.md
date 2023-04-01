# Subjectivity-Classification.-Identifying-news-and-editorials
Replication and extention of for Alhindi et al. (2020) for course "Mining opinions and arguments".

The  replication and further extension of argumentation features model.

The main goal is to investigate the importance of  article content representation with argumentation features in distinguishing between news and opinion articles.The results of the original model and replication differ as two models were not trained on the same model. However, argumentation features were improving the result of the model almost always. Moreover, the frequency analysis of argumentation features confirms  the relation between argumentative types of sentences and the discourse structure of the articles.

The "Models" folder contains the notebooks:
1.Arg_Features_Bert_Embeddings.ipynb contains models such as: 
* BERT,
* RNN (3 labels)
* RNN (6 labels)
* BERT+RNN (3 labels)
* BERT+RNN (6 labels)
2.Vader_POS_merged.ipynb  contains models such as:
* VADER
* POS tagger
* VADER+POS tagger
3.All_4_models_combined.ipynb contains models such as:
* BERT+RNN+ VADER+POS tagger (3 labels)
* BERT+RNN+VADER+POS tagger (6 labels)
