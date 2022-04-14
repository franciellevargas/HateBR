![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/6eabdd240ea21af9c1d26529c2085991b4eb2bc1/.github/locus_dcc_ufmg.png)
![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/aa9d109553c039d1ed619bede851ca2ebaeed8b1/.github/dcc-ufmg.png)
![Screenshot from 2019-08-22 12-36-57](https://github.com/franciellevargas/HateBR/blob/46edf1abad6bd49d90b0e42163bdd0de68bfe408/.github/logo_icmc.png) 




<h2 align="center"> HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese </h2>  

</br>
<p align="justify"> HateBR is the first large-scale expert annotated corpus of Brazilian Instagram comments for hate speech and offensive language detection on the web and social media. The HateBR corpus was collected from Brazilian Instagram comments of political personalities and manually annotated by specialists, being composed of 7,000 documents annotated according to three different layers: a binary classification (offensive versus non-offensive comments), offensiveness-level (highly, moderately, and slightly offensive messages), and nine hate speech targets (xenophobia, racism, homophobia, sexism, religious intolerance, partyism, apology to the dictatorship, antisemitism, and fatphobia). Each comment was annotated by three different annotators and achieved high inter-annotator agreement. At last, baseline experiments were implemented reaching 85% of F1-score outperforming the current literature proposals for the Portuguese language. We hope that the proposed expertly annotated corpus may foster research on hate speech and offensive language detection in the Natural Language Processing area. </p>

---

<p align="justify"> This repository contains the corpus and the best models presented in the article "Building an Expert Annotated Corpus for Brazilian Offensive Language and Hate Speech Detection". The hateBR.csv file is composed of an offensive language and hate speech annotated corpus, which provides 4 (four) columns as described above: </p>

* 1st column: Instagram comment.   
* 2nd column: Offensive language classification, which consists of offensive (label 1) and non-offensive (label 2) labels.
* 3rd column: Offensiveness-level classification, which consists of  highly (label 3), moderately (label 2), and slightly (label 1) offensive. 
* 4rd column: Hate speech classification, which consist of nine different hate target groups: antisemitism (label 1), apology to the dictatorship (label 2), fatphobia (label 3), homophobia (label 4), partyism (label 5), racism (label 6), religious intolerance (label 7), sexism (label 8), and xenophobia (label 9). No hate speech comments was classified such as (label 0).

The following table describes in detail the labels for each layer of classification.
<div align="center">
<table> 
<tr><th>Offensive Language</th><th>Offensiveness Levels</th><th>Hate Speech</th></tr>
<tr><td>

|class|label|total|
|--|--|--|  
|offensive|1|3,500| 
|non-offensive|0|3,500| 

</td><td>

|class|label|total|
|--|--|--|
|highly|3|778|
|moderately|2|1,044|
|slightly|1|1,678|
|non-offensive|0|3,500|
  
</td><td>

|class|label|total|  
|--|--|--|  
|antisemitism|1|2|
|apology for the dictatorship|2|32|
|fatphobia|3|27|
|homophobia|4|17|
|partyism|5|496|
|racism|6|8|
|religious intolerance|7|47|
|sexism|8|97|
|xenophobia|9|1|
|non-hate |-1|2,773|
|non-offensive|0|3,500|

</td></tr></table>
</div>

</br>

In addition, we also provide baseline machine learning results for both task: offensive language and hate speech detection. The best obtained models is available here in .pkl files. File names are organized as `[classification (offensive or hate)_representation (ngram or tfidf)_algorithms (nb, svm, mlp or lr)]`. For example, the file *offensive_tfidf_svm.pkl* presents the model about offensive detection with tf-idf representation using the support vector machine algorithm.

</br>

CITING

*Vargas, F.A., Carvalho, I., Góes, F. R., Pardo, T.A.S., Benevenuto, F. (2022). HateBR: large expert annotated corpus of Brazilian Instagram comments for offensive language and hate speech detection. Proceedings of the 13th International Conference on Language Resources and Evaluation (LREC 2022) , pp 1-10. Marseille, France. Association for Computational Linguistics (ACL).



