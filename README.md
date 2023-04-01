# Subjectivity-Classification.-Identifying-news-and-editorials
Replication and extention of for Alhindi et al. (2020) for course "Mining opinions and arguments".

The  replication and further extension of argumentation features model.

The main goal is to investigate the importance of  article content representation with argumentation features in distinguishing between news and opinion articles.The results of the original model and replication differ as two models were not trained on the same model. However, argumentation features were improving the result of the model almost always. Moreover, the frequency analysis of argumentation features confirms  the relation between argumentative types of sentences and the discourse structure of the articles. The [report](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Subjectivity_Classification.pdf) describes details of the project.

The [Models folder](https://github.com/yerkesoul/Subjectivity-Classification/tree/main/Models) contains the notebooks:

1.[Arg_Features_Bert_Embeddings.ipynb](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Models/Arg_Features_Bert_Embeddings%20(1).ipynb) contains models such as: 
* BERT,
* RNN (3 labels)
* RNN (6 labels)
* BERT+RNN (3 labels)
* BERT+RNN (6 labels)

2.[Vader_POS_merged.ipynb](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Models/Vader_POS_merged%20(1).ipynb)  contains models such as:
* VADER
* POS tagger
* VADER+POS tagger

3.[All_4_models_combined.ipynb](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Models/All_4_models_combined%20(1).ipynb) contains models such as:
* BERT+RNN+ VADER+POS tagger (3 labels)
* BERT+RNN+VADER+POS tagger (6 labels)

The [Extracting features](https://github.com/yerkesoul/Subjectivity-Classification/tree/main/Extracting%20features) contains scripts needed for extracting BERT embeddings and argumentation features:

1.[ExtractingBertEmbeddings.ipynb](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Extracting%20features/ExtractingBertEmbeddings.ipynb)
derives BERT embeddings with [CLS] token representing the whole article.The embeddings are saved separately per ariticle and collected in a folder, further the  folder is wrapped in a zip format.

2.[TraingArgClassification.ipynb](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Extracting%20features/TraingArgClassification.ipynb) file is used to train the BERT  argumentation classification model and the weights are saved  for the later extraction.

3.[ExtractingArgFeatures.ipynb](https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Extracting%20features/ExtractingArgFeatures.ipynb) is needed for prediction and  extraction of arg. features.

[Data ](https://github.com/yerkesoul/Subjectivity-Classification/tree/main/Data) has the file for the dataset preprocessing, however due to data protection law they can not be shown publickly.

Lastly,there is a [Plots.ipynb|(https://github.com/yerkesoul/Subjectivity-Classification/blob/main/Plots.ipynb) which shows the realation of
argumentative types of sentences and the discourse structure of the articles.
