# Multilingual-STSB

The original STS Benchmark [[1]](#1) consists of train-dev-test splits of 5749, 1500, and 1379 pairs of sentences, respectively, labelled with a similarity score between 0 and 5, from less to more similar. To extend the original English STSb to a multilingual dataset, we translate the STS Benchmark splits from English to 15 languages<sup>[1](#myfootnote1)</sup>. The [Google Translator python package](https://pypi.org/project/google-trans-new/}{https://pypi.org/project/google-trans-new/) is used for this purpose, following the same  procedure that has been largely used in existing related literature [[2]](#2) [[3]](#3) [[4]](#4). In addition, to maintain data quality, translated sentence pairs with a confidence value below 0.7 were dropped. As a result, Dutch is the language with the lowest sentence pairs in development (1483 sentence pairs) and test (1358 sentence pairs) sets. Besides, Google Translator distinguishes two variants of Chinese: simplified and using Mainland Chinese terms (<i>zh-CN</i>), and traditional and using Taiwanese terms (<i>zh-TW</i>).

<a name="myfootnote1"><sup>1</sup>Languages</a>: ar, cs, de, en, es, fr, hi, it, ja, nl, pl, pt, ru, tr, zh-CN, zh-TW

# Data

The data is splitted into train, dev and test sets at "Data" folder in pickle files. You can easily load the data using `read_pickle()` function from `pandas`. 

# References
<a id="1">[1]</a> 
Cer, Daniel, Diab, Mona, Agirre, Eneko, Lopez-Gazpio, Iñigo, & Specia, Lucia. (2017). SemEval-2017 Task 1: Semantic Textual Similarity - Multilingual and Cross-lingual Focused Evaluation. https://doi.org/10.18653/v1/S17-2001

<a id="2">[2]</a> 
Ham, Jiyeon, Choe, Yo Joong, Park, Kyubyong, Choi, Ilji, & Soh, Hyungjoon. (2020). KorNLI and KorSTS: New Benchmark Datasets for Korean Natural Language Understanding.

<a id="3">[3]</a> 
Reimers, Nils, & Gurevych, Iryna. (2020). Making Monolingual Sentence Embeddings Multilingual using Knowledge Distillation.

<a id="4">[4]</a> 
Hu, Junjie, Ruder, Sebastian, Siddhant, Aditya, Neubig, Graham, Firat, Orhan, & Johnson, Melvin. (2020). XTREME: A Massively Multilingual Multi-task Benchmark for Evaluating Cross-lingual Generalization.



