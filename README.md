[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7681302.svg)](https://doi.org/10.5281/zenodo.10794024)

<h2 align="center"> HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese </h2>  

</br>
<p align="justify"> HateBR is the first large-scale expert annotated dataset of Brazilian Instagram comments for abusive language detection on the web and social media. The HateBR was collected from Brazilian Instagram comments of politicians and manually annotated by specialists. It is composed of 7,000 documents annotated according to three different layers: a binary classification (offensive versus non-offensive comments), offensiveness-level (highly, moderately, and slightly offensive messages), and 9 (nine) hate speech targets (xenophobia, racism, homophobia, sexism, religious intolerance, partyism, apology for the dictatorship, antisemitism, and fatphobia). Each comment was annotated by three different annotators and achieved high inter-annotator agreement. Furthermore, baseline experiments were implemented reaching 85% of the F1-score outperforming the current literature dataset baselines for the Portuguese language. We hope that the proposed expert annotated dataset may foster research on hate speech detection in the Natural Language Processing area. </p>

---

<p align="justify"> This repository contains the corpus and the best models presented in the paper (see section "citing"). <b>HateBr.csv file</b> provides 4 (four) columns as described above: </p>

* **1st column**: Instagram comments.   
* **2nd column**: Offensive language classification is divided into offensive comments versus non-offensive comments.
* **3rd column**: Offensiveness-level classification is divided into highly offensive, moderately offensive, and slightly offensive. 
* **4th column**: Hate speech classification is divided into 9 (nine) different hate speech targets: antisemitism, apology for the dictatorship, fatphobia, homophobia, partyism, racism, religious intolerance, sexism, and xenophobia. At last, offensive & no hate speech comments were also classified.

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

In addition, we also provide baseline machine learning results for both tasks: offensive language and hate speech detection. The best-obtained models are available here in .pkl files. File names are organized as `[classification (offensive or hate)_representation (ngram or tfidf)_algorithms (nb, svm, mlp or lr)]`. For example, the file *offensive_tfidf_svm.pkl* presents the model of offensive detection with tf-idf representation using the support vector machine algorithm.

</br>


<h2 align="left"> CITING </h2>

<p align="justify">
Vargas, F., Carvalho, I., Góes, F. R., Pardo, T.A.S., Benevenuto, F. (2022). <b>HateBR: large expert annotated corpus of Brazilian Instagram comments for offensive language and hate speech detection</b>. Proceedings of the 13th International Conference on Language Resources and Evaluation (LREC 2022), pp.7174–7183. Marseille, France. https://aclanthology.org/2022.lrec-1.777/
</p>

<br>
<p align="justify">
Vargas, F., Carvalho, I., Pardo, T.A.S., Benevenuto, F. (2024). <b>Context-Aware and Expert Data Resources for Brazilian Portuguese Hate Speech Detection</b>. 
Natural Language Processing Journal. Cambridge University Press. pp.1-22. https://www.cambridge.org/core/journals/natural-language-processing/article/contextaware-and-expert-data-resources-for-brazilian-portuguese-hate-speech-detection/7D9019ED5471CD16E320EBED06A6E923#.
</p>

<br>

<h2 align="left"> BIBTEX </h2>

<p align="justify">
  @inproceedings{vargas-etal-2022-hatebr,
    title = "{H}ate{BR}: A Large Expert Annotated Corpus of {B}razilian {I}nstagram Comments for Offensive Language and Hate Speech Detection",
    author = "Vargas, Francielle  and
      Carvalho, Isabelle  and
      Rodrigues de G{\'o}es, Fabiana  and
      Pardo, Thiago  and
      Benevenuto, Fabr{\'\i}cio",
    booktitle = "Proceedings of the 13th Conference on Language Resources and Evaluation (LREC 2022)",
    year = "2022",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://aclanthology.org/2022.lrec-1.777",
    pages = "7174--7183",
    }
</p>

<br></br>

 @article{Vargas_Carvalho_Pardo_Benevenuto_2024, 
 author={Vargas, Francielle and Carvalho, Isabelle and Pardo, Thiago A. S. and Benevenuto, Fabrício},
 title={Context-aware and expert data resources for Brazilian Portuguese hate speech detection}, 
 DOI={10.1017/nlp.2024.18}, 
 journal={Natural Language Processing},  
 year={2024}, 
 pages={1–22},
 url={https://www.cambridge.org/core/journals/natural-language-processing/article/contextaware-and-expert-data-resources-for-brazilian-portuguese-hate-speech-detection/7D9019ED5471CD16E320EBED06A6E923#},
 } 
 <div></div>

<br></br>

<p align="justify">
  @inproceedings{vargas-etal-2022-hatebr,
    title = "HateBRXplain: A Benchmark Dataset with Human-Annotated Rationales for Explainable Hate Speech Detection in Brazilian Portuguese",
    author = "Salles, Isadora
      Vargas, Francielle  and
      Benevenuto, Fabr{\'\i}cio",
    booktitle = "Proceedings of the 31th International Conference on Computational Linguistics (COLING 2025)",
    year = "2025",
    address = "Abu Dhabi, UAE",
    publisher = "Association for Computational Linguistics",
    url = "",
    pages = "",
    }
</p>

<br></br>

<h2 align="left"> FUNDING </h2>

![SSC-logo-300x171](https://github.com/franciellevargas/franciellevargas.github.io/blob/fc03a6672ab2937e413e4508a5061abed4a66098/img/fapesp.jpg)
</br>
