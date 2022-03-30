<h2 align="center"> HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese </h2>  

</br>
HateBR is the first large-scale multilayer annotated corpus of Brazilian Instagram comments for hate speech and offensive language detection on the web and social media. The HateBR corpus was collected from Brazilian Instagram comments of political personalities and manually annotated by specialists, being composed of 7,000 documents annotated according to three different layers: a binary classification (offensive versus non-offensive comments), offensiveness-level (highly, moderately, and slightly offensive messages), and nine hate speech targets (xenophobia, racism, homophobia, sexism, religious intolerance, partyism, apology to the dictatorship, antisemitism, and fatphobia). Each comment was annotated by three different annotators and achieved high inter-annotator agreement.

---

This repository contains the corpus and the best models presented in the article "Building an Expert Annotated Corpus for Brazilian Offensive Language and Hate Speech Detection" *(under review by a scientific journal)*. The hateBR.csv file is composed of an offensive language and hate speech annotated corpus, which provides 4 (four) columns as described above:
* First column: Text of the Instagram comment.  
* Second column:  Binary classification, which consists of offensive (label 1) and non-offensive (label 2) classes.
* Third column:  Offensiveness levels, which consists of  highly (label 3), moderately (label 2), and slightly (label 1) offensive.  
* Fourth column: hate targets which consist of  nine different hate groups: xenophobia, racism, homophobia, sexism, religious intolerance, partyism, an apology to the dictatorship, antisemitism, and fatphobia.

The following table describes the labels for each class.
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
|apology to the dictatorship|2|32|
|fatphobia|3|27|
|homophobia|4|17|
|partyism|5|496|
|racism|6|8|
|religious intolerance|7|47|
|sexism|8|97|
|xenophobia|9|1|
|non-hate & offensive|-1|2,773|
|non-offensive|0|3,500|

</td></tr></table>
</div>

</br>

In addition to the corpus, the .pkl files refer to the most accurate models. 
File names are organized as `[classification (offensive or hateful)_representation (ngram or tfidf)_algorithms (nb, svm, mlp or lr)]`. 
For example, the file *offensive_tfidf_svm.pkl* presents the model about offensive detection with tf-idf representation using the support vector machine algorithm.

CITING

Vargas, F.A., Carvalho, I., Góes, F. R., Pardo, T.A.S., Benevenuto, F. (2022). Building an Expert Annotated Corpus for Brazilian Offensive Language and Hate Speech Detection. In Natural Language Engineering Journal, pp. Association for Computational Linguistics (ACL). 

