# Cross-lingual datasets

As mentioned in the paper we have combined the pair-sentences from different languages to create new cross-lingual tasks apart from the monolingual tasks. There are different cross-lingual datasets verison. The number of tasks increase from v1 to v3. 

### Data fields

Take a look to this random sample data from Version 3 (v3)

|      | task   | stsb_test_1_lang1                                                                                                                  | stsb_test_2_lang2                                                                                                                         |   score_lang2 |
|-----:|:-------|:-----------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------|--------------:|
|  661 | hi;es  | कॉफी केवल पॉट से एल्यूमीनियम उठाता है, क्योंकि कॉफी अम्लीय है।                                                                              | Una idea es limpiar los residuos de café de la cafetera.                                                                                  |          0.2  |
|  750 | fr;es  | Cela dépend de ce que vous voulez avoir dans votre réservoir.                                                                      | Depende de lo que quieras lograr.                                                                                                         |          0.4  |
| 1055 | ja;ar  | BlueCore3-Multimediaには、ステレオオーディオ用のデュアルADCおよびDACを備えた16ビットステレオオーディオコーデックが含まれています。 | يحتوي BlueCore3-Multimedia على منصة DSP مفتوحة للمعالج المشترك ويتضمن أيضًا برنامج ترميز صوتي استريو 16 بت مع ADC و DAC مزدوج لصوت ستيريو. |          0.72 |

### Versions explanations
All these versions include the 15 monolingual tasks (e.g., en;en, es;es, de;de).  
* Version 1 (v1): Multilingual STS Benchmark test split with  31 - 15 = 16 crosslingual tasks. Cross-lingual tasks have always English as first language (i.e., EN;lang)
* Version 2 (v2): Multilingual STS Benchmark test split with  46 - 15 = 31 crosslingual tasks. This v2 is composed of monolingual, EN;lang and lang;EN tasks. 
* Version 3 (v3): Multilingual STS Benchmark test split with  240 - 15 = 225 crosslingual tasks. This v3 is composed of all the possible PERMUTATIONS between languages (lang;lang). 
