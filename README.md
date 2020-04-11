# awesome-nlp-polish
A curated list of resources dedicated to Natural Language Processing (NLP) in polish. Models, tools, datasets.

![Awesome NLP Polish Logo](/Awesome_nlp_polish.png)


## Models (Embeddings)

* [PolBert](https://github.com/kldarek/polbert) - Polish BERT model. Model was trained with code provided in Google BERT's github repository. Merge with [huggingface/Transformers](https://huggingface.co/dkleczek/bert-base-polish-uncased-v1)
* [Polish Roberta Model](https://github.com/sdadas/polish-nlp-resources?fbclid=IwAR0tv_YbuBwfFirGFQvqaGdCSL6BV-9pNW8Wm3gkGiyXNajE_M9tpY0hIaM#roberta) - model was trained on a corpus consisting of Polish Wikipedia dump, Polish books and articles, Polish Parliamentary Corpus
* Allegro BERT - It has not been publish yet (12.2019) - but there is a poster - https://conference.mlinpl.org/pdf/CfC_AllPosters.pdf
* [SlavicBert - multilingual BERT model](https://github.com/deepmipt/Slavic-BERT-NER) -BERT, Slavic Cased: 4 languages(Bulgarian,Czech, Polish, Russian), 12-layer, 768-hidden, 12-heads, 110M parameters, 600Mb. There is also another SlavicBert model http://docs.deeppavlov.ai/en/master/features/models/bert.html but I have problems to convert it to pytorch.



* [ELMO embeddings](https://clarin-pl.eu/dspace/handle/11321/690?show=full) - A model of ELMo embeddings for Polish language trained on large textual corpora (KGR10).
* [Zalando Flair polish models](https://github.com/flairNLP/flair/blob/master/resources/docs/embeddings/FLAIR_EMBEDDINGS.md) - Contextual string embeddings that capture latent syntactic-semantic information that goes beyond standard word embeddings. There are two models "pl-forward and pl-backward" 
* [IPIPAN Word2vec polish models](http://dsmodels.nlp.ipipan.waw.pl/w2v.html)
* [Wrocław University of Science and Technology Word2Vec](https://clarin-pl.eu/dspace/handle/11321/442) - Distributional language models for Polish trained on different corpora (KGR10, NKJP, Wikipedia).
* FastText polish model FB - train on: [Common Crawl](https://github.com/facebookresearch/fastText/blob/master/docs/crawl-vectors.md), [Wikipedia](https://github.com/facebookresearch/fastText/blob/master/docs/pretrained-vectors.md)
* [FastText KGR10 polish model binary](https://clarin-pl.eu/dspace/handle/11321/600)
* [Universal Sentence Encoder Multilingual](https://tfhub.dev/google/universal-sentence-encoder-multilingual-large/3) - sentence embeddings, it covers 16 languages (including Polish)

* [BPEmb: Subword Embeddings includes polish](https://nlp.h-its.org/bpemb/) - easy to use with [Flair](https://github.com/flairNLP/flair/blob/master/resources/docs/embeddings/BYTE_PAIR_EMBEDDINGS.md)


## Language processing resources and libs

* [Morfologik](https://github.com/morfologik/morfologik-stemming) (Java) and [pyMorfologik](https://github.com/dmirecki/pyMorfologik) (Python wrapper) - dictionary-based morphological analyzer
* [Morfeusz](http://morfeusz.sgjp.pl/download/) - morphological analyzer. See also [Elasticsearch plugin](https://github.com/allegro/elasticsearch-analysis-morfologik)
* [Stempel](https://github.com/dzieciou/pystempel) (Python port) - algorithmic stemmer. See also [Elasticsearch plugin](https://www.elastic.co/guide/en/elasticsearch/plugins/current/analysis-stempel.html)
* [scaCy for Polish](http://spacypl.sigmoidal.io/) - extend spaCy, a popular production-ready NLP library, to fully support Polish language.
* [KRNNT Polish morphological tagger ](https://github.com/kwrobel-nlp/krnnt) - KRNNT is a morphological tagger for Polish based on recurrent neural networks [Paper](http://ltc.amu.edu.pl/book2017/papers/PolEval1-6.pdf)
* [Stanza](https://stanfordnlp.github.io/stanza/) (Python) - NLP analysis package from Stanford University 

* A curated list of [Polish abbreviations for NLTK sentence tokenizer](https://gist.github.com/ksopyla/f05fe2f48bbc9de895368b8a7863b5c3) based on Wikipedia text


## Useful articles or projects

* Github Repo with list of polish: word embeddings and language models (Word2vec, fasttext, Glove, Elmo) -  https://github.com/sdadas/polish-nlp-resources
* [Polish Word Embeddings Review](https://github.com/Ermlab/polish-word-embeddings-review) - Evaluation of polish word embeddings: word2vec, fastext etc. prepared by various research groups. Evaluation is done by words analogy task. 
* [Polish Sentence Evaluation](https://github.com/sdadas/polish-sentence-evaluation)- contains evaluation of eight sentence representation methods (Word2Vec, GloVe, FastText, ELMo, Flair, BERT, LASER, USE) on five polish linguistic tasks
* [TRAINING ROBERTA FROM SCRATCH - THE MISSING GUIDE](https://zablo.net/blog/post/training-roberta-from-scratch-the-missing-guide-polish-language-model/) - complete user guide for trainning Roberta model with use of Huggingface/Transformers for polish



## Datasets

### Task oriented datsets

* [The KLEJ (Kompleksowa Lista Ewaluacji Językowych) benchmark is a set of nine evaluation tasks for the Polish language understanding.](https://klejbenchmark.com/index.html)
* PolEval datasets - 
    * Hate speech classification -distinguish between normal/non-harmful tweets (class: 0) and tweets that contain any kind of harmful information (class: 1) [[PolEval 2019 Task6](http://2019.poleval.pl/index.php/tasks/task6)]  [[mirror GDrive](https://drive.google.com/drive/folders/1Dp7h9FrejUGK4jOeMsuxObiwP5h4x6q6?usp=sharing)]
* [Polish CDSCorpus](http://zil.ipipan.waw.pl/Scwad/CDSCorpus) - The dataset for compositional distributional semantics. Polish CDSCorpus consists of 10K Polish sentence pairs which are human-annotated for semantic relatedness and entailment. 
* [Wroclaw Corpus of Consumer Reviews Sentiment (WCCRS)](https://clarin-pl.eu/dspace/handle/11321/700) - corpus of Polish reviews annotated with sentiment at the level of the whole text (*text*) and at the level of sentences (*sentence*) for the following domains: hotels, medicine, products and university (reviews*)    
* [Ermlab Opineo dataset](https://github.com/Ermlab/pl-sentiment-analysis)- opineo reviews - [GDrive](https://drive.google.com/file/d/1vXqUEBjUHGGy3vV2dA7LlvBjjZlQnl0D/view?usp=sharing)
* HateSpeech corpus contains over 2000 posts crawled from public Polish web.http://zil.ipipan.waw.pl/HateSpeech
* [Polish analogy dataset](https://dl.fbaipublicfiles.com/fasttext/word-analogies/questions-words-pl.txt) - example: "Ateny Grecja Bagdad Irak" - useful for word embeddings evaluation
* [NKJP](http://nkjp.pl/index.php?page=0&lang=1) - National Corpus of Polish. It contains classic literature, daily newspapers, specialist periodicals and journals, transcripts of conversations, and a variety of short-lived and internet texts. Only a small sub-corpus is available for [download](http://clip.ipipan.waw.pl/NationalCorpusOfPolish?action=AttachFile&do=get&target=NKJP-PodkorpusMilionowy-1.2.tar.gz) (GNU GLP v.3). Direct contact and maybe necessary to get the full corpus. 
* [PolEmo 2.0 Sentiment Analysis Dataset for CoNLL](https://clarin-pl.eu/dspace/handle/11321/710)


### Raw texts
* [OSCAR or Open Super-large Crawled ALMAnaCH coRpus](https://traces1.inria.fr/oscar/#corpus) -  is a huge multilingual corpus obtained by language classification and filtering of the Common Crawl corpus. Contains 109GB or 49GB of polish text.
* [Polish Wikipedia dump](https://dumps.wikimedia.org/plwiki/) - regular monthly copy of Polish wikipedia. More then 4GB of text.

* [Opus - the open parallel corpus](http://opus.nlpl.eu/) - you can select languages and download only polish file
    * [Polish OpenSubtitles v2018](http://opus.nlpl.eu/OpenSubtitles-v2018.php) - sentences 45.9M, polish tokens 287.1M ,collection of translated movie subtitles from [opensubtitles](http://www.opensubtitles.org/) [raw txt corpus (unpacked 7.2GB)](https://object.pouta.csc.fi/OPUS-OpenSubtitles/v2018/mono/pl.txt.gz) [tokenized txt corpus (unpacked 7.6GB)](https://object.pouta.csc.fi/OPUS-OpenSubtitles/v2018/mono/pl.tok.gz).
    * [ParaCrawl v5](http://opus.nlpl.eu/ParaCrawl-v5.php) sentences 6.4M, polish tokens 157.1M [raw txt corpus (unpacked 1.1GB)](https://object.pouta.csc.fi/OPUS-ParaCrawl/v5/mono/pl.txt.gz) [tokenized txt corpus](https://object.pouta.csc.fi/OPUS-ParaCrawl/v5/mono/pl.tok.gz)


* [Polish Parliamentary Corpus](http://clip.ipipan.waw.pl/PPC) text from proceedings of Polish Parliament, Sejm and Senate


## Reserch papers

* "Evaluation of Sentence Representations in Polish" - Sławomir Dadas, Michał Perełkiewicz, Rafał Poswiata 2019 https://arxiv.org/pdf/1910.11834.pdf
* "Multi-level analysis and recognition of the text sentiment on the example of consumer opinions" - Kocoń Jan, Zaśko-Zielińska Monika, Miłkowski Piotr, 2019


## Contributors

