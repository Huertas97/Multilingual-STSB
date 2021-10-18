# Cross-lingual datasets

As mentioned in the paper we have combined the pair-sentences from different languages to create new cross-lingual tasks apart from the monolingual tasks. There are different cross-lingual datasets verison. The number of tasks increase from v1 to v3. 

### Data fields

|      | task     | stsb_test_1_lang1                                                                                                               | stsb_test_2_lang2                                                                                                          |   score_lang2 |
|-----:|:---------|:--------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|--------------:|
|  218 | pl;en    | Kot pije mleko.                                                                                                                 | A white cat is licking and drinking milk kept on a plate.                                                                  |          0.76 |
|   73 | pt;cs    | As pessoas estão dançando lá fora.                                                                                              | Skupina lidí tančí.                                                                                                        |          0.75 |
| 1339 | tr;nl    | Türkiye Başbakanı ile cumhurbaşkanı protestolara yanıt konusunda çatıştı                                                        | De Turkse president roept op tot rust te midden van landelijke protesten                                                   |          0.52 |
| 1347 | it;zh-TW | La Francia avverte che gli estremisti beneficiano della violenza dell'Egitto                                                    | 法國擔心極端分子將從埃及暴力中受益                                                                                         |          0.88 |
|  757 | ar;it    | لقد فهمت الأمر بشكل صحيح.                                                                                                       | Sì, hai capito.                                                                                                            |          1    |
|  462 | nl;de    | Een jonge werper gooit het honkbal.                                                                                             | Ein brauner Hund läuft auf dem Rasen neben einem Zaun.                                                                     |          0    |
|  693 | nl;ru    | U moet uw antwoord alleen baseren op wat u wel weet, en dat is wat u wilt.                                                      | Ответ на вашу проблему заключается в том, что вы на самом деле не знаете, что получаете.                                   |          0.4  |
|  271 | zh-TW;tr | 坐在後院的一個人彈吉他。                                                                                                        | Turuncu bir cipin arkasına binen bir adam.                                                                                 |          0    |
|  910 | es;pl    | La moneda única subió hasta 135,13 yenes, igualando un récord histórico poco después del lanzamiento del euro en enero de 1999. | Wspólna waluta wzrosła do 135,26 jenów, czyli najwyższy poziom od czasu wprowadzenia wspólnej waluty w styczniu 1999 roku. |          0.7  |
|  157 | ar;zh-TW | رجل بصق.                                                                                                                        | 一個男人在說話。                                                                                                           |          0.16 |

### Versions explanations
All these versions include the 15 monolingual tasks (e.g., en;en, es;es, de;de).  
* Version 1 (v1): Multilingual STS Benchmark test split with  31 - 15 = 16 crosslingual tasks. Cross-lingual tasks have always English as first language (i.e., EN;lang)
* Version 2 (v2): Multilingual STS Benchmark test split with  45 - 15 = 30 crosslingual tasks. This v2 is composed of monolingual, EN;lang and lang;EN tasks. 
* Version 3 (v3): Multilingual STS Benchmark test split with  240 - 15 = 225 crosslingual tasks. This v3 is composed of all the possible PERMUTATIONS between languages (lang;lang). 
