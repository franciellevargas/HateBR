# HateBR - Offensive Language and Hate Speech Dataset in Brazilian Portuguese

HateBR is the first large-scale multilayer annotated corpus of Brazilian Instagram comments for hate speech and offensive language detection on the web and social media. The HateBR corpus was collected from Brazilian Instagram comments of political personalities and manually annotated by specialists, being composed of 7,000 documents annotated according to three different layers: a binary classification (offensive versus non-offensive comments), offensiveness-level (highly, moderately, and slightly offensive messages), and nine hate speech targets (xenophobia, racism, homophobia, sexism, religious intolerance, partyism, apology to the dictatorship, antisemitism, and fatphobia). Each comment was annotated by three different annotators and achieved high inter-annotator agreement.


This repository contains the corpus and the best models presented in the article [ref-artigo]. The hateBR.csv file is composed of an offensive language and hate speech annotated corpus, which provides 4 (four) columns as described above:
First column: Text of the Instagram comment.  

Second column:  Binary classification, which consists of offensive (label 1) and non-offensive (label 2) classes. 
Third column:  Offensiveness levels, which consists of  highly (label 3), moderately (label 2), and slightly (label 1) offensive. 
Fourth column: hate targets which consist of  nine different hate groups: xenophobia, racism, homophobia, sexism, religious intolerance, partyism, an apology to the dictatorship, antisemitism, and fatphobia. 


