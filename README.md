![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/5611312b1573cb1e5689fae64ab4ede88502ed78/.github/Logo-DCCUFMG.jpg)
![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/7e5fe34063f89296b17f8c255b89360dfef75761/.github/icmc.png)     ![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/1c2ecbc54df5719102d068370b3eca9dacea8334/.github/locus_media.png)

<h2 align="center"> HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese </h2>  

</br>
<p align="justify"> HateBR is the first large-scale expert annotated dataset of Brazilian Instagram comments for abusive language detection on the web and social media. The HateBR was collected from Brazilian Instagram comments of politicians and manually annotated by specialists. It is composed of 7,000 documents annotated according to three different layers: a binary classification (offensive versus non-offensive comments), offensiveness-level (highly, moderately, and slightly offensive messages), and nine hate speech groups (xenophobia, racism, homophobia, sexism, religious intolerance, partyism, apology for the dictatorship, antisemitism, and fatphobia). Each comment was annotated by three different annotators and achieved high inter-annotator agreement. Furthermore, baseline experiments were implemented reaching 85% of F1-score outperforming the current literature dataset baselines for the Portuguese language. We hope that the proposed expert annotated dataset may foster research on hate speech detection in the Natural Language Processing area. </p>

---

<p align="justify"> This repository contains the corpus and the best models presented in the paper (see section "citing"). HateBr.csv file is composed of an offensive language and hate speech annotated corpus, which provides 4 (four) columns as described above: </p>

* **1st column**: Instagram comments.   
* **2nd column**: Offensive language classification divided into offensive comments versus non-offensive comments.
* **3rd column**: Offensiveness-level classification divided into highly offensive, moderately offensive, and slightly offensive. 
* **4th column**: Hate speech classification divided into nine different hate groups: antisemitism, apology for the dictatorship, fatphobia, homophobia, partyism, racism, religious intolerance, sexism, and xenophobia. At last, offensive & no hate speech comments was also classified.

The following table describes in detail the labels for each proposed layer of annotation:
<div align="center">
<table> 
<tr><th>Offensive Language</th><th>Offensiveness Levels</th><th>Hate Speech</th></tr>
<tr><td>

|class|label|total|
|--|--|--|  
|offensive|1|3,500| 
|non-offensive|0|3,500| 
**Total** | | **7,000**|


</td><td>

|class|label|total|
|--|--|--|
|highly|3|778|
|moderately|2|1,044|
|slightly|1|1,678|
|non-offensive|0|3,500|
|**Total**||**7,000**|
  
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
|offensive & non-hate speech |-1|2,773|
|non-offensive|0|3,500|
|**Total**||**7,000**|

</td></tr></table>
</div>

</br>

In addition, we also provide baseline machine learning results for both task: offensive language and hate speech detection. The best obtained models is available here in .pkl files. File names are organized as `[classification (offensive or hate)_representation (ngram or tfidf)_algorithms (nb, svm, mlp or lr)]`. For example, the file *offensive_tfidf_svm.pkl* presents the model about offensive detection with tf-idf representation using the support vector machine algorithm.

</br>


<h2 align="left"> CITING </h2>

<p align="justify">
Vargas, F., Carvalho, I., Góes, F. R., Pardo, T.A.S., Benevenuto, F. (2022). HateBR: large expert annotated corpus of Brazilian Instagram comments for offensive language and hate speech detection. Proceedings of the 13th International Conference on Language Resources and Evaluation (LREC 2022), pp.7174–7183. Marseille, France. Association for Computational Linguistics (ACL). 

</p>


<br>

<h2 align="left"> FUNDING </h2>

![SSC-logo-300x171](https://github.com/franciellevargas/franciellevargas.github.io/blob/9f2aba738836e85dbedbe969010ed8593d1c0d69/img/sinch-logo.png)
![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/e5ccb9cd6b43c26edacb2c4abd32fd75f8a574a2/.github/logo_novo_english.gif)
![SSC-logo-300x171](https://github.com/franciellevargas/HateBR/blob/1c6044026c8617de939f562c83e1e45c19ca8c89/.github/cnpq.png)

</br>
