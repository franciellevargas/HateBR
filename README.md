[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7681302.svg)](https://doi.org/10.5281/zenodo.10794024)

<h2 align="center"> HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese </h2>  

</br>
<p align="justify"> HateBR is the first large-scale expert annotated dataset of Brazilian Instagram comments for abusive language detection on the web and social media. The HateBR was collected from Brazilian Instagram comments of politicians and manually annotated by specialists. It is composed of 7,000 documents annotated according to three different layers: a binary classification (offensive versus non-offensive comments), offensiveness-level (highly, moderately, and slightly offensive messages), and 9 (nine) hate speech targets (xenophobia, racism, homophobia, sexism, religious intolerance, partyism, apology for the dictatorship, antisemitism, and fatphobia). Each comment was annotated by three different expert annotators and achieved high inter-annotator agreement. Furthermore, baseline experiments were implemented outperforming the current literature dataset baselines for the Portuguese language. We hope that the proposed expert annotated dataset may foster research on hate speech detection in the Natural Language Processing area. </p>

</br>
<h3 align="center">***UPDATE***: <u>HateBR 2.0</u> AND <u>HateBRXplain</u> VERSIONS ARE AVAILABLE.</h3> 
</br>
  
<p align="justify"> This repository contains the corpus and the best models presented in the LREC's paper (see section "CITING / BIBTEX"). 
  
The following table describes in detail the binary class:
<div align="center">
<table> 
<tr><th>Offensive Language</th></tr>
<tr><td>

|class|label|total|
|--|--|--|  
|offensive|1|3,500| 
|non-offensive|0|3,500| 
**Total** | | **7,000**|


</td><td>

</table>
</div>

</br>

In addition, we also provide baseline machine learning results for both tasks: offensive language and hate speech detection. The best-obtained models are available here in .pkl files. File names are organized as `[classification (offensive or hate)_representation (ngram or tfidf)_algorithms (nb, svm, mlp or lr)]`. For example, the file *offensive_tfidf_svm.pkl* presents the model of offensive detection with tf-idf representation using the support vector machine algorithm.

</br>


<h2 align="left"> CITING / BIBTEX </h2>

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
    author = "Salles, Isadora and
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

![SSC-logo-300x171](https://github.com/franciellevargas/franciellevargas.github.io/blob/fc03a6672ab2937e413e4508a5061abed4a66098/img/google-logo-menor.png)
![SSC-logo-300x171](https://github.com/franciellevargas/franciellevargas.github.io/blob/fc03a6672ab2937e413e4508a5061abed4a66098/img/fapesp.jpg)

</br>
