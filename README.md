<h3 align="center"> HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese </h3>  

</br>

This repository contains the corpus and the best models presented in the article [ref-artigo]. The hateBR.csv file is composed of an offensive language and hate speech annotated corpus, which provides 4 (four) columns as described above:
* First column: Text of the Instagram comment.  
* Second column:  Binary classification, which consists of offensive (label 1) and non-offensive (label 2) classes. 
* Third column:  Offensiveness levels, which consists of  highly (label 3), moderately (label 2), and slightly (label 1) offensive. 
* Fourth column: hate targets which consist of  nine different hate groups: xenophobia, racism, homophobia, sexism, religious intolerance, partyism, an apology to the dictatorship, antisemitism, and fatphobia. 

<div align="center">
<table> 
<tr><th>Offensive Language</th><th>Offensiveness Levels</th><th>Hate Speech</th></tr>
<tr><td>

|class|label| 
|--|--|  
|offensive|1|
|non-offensive|0|

</td><td>

|class|label|
|--|--|
|highly|3|
|moderately|2|
|slightly|1|
|non-offensive|0|
  
</td><td>

|class|label|  
|--|--|  
|antisemitism|1|
|apology to the dictatorship|2|
|fatphobia|3|
|homophobia|4|
|partyism|5|
|racism|6|
|religious intolerance|7|
|sexism|8|
|xenophobia|9|
|non-hate & offensive|-1|
|non-offensive|0|

</td></tr></table>
</div>

</br>

In addition to the corpus, the .pkl files refer to the most accurate models. 
File names are organized as `[classification (offensive or hateful)_representation (ngram or tfidf)_algorithms (nb, svm, mlp or lr)]`. 
For example, the file *offensive_tfidf_svm.pkl* presents the model about offensive detection with tf-idf representation using the support vector machine algorithm.
