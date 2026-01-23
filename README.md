# GEC Information

### Policy
- This repository aims to collect and categorize GEC (Grammatical Error Correction) papers.
- Unlike [NLP-progress](http://nlpprogress.com/), GEC-Info does not consider performance on benchmarks.
  - Authors and conferences are also not be considered.
- The papers are limited to refereed papers in international conferences for now.
  - This is not the case for survey papers.

### Contributing
- Pull Requests for adding papers are accepted. Please make a commit changing only lines regarding the addition of papers (and take care of changing by auto-formatting).
- You can also request to add papers as an [issue](https://github.com/gotutiyan/GEC-Info/issues).

It can also be viewed on [GitHub Pages](https://gotutiyan.github.io/GEC-Info/)

# Overview

* [Surveys](https://github.com/gotutiyan/GEC-Info#surveys)
* [Shared Tasks](https://github.com/gotutiyan/GEC-Info#shared-tasks)
* [Libraries](https://github.com/gotutiyan/GEC-Info#libraries)
* [Datasets](https://github.com/gotutiyan/GEC-Info#datasets)
  * [For Training](https://github.com/gotutiyan/GEC-Info#for-training-real-data)
  * [For Evaluation](https://github.com/gotutiyan/GEC-Info#for-evaluation)
* [Performance Measures](https://github.com/gotutiyan/GEC-Info#performance-measures)
  * [Reference-based](https://github.com/gotutiyan/GEC-Info#reference-based)
  * [Reference-less](https://github.com/gotutiyan/GEC-Info#reference-less)
  * [Meta-evaluation](https://github.com/gotutiyan/GEC-Info#meta-evaluatoin)
* [Quality Estimation](https://github.com/gotutiyan/GEC-Info#quality-estimation)
* [Models](https://github.com/gotutiyan/GEC-Info#models)
  * [Before Neural](https://github.com/gotutiyan/GEC-Info#before-neural-eg-smt)
  * [Encoder-Decoder](https://github.com/gotutiyan/GEC-Info#encoder-decoder)
  * [Tagging / Non-autogressive](https://github.com/gotutiyan/GEC-Info#tagging--non-autogressive)
  * [Large Language Model](https://github.com/gotutiyan/GEC-Info#large-language-model)
* [Ensembles / Post-processing](https://github.com/gotutiyan/GEC-Info#ensembles--post-processing)
* [Strategies](https://github.com/gotutiyan/GEC-Info#strategies)
* [Data Augmentation](https://github.com/gotutiyan/GEC-Info#data-augmentation)
* [Analyses](https://github.com/gotutiyan/GEC-Info#analyses)
* [Other Tools](https://github.com/gotutiyan/GEC-Info#other-tools)
* [Spoken Domain](https://github.com/gotutiyan/GEC-Info#spoken-domain)
* [Applications](https://github.com/gotutiyan/GEC-Info#applications)
* [Projects](https://github.com/gotutiyan/GEC-Info#projects)
* [Other Materials](https://github.com/gotutiyan/GEC-Info#other-materials)
* [Related Tasks](https://github.com/gotutiyan/GEC-Info#related-tasks)
  * [Grammatical Error Detection](https://github.com/gotutiyan/GEC-Info#grammatical-error-detection)
  * [Feedback Comment Generation](https://github.com/gotutiyan/GEC-Info#feedback-comment-generation)
* [Other Languages](https://github.com/gotutiyan/GEC-Info#other-languages)
  * [Arabic](https://github.com/gotutiyan/GEC-Info#arabic)
  * [Bangla](https://github.com/gotutiyan/GEC-Info#bangla)
  * [Chinese](https://github.com/gotutiyan/GEC-Info#chinese)
  * [Czech](https://github.com/gotutiyan/GEC-Info#czech)
  * [Geek](https://github.com/gotutiyan/GEC-Info#geek)
  * [German](https://github.com/gotutiyan/GEC-Info#german)
  * [Hindi](https://github.com/gotutiyan/GEC-Info#hindi)
  * [Icelandic](https://github.com/gotutiyan/GEC-Info#icelandic)
  * [Japanese](https://github.com/gotutiyan/GEC-Info#japanese)
  * [Korean](https://github.com/gotutiyan/GEC-Info#korean)
  * [Lithuanian](https://github.com/gotutiyan/GEC-Info#lithuanian)
  * [Romain](https://github.com/gotutiyan/GEC-Info#romain)
  * [Russian](https://github.com/gotutiyan/GEC-Info#russian)
  * [Spanish](https://github.com/gotutiyan/GEC-Info#spanish)
  * [Turkish](https://github.com/gotutiyan/GEC-Info#turkish)
  * [Ukrainian](https://github.com/gotutiyan/GEC-Info#ukrainian)


# Surveys

|Title|Year|Page|Note|
|:--|:--|:--|:--|
|"Automated Grammatical Error Correction: A Comprehensive Review"|2017|[[paper]](https://www.journals.nust.edu.pk/index.php/njes/article/download/219/100)||
|"A Comprehensive Survey of Grammar Error Correction"|2020|[[paper]](https://arxiv.org/abs/2005.06600)||
|"Recent Trends in the Use of Deep Learning Models for Grammar Error Handling" |2020|[[paper]](https://arxiv.org/abs/2009.02358)||
|"Grammatical Error Correction: A Survey of the State of the Art"|2022|[[paper]](https://arxiv.org/abs/2211.05166)||

# Shared Tasks

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|HOO 2011|2011| [[paper]](https://aclanthology.org/W11-2838/)| [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2011)|
|HOO 2012|2012| [[paper]](https://aclanthology.org/W12-2006)| [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2012-shared-task-on-preposition-and-determiner-error-correction)|
|CoNLL-2013|2013| [[paper]](https://aclanthology.org/W13-3601/)| [[website]](https://www.comp.nus.edu.sg/~nlp/conll13st.html)|
|CoNLL-2014|2014| [[paper]](https://aclanthology.org/W14-1701/)| [[website]](https://www.comp.nus.edu.sg/~nlp/conll14st.html) [[system outputs]](https://www.comp.nus.edu.sg/~nlp/conll14st/official_submissions.tar.gz)|
|BEA-2019|2019| [[paper]](https://aclanthology.org/W19-4406/)| [[website]](https://www.cl.cam.ac.uk/research/nl/bea2019st/) [[system outpus]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/system_output.bea19.tar.gz)|

# Libraries

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|UnifiedGEC|2025|[UnifiedGEC: Integrating Grammatical Error Correction Approaches for Multi-languages with a Unified Framework](https://aclanthology.org/2025.coling-demos.5/)|[[code]](https://github.com/AnKate/UnifiedGEC)|
|gec-metrics|2025|[gec-metrics: A Unified Library for Grammatical Error Correction Evaluation](https://aclanthology.org/2025.acl-demo.50/)|[[code]](https://github.com/gotutiyan/gec-metrics)|

# Datasets

### For Training (Real Data)

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|EFCamDat|2014| [[Automatic Linguistic Annotation ofLarge Scale L2 Databases: The EF-Cambridge Open Language Database(EFCamDat)]](https://www.semanticscholar.org/paper/Automatic-Linguistic-Annotation-ofLarge-Scale-L2-Geertzen-Alexopoulou/3261659127bebca4d805e8592906b37ece8d0ca3) [[The EF Cambridge Open Language Database (efcamdat) Information for Users]](https://corpus.mml.cam.ac.uk/faq/EFCamDat-Intro_release2.pdf)| [[download v2]](https://philarion.mml.cam.ac.uk)|
|GitHub Typo Corpus| 2019|[[GitHub Typo Corpus: A Large-Scale Multilingual Dataset of Misspellings and Grammatical Errors]](https://arxiv.org/abs/1911.12893)| [[download]](https://github.com/mhagiwara/github-typo-corpus)|
|W&I+LOCNESS on BEA2019 Shared Task| 2019|[[Developing an Automated Writing Placement System for ESL Learners ]](https://www.cl.cam.ac.uk/~hy260/WI-cefr.pdf)| [[direct download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/wi+locness_v2.1.bea19.tar.gz)
|FCE|2011| [[A New Dataset and Method for Automatically Grading ESOL Texts]](https://www.aclweb.org/anthology/P11-1019)| [[direct download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/fce_v2.1.bea19.tar.gz)|
|NUCLE|2013| [[Building a Large Annotated Corpus of Learner English: The NUS Corpus of Learner English]](https://www.aclweb.org/anthology/W13-1703)| [[download]](https://www.comp.nus.edu.sg/~nlp/corpora.html)|
|ICNALE|2013| [[The ICNALE and Sophisticated Contrastive Interlanguage Analysis of Asian Learners of English]](http://www.lib.kobe-u.ac.jp/infolib/meta_pub/G0000003kernel_81006678)| [[download]](http://language.sakura.ne.jp/icnale/)|
|Lang-8|2011| [[Mining Revision Log of Language Learning SNS for Automated Japanese Error Correction of Second Language Learners]](https://aclanthology.org/I11-1017)| [[website]](https://sites.google.com/site/naistlang8corpora/) [[download: Fill this form]](https://docs.google.com/forms/d/17gZZsC_rnaACMXmPiab3kjqBEtRHPMz0UG9Dk-x_F0k/viewform?edit_requested=true)<br>Related tools are useful. See the [[Other Tools]](https://github.com/gotutiyan/GEC-Info#other-tools) for the details.|

### For Training (Pseudo/Systhetic Data)

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|PIE-synthetic|2019| [[Parallel Iterative Edit Models for Local Sequence Transduction]](https://aclanthology.org/D19-1435)| [[download]](https://drive.google.com/open?id=1bl5reJ-XhPEfEaPjvO45M7w0yN-0XGOA)|
|OmniGEC|2025|[Introducing OmniGEC: A Silver Multilingual Dataset for Grammatical Error Correction](https://aclanthology.org/2025.unlp-1.17/)|[[HF datasets]](https://huggingface.co/collections/lang-uk/omnigec-68095391ebef195ed6c0a5f3), [[code]](https://github.com/r-kovalch/omnigec-data). Czech, English, Estonian, German, Greek, Icelandic, Italian, Latvian, Slovene, Swedish, and Ukrainian|

### For Evaluation

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|KJ|2011| [[Creating a manually error-tagged and shallow-parsed learner corpus]](https://aclanthology.org/P11-1121/)| [[download]](https://www.gsk.or.jp/catalog/gsk2019-a/)|
|CoNLL-2013|2013| [[The CoNLL-2013 Shared Task on Grammatical Error Correction]](https://aclanthology.org/W13-3601/)| [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll13st/release2.3.1.tar.gz)|
|CoNLL-2014|2014| [[The CoNLL-2014 Shared Task on Grammatical Error Correction]](https://aclanthology.org/W14-1701/)| [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll14st/conll14st-test-data.tar.gz)|
|10 additional annotations for the CoNLL14 |2015| [[How Far are We from Fully Automatic High Quality Grammatical Error Correction?]](https://aclanthology.org/P15-1068/)| [[direct download]](https://aclanthology.org/attachments/P15-1068.Datasets.zip)|
|8 additional annotations for the CoNLL14|2016| [[Reassessing the Goals of Grammatical Error Correction: Fluency Instead of Grammaticality]](https://aclanthology.org/Q16-1013)| [[download]](https://github.com/keisks/reassess-gec)|
|JFLEG|2017| [[JFLEG: A Fluency Corpus and Benchmark for Grammatical Error Correction]](https://aclanthology.org/E17-2037/)| [[download]](https://github.com/keisks/jfleg)|
|GMEG-Data|2019| [[Enabling Robust Grammatical Error Correction in New Domains: Data Sets, Metrics, and Analyses]](https://aclanthology.org/Q19-1032)| [[code]](https://github.com/grammarly/GMEG)|
|CWEB|2020| [[Grammatical Error Correction in Low Error Density Domains: A New Benchmark and Analyses]](https://www.aclweb.org/anthology/2020.emnlp-main.680)| [[download]](https://github.com/SimonHFL/CWEB)|
|ErAConD|2021|[[ErAConD : Error Annotated Conversational Dialog Dataset for Grammatical Error Correction]](https://aclanthology.org/2022.naacl-main.5/)|[[data]](https://github.com/yuanxun-yx/eracond)<br>Training dataset is also included.|
|RobustGEC|2023|[RobustGEC: Robust Grammatical Error Correction Against Subtle Context Perturbation](https://aclanthology.org/2023.emnlp-main.1043/)|[[code]](https://github.com/hillzhang1999/RobustGEC)|
|CSW Lang-8 Dataset|2024|[Grammatical Error Correction for Code-Switched Sentences by Learners of English](https://aclanthology.org/2024.lrec-main.698/)|[[code/data]](https://github.com/kelvinchanwh/csw-gector?tab=readme-ov-file)|
|CTSEG|2025|[Targeted Syntactic Evaluation for Grammatical Error Correction](https://aclanthology.org/2025.acl-long.1026/)|[[data]](https://github.com/SDS-NLP/CTSEG)|


# Performance measures

### Reference-based

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|M^2 Scorer|2012| [[Better Evaluation for Grammatical Error Correction]](https://aclanthology.org/N12-1067/)| [[code]](https://github.com/nusnlp/m2scorer)<br>It is often used to evaluate CoNLL-2013 and CoNLL-2014.|
|GLEU|2015| [[Ground Truth for Grammatical Error Correction Metrics]](https://aclanthology.org/P15-2097)<br>[[GLEU Without Tuning]](https://arxiv.org/abs/1605.02592)| [[code]](https://github.com/cnap/gec-ranking)<br>It is often used to evaluate JFLEG.|
|I-measure|2015| [[Towards a standard evaluation method for grammatical error detection and correction]](https://aclanthology.org/N15-1060/)| [[code]](https://github.com/mfelice/imeasure)<br>Code is available only python 2.x.|
|ERRANT|2016| [[Automatic Extraction of Learner Errors in ESL Sentences Using Linguistically Enhanced Alignments]](https://www.aclweb.org/anthology/C16-1079)<br>[[Automatic Annotation and Evaluation of Error Types for Grammatical Error Correction]](https://www.aclweb.org/anthology/P17-1074)| [[code]](https://github.com/chrisjbryant/errant)<br>It is often used to evaluate BEA-2019.|
|GMEG-Metric|2019| [[Enabling Robust Grammatical Error Correction in New Domains: Data Sets, Metrics, and Analyses]](https://aclanthology.org/Q19-1032)| [[code]](https://github.com/grammarly/GMEG)<br>Ridge regression using existing metrics (e.g. ERRANT, GLEU) as features.|
|GoToScorer|2019| [[Taking the Correction Difficulty into Account in Grammatical Error Correction Evaluation]](https://www.aclweb.org/anthology/2020.coling-main.188)| [[code]](https://github.com/gotutiyan/GTS)<br>It can be evaluated systems considering error correction difficulty.|
|PT-M2|2022|[Revisiting Grammatical Error Correction Evaluation and Beyond](https://aclanthology.org/2022.emnlp-main.463/)|[[code]](https://github.com/pygongnlp/PT-M2)|
|CLEME|2023|[CLEME: Debiasing Multi-reference Evaluation for Grammatical Error Correction](https://aclanthology.org/2023.emnlp-main.378/)|[[code]](https://github.com/THUKElab/CLEME.git)|
|GREEN|2024|[n-gram F-score for Evaluating Grammatical Error Correction](https://aclanthology.org/2024.inlg-main.25/)|[[code]](https://github.com/shotakoyama/green)|
||2025|[Refined Evaluation for End-to-End Grammatical Error Correction Using an Alignment-Based Approach](https://aclanthology.org/2025.coling-main.52/)|[[website]](https://open-writing-evaluation.github.io/)|
|CLEME2.0|2025|[CLEME2.0: Towards Interpretable Evaluation by Disentangling Edits for Grammatical Error Correction](https://aclanthology.org/2025.acl-long.10/)|[[code]](https://github.com/THUKElab/CLEME.git)|
|ERRANT extended to multiple languages|2025|[Multilingual Grammatical Error Annotation: Combining Language-Agnostic Framework with Language-Specific Flexibility](https://aclanthology.org/2025.bea-1.15/)|[[code]](https://github.com/open-writing-evaluation/jp_errant_bea)|

### Reference-free

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Scoring by counting the errors|2016|[[There’s No Comparison: Reference-less Evaluation Metrics in Grammatical Error Correction]](https://aclanthology.org/D16-1228)|[[code]](https://github.com/cnap/grammaticality-metrics)|
|Fluency + grammaticality + meaning preservation| 2017| [[Reference-based Metrics can be Replaced with Reference-less Metrics in Evaluating Grammatical Error Correction Systems]](https://aclanthology.org/I17-2058)||
|USim| 2018| [[Reference-less Measure of Faithfulness for Grammatical Error Correction]](https://aclanthology.org/N18-2020/)| [[code]](https://github.com/borgr/USim)|
|SOME|2020| [[SOME: Reference-less Sub-Metrics Optimized for Manual Evaluations of Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.573)| [[code]](https://github.com/kokeman/SOME)|
|Scribendi Score|2021|[[Is this the end of the gold standard? A straightforward reference-less grammatical error correction metric]](https://aclanthology.org/2021.emnlp-main.239/)|[[Unofficial code]](https://github.com/gotutiyan/scribendi_score)|
|IMPARA|2022|[IMPARA: Impact-Based Metric for GEC Using Parallel Data](https://aclanthology.org/2022.coling-1.316/)|[[code]](https://github.com/Silviase/IMPARA)|
||2024|[Large Language Models Are State-of-the-Art Evaluator for Grammatical Error Correction](https://aclanthology.org/2024.bea-1.6)||
|IMPARA-GED|2025|[IMPARA-GED: Grammatical Error Detection is Boosting Reference-free Grammatical Error Quality Estimator](https://aclanthology.org/2025.findings-acl.1315/)|[[Official model]](https://huggingface.co/naist-nlp/IMPARA-GED)|
||2025|[LLM-based post-editing as reference-free GEC evaluation](https://aclanthology.org/2025.bea-1.16/)||

### Meta-evaluation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Re-rank the CoNLL14 systems by human evaluation|2015|[Human Evaluation of Grammatical Error Correction Systems](https://aclanthology.org/D15-1052/)|[[code]](https://github.com/grammatical/evaluation/)|
|Reassess M^2, I-measure, GLEU by comparing human evaluation|2018|[[A Reassessment of Reference-Based Grammatical Error Correction Metrics]](https://aclanthology.org/C18-1231) |[[code]](https://github.com/nusnlp/gecmetrics)|
|MAEGE|2018|[Automatic Metric Validation for Grammatical Error Correction](https://aclanthology.org/P18-1127)|[[code]](https://github.com/borgr/EoE)|
|SEEDA|2024|[Revisiting Meta-evaluation for Grammatical Error Correction](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00676/123651/Revisiting-Meta-evaluation-for-Grammatical-Error)|[[code]](https://github.com/tmu-nlp/SEEDA)|

# Quality Estimation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2022|[Proficiency Matters Quality Estimation in Grammatical Error Correction](https://arxiv.org/abs/2201.06199)||


# Models

### Before Neural (E.g., SMT)

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2006|[Correcting ESL Errors Using Phrasal SMT Techniques](https://aclanthology.org/P06-1032/)||
||2009|[Using First and Second Language Models to Correct Preposition Errors in Second Language Authoring](https://aclanthology.org/W09-2110/)||
||2010|[Generating Confusion Sets for Context-Sensitive Error Correction](https://aclanthology.org/D10-1094/)||
||2011|[Correcting Semantic Collocation Errors with L1-induced Paraphrases](https://aclanthology.org/D11-1010/)||
||2012|[Tense and Aspect Error Correction for ESL Learners Using Global Context](https://aclanthology.org/P12-2039/)||
||2012|[Exploring Grammatical Error Correction with Not-So-Crummy Machine Translation](https://aclanthology.org/W12-2005/)||
||2014|[Grammatical error correction using hybrid systems and type filtering](https://aclanthology.org/W14-1702/)|CoNLL2014: CAMB|
||2014|[The AMU System in the CoNLL-2014 Shared Task: Grammatical Error Correction by Data-Intensive and Feature-Rich Statistical Machine Translation](https://aclanthology.org/W14-1703/)|CoNLL2014: AMU|
||2014|[The Illinois-Columbia System in the CoNLL-2014 Shared Task](https://aclanthology.org/W14-1704/)|CoNLL2014: CUUI|
||2014|[RACAI GEC – A hybrid approach to Grammatical Error Correction](https://aclanthology.org/W14-1705)|CoNLL2014: RAC|
||2014|[Grammatical Error Detection Using Tagger Disagreement](https://aclanthology.org/W14-1706/)|CoNLL2014: UFC|
||2014|[CoNLL 2014 Shared Task: Grammatical Error Correction with a Syntactic N-gram Language Model from a Big Corpora](https://aclanthology.org/W14-1707/)|CoNLL2014: IPN|
||2014|[Tuning a Grammar Correction System for Increased Precision](https://aclanthology.org/W14-1708/)|CoNLL2014: IITB|
||2014|[POSTECH Grammatical Error Correction System in the CoNLL-2014 Shared Task](https://aclanthology.org/W14-1709/)|CoNLL2014: POST|
||2014|[Grammatical Error Detection and Correction using a Single Maximum Entropy Model](https://aclanthology.org/W14-1710/)|CoNLL2014: SJTU|
||2014|[Factored Statistical Machine Translation for Grammatical Error Correction](https://aclanthology.org/W14-1711/)|CoNLL2014: UMC|
||2014|[NTHU at the CoNLL-2014 Shared Task](https://aclanthology.org/W14-1712/)|CoNLL2014: NTHU|
||2014|[A Unified Framework for Grammar Error Correction](https://aclanthology.org/W14-1713/)|CoNLL2014: PKU|
||2016|[Exploiting N-Best Hypotheses to Improve an SMT Approach to Grammatical Error Correction](https://arxiv.org/abs/1606.00210)||
||2016|[Adapting Grammatical Error Correction Based on the Native Language of Writers with Neural Network Joint Models](https://aclanthology.org/D16-1195/)
|Phrase-based SMT| 2016| [[Phrase-based Machine Translation is State-of-the-Art for Automatic Grammatical Error Correction]](https://aclanthology.org/D16-1161/)| [[code]](https://github.com/grammatical/baselines-emnlp2016)|
|Word-level SMT enhanced NNJMs + char-based SMT|2017|[[Connecting the Dots: Towards Human-Level Grammatical Error Correction]](https://aclanthology.org/W17-5037)|[[code]](https://github.com/nusnlp/smtgec2017)|
|SMEG|2017|[[Systematically Adapting Machine Translation for Grammatical Error Correction]](https://aclanthology.org/W17-5039)|[[code]](https://github.com/cnap/smt-for-gec)|

### Encoder-Decoder
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|First NMT-based approach|2016|[[Grammatical error correction using neural machine translation]](https://aclanthology.org/N16-1042/)||
||2016|[Neural Network Translation Models for Grammatical Error Correction](https://arxiv.org/abs/1606.00189)||
|Neural reinforcement learning|2017|[[Grammatical Error Correction with Neural Reinforcement Learning]](https://aclanthology.org/I17-2062/)|[[code]](https://github.com/keisks/nematus/tree/nrl-gleu)|
|A nested attention (word and char attention)|2017|[[A Nested Attention Neural Hybrid Model for Grammatical Error Correction]](https://aclanthology.org/P17-1070)||
|Re-ranking N-best sentence (by SMT) with LSTM-based GED|2017|[[Neural Sequence-Labelling Models for Grammatical Error Correction]](https://aclanthology.org/D17-1297/)||
|Hybrid SMT and NMT|2018|[[Near Human-Level Performance in Grammatical Error Correction with Hybrid Machine Translation]](https://aclanthology.org/N18-2046)||
|CNN-based Encder-Decoder approach| 2018|[[A Multilayer Convolutional Encoder-Decoder Neural Network for Grammatical Error Correction]](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/17308/16137)|[[code]](https://github.com/nusnlp/mlconvgec2018)|
|Fluency boosting learning|2018|[[Fluency Boost Learning and Inference for Neural Grammatical Error Correction]](https://aclanthology.org/P18-1097)|[[code]](https://github.com/getao/human-performance-gec) [[arXiv]](https://arxiv.org/abs/1807.01270)|
|Copy-Augmented Architecture|2019|[[Improving Grammatical Error Correction via Pre-Training a Copy-Augmented Architecture with Unlabeled Data]](https://aclanthology.org/N19-1014)|[[code]](https://github.com/yuantiku/fairseq-gec)|
|Consider a few previous sentences|2019|[[Cross-Sentence Grammatical Error Correction]](https://aclanthology.org/P19-1042)|[[code]](https://github.com/nusnlp/crosentgec)|
|Use sentence-level error dectection| 2019|[[The AIP-Tohoku System at the BEA-2019 Shared Task]](https://aclanthology.org/W19-4418)|BEA-2019: AIP-Tohoku||
|Four CNN + eight Transformer|2019|[[The LAIX Systems in the BEA-2019 GEC Shared Task]](https://aclanthology.org/W19-4416)|BEA-2019: LAIX|
|Combine Transformer+CNN with FST + Re-ranking|2019|[[Neural and FST-based approaches to grammatical error correction]](https://aclanthology.org/W19-4424)|BEA-2019: CAMB-CLED|
|Transformer seq2seq + BERT re-ranker|2019|[[TMU Transformer System Using BERT for Re-ranking at BEA 2019 Grammatical Error Correction on Restricted Track]](https://aclanthology.org/W19-4422)|BEA-2019: TMU|
|Apply noisy channel with BERT and GPT-2 as LM|2019|[[Noisy Channel for Low Resource Grammatical Error Correction]](https://aclanthology.org/W19-4420.pdf)|BEA-2019: Siteimprove|
|Use Finite State Transducers|2019|[[Neural Grammatical Error Correction with Finite State Transducers]](https://aclanthology.org/N19-1406)||
|BERT-fuse|2020|[[Encoder-Decoder Models Can Benefit from Pre-trained Masked Language Models in Grammatical Error Correction]](https://aclanthology.org/2020.acl-main.391/)|[[code]](https://github.com/kanekomasahiro/bert-gec)|
|Adversarial approach (G:seq2seq D:sentence-pair classification)|2020|[[Adversarial Grammatical Error Correction]](https://aclanthology.org/2020.findings-emnlp.275)||
|Erroneous span correction and detection|2020|[[Improving the Efficiency of Grammatical Error Correction with Erroneous Span Detection and Correction]](https://aclanthology.org/2020.emnlp-main.581/)||
|Document-level approach|2020|[[Document-level grammatical error correction]](https://aclanthology.org/2021.bea-1.8/)|[[code]](https://github.com/chrisjbryant/doc-gec)|
|Beam search considering copy probability|2020|[[Generating Diverse Corrections with Local Beam Search for Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.193)||
|BART-based|2020|[[Stronger Baselines for Grammatical Error Correction Using a Pretrained Encoder-Decoder Model]](https://aclanthology.org/2020.aacl-main.83)|[[code]](https://github.com/Katsumata420/generic-pretrained-GEC)|
|VERNet|2021|[[Neural Quality Estimation with Multiple Hypotheses for Grammatical Error Correction]](https://aclanthology.org/2021.naacl-main.429)|[[code]](https://github.com/thunlp/VERNet)|
|Shallow Aggressive Decoding|2021|[[Instantaneous Grammatical Error Correction with Shallow Aggressive Decoding]](https://aclanthology.org/2021.acl-long.462/)|[[code]](https://github.com/AutoTemp/Shallow-Aggressive-Decoding)|
|T5-based|2021|[[A Simple Recipe for Multilingual Grammatical Error Correction]](https://arxiv.org/abs/2106.03830)|[[code]](https://github.com/google-research-datasets/clang8)|
|Use multiclass GED for Transformer seq2seq and reranking|2021|[[Multi-Class Grammatical Error Detection for Correction: A Tale of Two Systems]](https://aclanthology.org/2021.emnlp-main.687/)||
|GEC for writing improvement model adapted to the writer’s L1|2021|[[Beyond Grammatical Error Correction: Improving L1-influenced research writing in English using pre-trained encoder-decoder models]](https://aclanthology.org/2021.findings-emnlp.216/)|[[code]](https://github.com/gzomer/BeyondGEC)|
|Constrastive Leaning approach|2021|[[Grammatical Error Correction with Contrastive Learning in Low Error Density Domains]](https://aclanthology.org/2021.findings-emnlp.419/)|[[code]](https://github.com/nusnlp/geccl)|
|Sequence Span Rewriting|2021|[[Improving Sequence-to-Sequence Pre-training via Sequence Span Rewriting]](https://aclanthology.org/2021.emnlp-main.45/)||
|Pretrain by DAE + sequential transfer learning|2019|[[A Neural Grammatical Error Correction System Built On Better Pre-training and Sequential Transfer Learning]](https://aclanthology.org/W19-4423/)|[[code]](https://github.com/kakaobrain/helo_word)<br>BEA-2019: Kakao&Brain|
|Dependent Self-Attention (DSA)|2021|[[Grammatical Error Correction with Dependency Distance]](https://dl.acm.org/doi/abs/10.1145/3459637.3482348)||
|A GEC model using only 11.6MB|2021|[An efficient system for grammatical error correction on mobile devices](https://ieeexplore.ieee.org/document/9364435)||
|LM-Critic| 2021|[LM-Critic: Language Models for Unsupervised Grammatical Error Correction](https://aclanthology.org/2021.emnlp-main.611/)| [[code]](https://github.com/michiyasunaga/LM-Critic)<br>Supervised setting is also performed|
||2022|[Interpretability for Language Learners Using Example-Based Grammatical Error Correction](https://aclanthology.org/2022.acl-long.496/)|[[code]](https://github.com/kanekomasahiro/eb-gec)|
||2022|[Position Offset Label Prediction for Grammatical Error Correction](https://aclanthology.org/2022.coling-1.480/)||
|SynGEC|2022|[SynGEC: Syntax-Enhanced Grammatical Error Correction with a Tailored GEC-Oriented Parser](https://aclanthology.org/2022.emnlp-main.162/)|[[code]](https://github.com/HillZhang1999/SynGEC)|
|EdiT5|2022|[EdiT5: Semi-Autoregressive Text Editing with T5 Warm-Start](https://aclanthology.org/2022.findings-emnlp.156/)|[[code]](https://emalmi.kapsi.fi/edit5_code.html)|
|GEC-DePenD|2023|[GEC-DePenD: Non-Autoregressive Grammatical Error Correction with Decoupled Permutation and Decoding](https://aclanthology.org/2023.acl-long.86)|[[code]](https://github.com/Gibson210/GEC-DePenD)|
|TemplateGEC|2023|[TemplateGEC: Improving Grammatical Error Correction with Detection Template](https://aclanthology.org/2023.acl-long.380)|[[code]](https://github.com/li-aolong/TemplateGEC)|
|LET|2023|[LET: Leveraging Error Type Information for Grammatical Error Correction](https://aclanthology.org/2023.findings-acl.371)||
||2023|[Leveraging Denoised Abstract Meaning Representation for Grammatical Error Correction](https://aclanthology.org/2023.findings-acl.449)||
|Use speech information|2023|[Improving Grammatical Error Correction with Multimodal Feature Integration](https://aclanthology.org/2023.findings-acl.594)|[[code]](https://github.com/NLP2CT/MultimodalGEC)|
||2023|[Improving Autoregressive Grammatical Error Correction with Non-autoregressive Models](https://aclanthology.org/2023.findings-acl.760)||
||2023|[Unsupervised Grammatical Error Correction Rivaling Supervised Methods](https://aclanthology.org/2023.emnlp-main.185/)|[[code]](https://github.com/nusnlp/ugec)|
||2024|[No Error Left Behind: Multilingual Grammatical Error Correction with Pre-trained Translation Models](https://aclanthology.org/2024.eacl-long.73/)||
|EDU Copy Mechanism|2024|[Improving Copy-oriented Text Generation via EDU Copy Mechanism](https://aclanthology.org/2024.lrec-main.768/)||
||2024|[Efficient and Interpretable Grammatical Error Correction with Mixture of Experts](https://aclanthology.org/2024.findings-emnlp.997/)|[[code]](https://github.com/nusnlp/moece)|
||2025|[InstructGEC: Enhancing Unsupervised Grammatical Error Correction with Instruction Tuning](https://aclanthology.org/2025.coling-main.9/)||
|CxGGEC|2025|[CxGGEC: Construction-Guided Grammatical Error Correction](https://aclanthology.org/2025.acl-long.307/)||

### Tagging / Non-autogressive
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|LSTM tagger for word coice task|2019|[[Choosing the Right Word: Using Bidirectional LSTM Tagger for Writing Support Systems]](https://arxiv.org/abs/1901.02490)|[[code]](https://github.com/vicmak/Exploiting-BiLSTM-for-Proper-Word-Choice)|
|PIE|2019|[[Parallel Iterative Edit Models for Local Sequence Transduction]](https://aclanthology.org/D19-1435/)|[[code]](https://github.com/awasthiabhijeet/PIE)|
|LaserTagger|2019|[[Encode, Tag, Realize: High-Precision Text Editing]](https://aclanthology.org/D19-1510/)|[[code]](https://github.com/google-research/lasertagger)|
|GECToR|2020|[[GECToR – Grammatical Error Correction: Tag, Not Rewrite]](https://aclanthology.org/2020.bea-1.16/)|[[code]](https://github.com/grammarly/gector)|
|Seq2Edits|2020|[[Seq2Edits: Sequence Transduction Using Span-level Edit Operations]](https://aclanthology.org/2020.emnlp-main.418/)|[[code]](https://github.com/tensorflow/tensor2tensor/blob/master/tensor2tensor/models/research/transformer_seq2edits.py)|
|GAN-like sequence labeling|2021|[[Grammatical Error Correction as GAN-like Sequence Labeling]](https://aclanthology.org/2021.findings-acl.290/)||
|GECToR Large|2022|[Ensembling and Knowledge Distilling of Large Sequence Taggers for Grammatical Error Correction](https://aclanthology.org/2022.acl-long.266/)|[[code]](https://github.com/makstarnavskyi/gector-large) [[Author's Master Thesis]](https://drive.google.com/file/d/17-qXILfafHR8Uv2Y9plcB9WVRdZLazzp/view)|
||2021|[Efficient Grammatical Error Correction with Hierarchical Error Detections and Correction](https://ieeexplore.ieee.org/document/9590395)|[[code]](https://github.com/AnticPan/Hierarchical-GEC)|
||2022|[Type-Driven Multi-Turn Corrections for Grammatical Error Correction](https://aclanthology.org/2022.findings-acl.254/)|[[code]](https://github.com/deeplearnxmu/tmtc)|
||2023|[An Extended Sequence Tagging Vocabulary for Grammatical Error Correction](https://aclanthology.org/2023.findings-eacl.119)|[[code]](https://github.com/StuartMesham/gector_experiment_public/tree/master)|

### Large Language Model
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|5-gram LM based approach| 2018|[Language Model Based Grammatical Error Correction without Annotated Training Data](https://aclanthology.org/W18-0529/)| [[code]](https://github.com/chrisjbryant/lmgec-lite)|
|Use Finite State Transducers|2019|[Neural Grammatical Error Correction with Finite State Transducers](https://aclanthology.org/N19-1406)||
|Use LM (BERT, GPT-1,2)|2019|[[The Unreasonable Effectiveness of Transformer Language Models in Grammatical Error Correction]](https://aclanthology.org/W19-4412/)||
||2023|[Reducing Sequence Length by Predicting Edit Spans with Large Language Models](https://aclanthology.org/2023.emnlp-main.619/)||
||2023|[Exploring Effectiveness of GPT-3 in Grammatical Error Correction: A Study on Performance and Controllability in Prompt-Based Methods](https://aclanthology.org/2023.bea-1.18)||
||2024|[Evaluating Prompting Strategies for Grammatical Error Correction Based on Language Proficiency](https://aclanthology.org/2024.lrec-main.569/)||
||2024|[GPT-3.5 for Grammatical Error Correction](https://aclanthology.org/2024.lrec-main.692/)|Target languages: CZ, DE, EN, RU, SV, UA|
||2024|[Ungrammatical-syntax-based In-context Example Selection for Grammatical Error Correction](https://aclanthology.org/2024.naacl-long.99)|[[code]](https://github.com/JamyDon/SynICL4GEC)|
|mEdIT|2024|[mEdIT: Multilingual Text Editing via Instruction Tuning](https://aclanthology.org/2024.naacl-long.56)|[[code]](https://github.com/vipulraheja/medit)|
|DeCoGLM|2024|[Detection-Correction Structure via General Language Model for Grammatical Error Correction](https://aclanthology.org/2024.acl-long.96)|[[code]](https://github.com/GMago-LeWay/GECFramework)|
|For code-switched text|2024|[LLM-based Code-Switched Text Generation for Grammatical Error Correction](https://aclanthology.org/2024.emnlp-main.942/)|[[code]](https://github.com/tpotterer/Synthetic-CSW-Text-for-GEC)|
|EPO|2025|[Edit-Wise Preference Optimization for Grammatical Error Correction](https://aclanthology.org/2025.coling-main.229/)||
||2024|[Prompting open-source and commercial language models for grammatical error correction of English learner text](https://aclanthology.org/2024.findings-acl.711)|[[code]](https://github.com/chrisdavis90/gec-prompting-public)|
||2025|[Explanation based In-Context Demonstrations Retrieval for Multilingual Grammatical Error Correction](https://aclanthology.org/2025.naacl-long.251/)|[[code]](https://github.com/GMago-LeWay/FewShotGEC)|
||2025|[Encode Errors: Representational Retrieval of In-Context Demonstrations for Multilingual Grammatical Error Correction](https://aclanthology.org/2025.findings-acl.1090/)|[[code]](https://github.com/viniferagy/GER)|
||2025|[Adapting LLMs for Minimal-edit Grammatical Error Correction](https://aclanthology.org/2025.bea-1.9/)|[[code]](https://github.com/richardxoldman/llms-for-minimal-gec)|
||2025|[Leveraging What’s Overfixed: Post-Correction via LLM Grammatical Error Overcorrection](https://aclanthology.org/2025.emnlp-main.1431/)||

# Ensembles / Post-processing

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Use MENT|2014|[System Combination for Grammatical Error Correction](https://aclanthology.org/D14-1102/)||
||2016|[Grammatical Error Correction: Machine Translation and Classifiers](https://aclanthology.org/P16-1208)||
||2019|[[Learning to combine Grammatical Error Corrections]](https://aclanthology.org/W19-4414/)|[[code]](https://github.com/IBM/learning-to-combine-grammatical-error-corrections)|
|Diversity-Driven Combination (DDC)|2021|[[Diversity-Driven Combination for Grammatical Error Correction]](https://arxiv.org/abs/2110.15149)|[[code]](https://github.com/nusnlp/gec-ddc)|
|Select a system for each error type with IP|2021|[[System Combination for Grammatical Error Correction Based on Integer Programming]](https://aclanthology.org/2021.ranlp-1.94/)|[[code]](https://github.com/nusnlp/gec_ip)|
||2022|[Frustratingly Easy System Combination for Grammatical Error Correction](https://aclanthology.org/2022.naacl-main.143/)|[[code]](https://github.com/nusnlp/esc)|
|EditScorer|2022|[Improved grammatical error correction by ranking elementary edits](https://aclanthology.org/2022.emnlp-main.785/)|[[code]](https://github.com/AlexeySorokin/EditScorer)|
|GRECO|2023|[System Combination via Quality Estimation for Grammatical Error Correction](https://aclanthology.org/2023.emnlp-main.785/)|[[code]](https://github.com/nusnlp/greco)|
||2024|[Improving Grammatical Error Correction by Correction Acceptability Discrimination](https://aclanthology.org/2024.lrec-main.772/)||


# Strategies

This includes methods such as decoding techniques and approaches that modify the loss function while keeping the model architecture unchanged.

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2012|[A Beam-Search Decoder for Grammatical Error Correction](https://aclanthology.org/D12-1052/)||
||2016|[Discriminative Reranking for Grammatical Error Correction with Statistical Machine Translation](https://aclanthology.org/N16-1133/)||
||2016|[Candidate re-ranking for SMT-based grammatical error correction](https://aclanthology.org/W16-0530/)||
|Some methods that can be adapted neural MT|2018|[[Approaching Neural Grammatical Error Correction as a Low-Resource Machine Translation Task]](https://aclanthology.org/N18-1055/)|[[code]](https://github.com/grammatical/neural-naacl2018)|
|Iterative decoding|2018|[[Weakly Supervised Grammatical Error Correction using Iterative Decoding]](https://arxiv.org/abs/1811.01710)||
||2019|[Controlling Grammatical Error Correction Using Word Edit Rate](https://aclanthology.org/P19-2020/)||
|Add adversarial examples continually|2020|[[Improving Grammatical Error Correction Models with Purpose-Built Adversarial Examples]](https://aclanthology.org/2020.emnlp-main.228)||
|Cross-lingual Transfer Learning|2020|[[Cross-lingual Transfer Learning for Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.415)||
|Data Weighted Training Strategies|2020|[[Data Weighted Training Strategies for Grammatical Error Correction]](https://aclanthology.org/2020.tacl-1.41/)||
|Align-and-Predict Decoding|2022|[Adjusting the Precision-Recall Trade-Off with Align-and-Predict Decoding for Grammatical Error Correction](https://aclanthology.org/2022.acl-short.77/)|[[code]](https://github.com/AutoTemp/Align-and-Predict.git)|
||2023|[Mitigating Exposure Bias in Grammatical Error Correction with Data Augmentation and Reweighting](https://aclanthology.org/2023.eacl-main.155)|[[code]](https://github.com/nusnlp/gec_eb)|
|BTR|2023|[Bidirectional Transformer Reranker for Grammatical Error Correction](https://aclanthology.org/2023.findings-acl.234)|[[code]](https://github.com/zhangying9128/BTR)|
||2023|[Efficient Grammatical Error Correction Via Multi-Task Training and Optimized Training Schedule](https://aclanthology.org/2023.emnlp-main.355/)||
|MainGEC|2023|[Grammatical Error Correction via Mixed-Grained Weighted Training](https://aclanthology.org/2023.findings-emnlp.400/)||
||2023|[Improving Seq2Seq Grammatical Error Correction via Decoding Interventions](https://aclanthology.org/2023.findings-emnlp.495)|[[code]](https://github.com/Jacob-Zhou/gecdi)|
||2024|[Multi-pass Decoding for Grammatical Error Correction](https://aclanthology.org/2024.emnlp-main.553/)||


# Data Augmentation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Make artificial errors in a probabilistic manner|2014|[[Generating artificial errors for grammatical error correction]](https://aclanthology.org/E14-3013/)||
|Back translation|2016|[[Improving Neural Machine Translation Models with Monolingual Data]](https://aclanthology.org/P16-1009/)||
|SMT based MT + pattern extraction|2017|[[Artificial Error Generation with Machine Translation and Syntactic Patterns]](https://aclanthology.org/W17-5032)||
|Diverse back translation with noisy beam search|2018|[[Noising and Denoising Natural Language: Diverse Backtranslation for Grammar Correction]](https://aclanthology.org/N18-1057/)||
|MAGEC|2019|[[Minimally-Augmented Grammatical Error Correction]](https://aclanthology.org/D19-5546)|Supervised setting is also performed|
|DirectNoise| 2019|[[Improving Grammatical Error Correction via Pre-Training a Copy-Augmented Architecture with Unlabeled Data]](https://aclanthology.org/N19-1014/)|The method was first called "DirectNoise" by [[kiyono+ 2019]](https://aclanthology.org/D19-1119/)?|
|Substituting words using confusion sets|2019|[[Neural Grammatical Error Correction Systems with Unsupervised Pre-training on Synthetic Data]](https://aclanthology.org/W19-4427)|[[synthetic data]](https://github.com/grammatical/pretraining-bea2019/issues/6)<br>BEA-2019: UEDIN-MS|
|Error+Context Dictionary|2019|[[Improving Precision of Grammatical Error Correction with a Cheat Sheet]](https://aclanthology.org/W19-4425)|BEA-2019: 	Buffalo|
|Use Google Translate for making pseudo data|2019|[[(Almost) Unsupervised Grammatical Error Correction using a Synthetic Comparable Corpus]](https://aclanthology.org/W19-4413)|BEA-2019: TMU in Low Resource|
|Inverted Spellchecker + Patterns+POS|2019|[[A Comparative Study of Synthetic Data Generation Methods for Grammatical Error Correction]](https://aclanthology.org/2020.bea-1.21)||
|Methods for erroneous data generation|2019|[[Erroneous data generation for Grammatical Error Correction]](https://aclanthology.org/W19-4415)|BEA-2019: Shuyao|
|Wikipedia revision & Wikipedia round-trip translation|2019|[[Corpora Generation for Grammatical Error Correction]](https://aclanthology.org/N19-1333)||
|Create confusion sets by edit distance, word embeddings, spell-breaking|2019|[[Minimally-Augmented Grammatical Error Correction]](https://aclanthology.org/D19-5546)|Supervised setting is also performed|
|Explore methods to make pseude data, seed corpus, training settings|2019|[[An Empirical Study of Incorporating Pseudo Data into Grammatical Error Correction]](https://aclanthology.org/D19-1119/)|[[code]](https://github.com/butsugiri/gec-pseudodata)|
||2020|[[Massive Exploration of Pseudo Data for Grammatical Error Correction]](https://ieeexplore.ieee.org/document/9134890)||
|Control error rates and error types by rule-based corruption and filtered back-translation|2020|[[Controllable Data Synthesis Method for Grammatical Error Correction]](https://arxiv.org/pdf/1909.13302.pdf)||
|Use machine translation pairs|2020|[[Improving Grammatical Error Correction with Machine Translation Pairs]](https://aclanthology.org/2020.findings-emnlp.30/)||
|Edit latent representation|2020|[[Improving Grammatical Error Correction with Data Augmentation by Editing Latent Representation]](https://aclanthology.org/2020.coling-main.200/)||
|Consider learner’s error tendency|2020|[[Grammatical Error Correction Using Pseudo Learner Corpus Considering Learner’s Error Tendency]](https://aclanthology.org/2020.acl-srw.5/)||
|Tagged corruption|2021|[[Synthetic Data Generation for Grammatical Error Correction with Tagged Corruption Models]](https://aclanthology.org/2021.bea-1.4/)|[[code]](https://github.com/google-research-datasets/C4_200M-synthetic-dataset-for-grammatical-error-correction)|
|Use 188 modules|2021|[[Various Errors Improve Neural Grammatical Error Correction]](https://aclanthology.org/2021.paclic-1.27/)|[[code]](https://github.com/shotakoyama/arteraro)|
|Use real error petterns and linguistic knowledge|2021|[[Data Augmentation of Incorporating Real Error Patterns and Linguistic Knowledge for Grammatical Error Correction]](https://aclanthology.org/2021.conll-1.17/)||
|Divide non-English sentence into chunks → translate to English for each of them → concatenate|2021|[[Grammatical Error Generation Based on Translated Fragments]](https://aclanthology.org/2021.nodalida-main.44/)||
||2023|[Grammatical Error Correction through Round-Trip Machine Translation](https://aclanthology.org/2023.findings-eacl.165)||
|TransGEC|2023|[TransGEC: Improving Grammatical Error Correction with Translationese](https://aclanthology.org/2023.findings-acl.223)|[[code]](https://github.com/NLP2CT/TransGEC)|
|Focus on gender bias|2023|[Gender-Inclusive Grammatical Error Correction through Augmentation](https://aclanthology.org/2023.bea-1.13)|[[code]](https://github.com/grammarly/gender-inclusive-gec)|
||2023|[Training for Grammatical Error Correction Without Human-Annotated L2 Learners’ Corpora](https://aclanthology.org/2023.bea-1.38)||
|MixEdit|2023|[MixEdit: Revisiting Data Augmentation and Beyond for Grammatical Error Correction](https://aclanthology.org/2023.findings-emnlp.681/)|[[code]](https://github.com/THUKElab/MixEdit)|
||2024|[Synthetic Data Generation for Low-resource Grammatical Error Correction with Tagged Corruption Models](https://aclanthology.org/2024.bea-1.2)||
||2024|[Improving Grammatical Error Correction via Contextual Data Augmentation](https://aclanthology.org/2024.findings-acl.647)|[[code]](https://github.com/wyxstriker/CDA4GEC)|
||2024|[To Err Is Human, but Llamas Can Learn It Too](https://aclanthology.org/2024.findings-emnlp.727/)|[[code]](https://github.com/TartuNLP/gec-llm)|
||2025|[Large Language Models are Good Annotators for Type-aware Data Augmentation in Grammatical Error Correction](https://aclanthology.org/2025.coling-main.14/)|[[code]](https://github.com/LiXinyuan1015/TypeDA)|
||2025|[Leveraging Multilingual Models for Robust Grammatical Error Correction Across Low-Resource Languages](https://aclanthology.org/2025.coling-industry.43/)||
||2025|[Low-Resource Grammatical Error Correction: Selective Data Augmentation with Round-Trip Machine Translation](https://aclanthology.org/2025.findings-acl.1322/)|[[code]](https://github.com/arozovskaya/Low-Resource-GEC-SeLex-RT). experiments Include Russian and Ukrainian.|

### Data Cleaning

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|A Self-Refinement Strategy for Noise Reduction|2020|[[A Self-Refinement Strategy for Noise Reduction in Grammatical Error Correction]](https://aclanthology.org/2020.findings-emnlp.26/)||
|cLang8 (Cleaned Lang-8)|2021| [[A Simple Recipe for Multilingual Grammatical Error Correction]](https://aclanthology.org/2021.acl-short.89/)| [[code]](https://github.com/google-research-datasets/clang8)|

# Analyses

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2011|[Algorithm Selection and Model Adaptation for ESL Correction Tasks](https://aclanthology.org/P11-1093.pdf)||
||2012|[The Effect of Learner Corpus Size in Grammatical Error Correction of ESL Writings](https://aclanthology.org/C12-2084/)||
||2015| [[How Far are We from Fully Automatic High Quality Grammatical Error Correction?]](https://aclanthology.org/P15-1068)||
|Human annotation focused on fluency |2016| [[Reassessing the Goals of Grammatical Error Correction: Fluency Instead of Grammaticality]](https://aclanthology.org/Q16-1013)|[[code]](https://github.com/keisks/reassess-gec)|
||2017| [[GEC into the future: Where are we going and how do we get there?]](https://aclanthology.org/W17-5019/)||
||2018| [[Inherent Biases in Reference-based Evaluation for Grammatical Error Correction]](https://aclanthology.org/P18-1059/)| [[code]](https://github.com/borgr/IBGEC)|
||2018|[[Assessing Grammatical Correctness in Language Learning]](https://aclanthology.org/2021.bea-1.15/)||
|Quality estimation (and re-ranking using estimated score)|2018|[[Neural Quality Estimation of Grammatical Error Correction]](https://aclanthology.org/D18-1274/)|[[code]](https://github.com/nusnlp/neuqe)|
|Evaluate four systems (SMT, CNN, LSTM, Transformer) for six corpora (CoNLL13&14, FCE, JFLEG, KJ, ICNALE)|2019| [[Cross-Corpora Evaluation and Analysis of Grammatical Error Correction Models — Is Single-Corpus Evaluation Enough?]](https://aclanthology.org/N19-1132/) ||
|Compare CNN, Transformer, PRPN, ON-LSTM as back-translation models|2019|[[The Unbearable Weight of Generating Artificial Errors for Grammatical Error Correction]](https://aclanthology.org/W19-4449)||
|GEC for post-processing|2019|[Automatic Grammatical Error Correction for Sequence-to-sequence Text Generation: An Empirical Study](https://aclanthology.org/P19-1609/)||
|CGOP|2020|[[Comparison of the Evaluation Metrics for Neural Grammatical Error Correction With Overcorrection]](https://ieeexplore.ieee.org/document/9102992)|Metric Considering overcorrection|
|Create new gold data by post-editing system outputs|2021| [[How Good (really) are Grammatical Error Correction Systems?]](https://aclanthology.org/2021.eacl-main.231/)||
|Explore whether models have grammatical knowledge with Known-setting and Unknown-setting|2021| [[Do Grammatical Error Correction Models Realize Grammatical Generalization?]](https://aclanthology.org/2021.findings-acl.399/)||
|Compare CNN, LSTM, transformer or combinations of them as BT models|2021| [[Comparison of Grammatical Error Correction Using Back-Translation Models]](https://aclanthology.org/2021.naacl-srw.16/)||
||2022|[Uncertainty Determines the Adequacy of the Mode and the Tractability of Decoding in Sequence-to-Sequence Models](https://aclanthology.org/2022.acl-long.591/)||
||2022|[Grammatical Error Correction: Are We There Yet?](https://aclanthology.org/2022.coling-1.246/)||
||2022|[Grammatical Error Correction Systems for Automated Assessment: Are They Susceptible to Universal Adversarial Attacks?](https://aclanthology.org/2022.aacl-main.13/)|[[code]](https://github.com/rainavyas/gec-universal-attack)|
||2023|[ChatBack: Investigating Methods of Providing Grammatical Error Feedback in a GUI-based Language Learning Chatbot](https://aclanthology.org/2023.bea-1.7)||
||2023|[A Closer Look at k-Nearest Neighbors Grammatical Error Correction](https://aclanthology.org/2023.bea-1.19)||
||2023|[Grammatical Error Correction for Sentence-level Assessment in Language Learning](https://aclanthology.org/2023.bea-1.41)||
||2023|[Evaluation Metrics in the Era of GPT-4: Reliably Evaluating Large Language Models on Sequence to Sequence Tasks](https://aclanthology.org/2023.emnlp-main.543/)||
||2024|[[Pillars of Grammatical Error Correction: Comprehensive Inspection Of Contemporary Approaches In The Era of Large Language Models](https://aclanthology.org/2024.bea-1.3)]|[[code]](https://github.com/grammarly/pillars-of-gec)|
||2024|[Likelihood-based Mitigation of Evaluation Bias in Large Language Models](https://aclanthology.org/2024.findings-acl.193)||
||2025|[Rethinking Evaluation Metrics for Grammatical Error Correction: Why Use a Different Evaluation Process than Human?](https://aclanthology.org/2025.acl-short.92/)|[[code]](https://github.com/gotutiyan/gec-metrics)|
||2025|[Improving Explainability of Sentence-level Metrics via Edit-level Attribution for Grammatical Error Correction](https://aclanthology.org/2025.acl-srw.77/)|[[code]](https://github.com/naist-nlp/gec-attribute)|
||2025|[Reliability Crisis of Reference-free Metrics for Grammatical Error Correction](https://aclanthology.org/2025.findings-emnlp.1356/)|[[code]](https://github.com/gotutiyan/attack-gec-metrics)|

# Spoken Domain

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2019|[AUTOMATIC GRAMMATICAL ERROR DETECTION OF NON-NATIVE SPOKEN LEARNER ENGLISH](https://www.repository.cam.ac.uk/bitstream/handle/1810/289493/ICASSP2019_SS__GED-11.pdf?)||
||2020|[Grammatical error detection in transcriptions of spoken English](https://aclanthology.org/2020.coling-main.195.pdf)||
|Disfluency detection (DD) model|2020|[Spoken Language ‘Grammatical Error Correction’](http://www.interspeech2020.org/uploadfile/pdf/Thu-1-8-1.pdf)||
||2022|[On Assessing and Developing Spoken ’Grammatical Error Correction’ Systems](https://aclanthology.org/2022.bea-1.9/)||


# Applications

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|GECko++|| [[GECko+: a Grammatical and Discourse Error Correction Tool]](https://aclanthology.org/2021.jeptalnrecital-demo.3)|[[website]](https://gecko-app.azurewebsites.net) [[code]](https://github.com/psawa/gecko-app)<br>An English assiting tool. Correction grammatical error and re-ordering sentences automatically.|
|MiSS|2021|[[MiSS: An Assistant for Multi-Style Simultaneous Translation]](https://aclanthology.org/2021.emnlp-demo.1/)|[[website]](http://miss.x2brain.com/) [[demo video]](https://www.youtube.com/watch?v=ZGCo7KtRKd8&ab_channel=AnonymousAnonymous)|
|ALLECS|2023|[ALLECS: A Lightweight Language Error Correction System](https://aclanthology.org/2023.eacl-demo.32)|[[website]](https://sterling8.d2.comp.nus.edu.sg/allecs/) [[code]](https://github.com/nusnlp/ALLECS)|
||2023|[Doolittle: Benchmarks and Corpora for Academic Writing Formalization](https://aclanthology.org/2023.emnlp-main.809/)|[[code]](https://github.com/shizhediao/Doolittle)|
||2025|[Who Wrote This? The Key to Zero-Shot LLM-Generated Text Detection Is GECScore](https://aclanthology.org/2025.coling-main.684/)|[[code]](https://github.com/NLP2CT/GECScore)|

# Projects

|Name|Website|
|:--|:--|
|GramFormer|[[GitHub]](https://github.com/PrithivirajDamodaran/Gramformer)|

# Other Tools

|Name|Code|Note|
|:--|:--|:--|
|Lang8-NAIST-extractor| [[code]](https://github.com/tomo-wb/Lang8-NAIST-extractor)|Scripts for extracting error-correct pairs from the Lang-8 Corpus.|
|M2Converter|[[code]](https://github.com/Jason3900/M2Convertor)|Scripts for converting m2 file into source file and target file.|
|EFCamDat-Preprocess| [[code]](https://github.com/NTHU-NLPLAB/EFCamDat-Preprocess)||


# Other materials

|Name|Paper|Note|
|:--|:--|:--|
|NLP-progress|| [[website]](http://nlpprogress.com/english/grammatical_error_correction.html)<br>The performance ranking on some datasets.|
|A Crash Course in Automatic Grammatical Error Correction| [[paper]](https://www.aclweb.org/anthology/2020.coling-tutorials.6/)| [[materials]](https://github.com/grammatical/coling2020-tutorial)<br>The tutorial about GEC in COLING2020.|
|Chunngai/gec-papers ||[[github]](https://github.com/Chunngai/gec-papers/blob/master/README.md)<br>The papers are being compiled around 2019-2020?|


# Related Tasks

### Grammatical Error Detection

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2003|[Automatic Error Detection in the Japanese Learners’ English Spoken Data](https://aclanthology.org/P03-2026/)||
||2006|[Detecting errors in English article usage by non-native speakers](https://www.cambridge.org/core/journals/natural-language-engineering/article/abs/detecting-errors-in-english-article-usage-by-nonnative-speakers/76D03BB128C2CE603325A086FFCB5B41)||
||2008|[The Ups and Downs of Preposition Error Detection in ESL Writing](https://aclanthology.org/C08-1109/)||
||2010|[Evaluating performance of grammatical error detection to maximize learning effect](https://aclanthology.org/C10-2103/)||
|A weighted measure according to crowdsourcing results (for GED)|2011|[[They Can Help: Using Crowdsourcing to Improve the Evaluation of Grammatical Error Detection Systems]](https://aclanthology.org/P11-2089/)||
||2014|[Detecting Learner Errors in the Choice of Content Words Using Compositional Distributional Semantics](https://aclanthology.org/C14-1164/)||
||2016|[Compositional Sequence Labeling Models for Error Detection in Learner Writing](https://aclanthology.org/P16-1112/)||
||2017|[Grammatical Error Detection Using Error- and Grammaticality-Specific Word Embeddings](https://aclanthology.org/I17-1005/)|[[code]](https://github.com/kanekomasahiro/grammatical-error-detection)|
|| 2018| [[Wronging a Right: Generating Better Errors to Improve Grammatical Error Detection]](https://aclanthology.org/D18-1541/)| [[code]](https://github.com/skasewa/wronging)|
|Bi-LSTM with contextual word embeddings|2019|[[Context is Key: Grammatical Error Detection with Contextual Word Representations]](https://aclanthology.org/W19-4410/)||
|Multi-head and multi-layer attention| 2019| [[Multi-Head Multi-Layer Attention to Deep Language Representations for Grammatical Error Detection]](https://arxiv.org/abs/1904.07334)||
||2021| [[Exploring the Capacity of a Large-scale Masked Language Model to Recognize Grammatical Errors]](https://aclanthology.org/2022.findings-acl.324/)||
||2022|[Probing for targeted syntactic knowledge through grammatical error detection](https://aclanthology.org/2022.conll-1.25/)|[[code]](https://github.com/chrisdavis90/ged-syntax-probing)|
||2024|[Zero-shot Cross-Lingual Transfer for Synthetic Data Generation in Grammatical Error Detection](https://aclanthology.org/2024.emnlp-main.176/)|[[data]](https://github.com/Ubisoft-LaForge/ubisoft-laforge-MultiLingualCheck-2M)|
||2025|[Oddballness: universal anomaly detection with language models](https://aclanthology.org/2025.coling-main.183/)|[[code]](https://github.com/richardxoldman/oddballness)|

### Feedback Comment Generation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2014|[[Correcting Preposition Errors in Learner English Using Error Case Frames and Feedback Messages]](https://aclanthology.org/P14-1071)||
|English grammar checker with feedback in Japanese|2018|[[Grammatical Error Checker for Japanese Learners of English]](https://dl.acm.org/doi/abs/10.1145/3274856.3274885)|This is not a research as a feedback comment generation, but I classify it here for now|
||2019|[[Toward a Task of Feedback Comment Generation for Writing Learning]](https://aclanthology.org/D19-1316)||
||2020|[[Creating Corpora for Research in Feedback Comment Generation]](https://aclanthology.org/2020.lrec-1.42/)||
||2021|[[Shared Task on Feedback Comment Generation for Language Learners]](https://aclanthology.org/2021.inlg-1.35/)||
||2023|[Template-guided Grammatical Error Feedback Comment Generation](https://aclanthology.org/2023.eacl-srw.10)||

### Explainable Grammatical Error Correction

- Studies to explain the reasons for and intentions of error correction.

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|EXPECT|2023|[Enhancing Grammatical Error Correction Systems with Explanations](https://aclanthology.org/2023.acl-long.413)|[[code]](https://github.com/lorafei/Explainable_GEC)|
|XGEC dataset|2024|[Controlled Generation with Prompt Insertion for Natural Language Explanations in Grammatical Error Correction](https://aclanthology.org/2024.lrec-main.350/)|[[data]](https://github.com/kanekomasahiro/gec-explanation)|
|GEE|2024|[GEE! Grammar Error Explanation with Large Language Models](https://aclanthology.org/2024.findings-naacl.49)|[[code]](https://github.com/Yixiao-Song/GEE-with-LLMs)|

### Document-level Revision

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|TETRA|2024|[Towards Automated Document Revision: Grammatical Error Correction, Fluency Edits, and Beyond](https://aclanthology.org/2024.bea-1.21)|[[code]](https://github.com/chemicaltree/tetra)|

# Other Languages

### Arabic

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Arabic Learner Corpus|2013|[[Arabic Learner Corpus v1: A New Resource for Arabic Language Research]](https://www.researchgate.net/publication/267600799_Arabic_Learner_Corpus_v1_A_New_Resource_for_Arabic_Language_Research)|[[website]](https://www.arabiclearnercorpus.com/)|
|QALB|2014|[[Large Scale Arabic Error Annotation: Guidelines and Framework]](https://aclanthology.org/L14-1721/)|[[QALB Project Website]](http://nlp.qatar.cmu.edu/qalb/)|
|QALB 2014 Shared Task| 2014| [[The First QALB Shared Task on Automatic Text Correction for Arabic]](https://aclanthology.org/W14-3605/)| [[website]](http://nlp.qatar.cmu.edu/qalb/sharedtask/shared_task.html)|
|QALB 2015 Shared Task| 2015| [[The Second QALB Shared Task on Automatic Text Correction for Arabic]](https://aclanthology.org/W15-3204/)||
|ARETA| 2021| [[Automatic Error Type Annotation for Arabic]](https://aclanthology.org/2021.conll-1.47/)|[[code]](https://github.com/CAMeL-Lab/arabic_error_type_annotation)|
||2023|[Advancements in Arabic Grammatical Error Detection and Correction: An Empirical Investigation](https://aclanthology.org/2023.emnlp-main.396/)|[[code]](https://github.com/CAMeL-Lab/arabic-gec)|
||2023|[Beyond English: Evaluating LLMs for Arabic Grammatical Error Correction](https://aclanthology.org/2023.arabicnlp-1.9/)|[[code]]|
||2025|[ARWI: Arabic Write and Improve](https://aclanthology.org/2025.in2writing-1.2/)|[[website]](https://arwi.mbzuai.ac.ae/)|
||2025|[Enhancing Text Editing for Grammatical Error Correction: Arabic as a Case Study](https://aclanthology.org/2025.acl-long.875/)|[[code]](https://github.com/CAMeL-Lab/text-editing)|

### Bangla

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2021|[[Development of Bangla Spell and Grammar Checkers: Resource Creation and Evaluation]](https://ieeexplore.ieee.org/document/9568876)||
||2025|[Leveraging LLMs for Bangla Grammar Error Correction: Error Categorization, Synthetic Data, and Model Evaluation](https://aclanthology.org/2025.findings-acl.431/)|[[code]](https://github.com/Bangla-iitk/Vaiyakarana)|

### Chinese

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2013|[Chinese Spelling Checker Based on Statistical Machine Translation](https://aclanthology.org/W13-4408/)||
||2014|[Chinese Word Ordering Errors Detection and Correction for Non-Native Chinese Language Learners](https://aclanthology.org/C14-1028/)||
||2015|[Improving Chinese Grammatical Error Correction with Corpus Augmentation and Hierarchical Phrase-based Statistical Machine Translation](https://aclanthology.org/W15-4417/)||
|NLPCC-2018 Shared Task| 2018| [[Overview of the NLPCC 2018 Shared Task: Grammatical Error Correction]](http://tcci.ccf.org.cn/conference/2018/papers/EV11.pdf)| [[data]](https://github.com/zhaoyyoo/NLPCC2018_GEC)
|Two-stage: Spell checker → seq2seq|2019|[[A Two-Stage Model for Chinese Grammatical Error Correction]](https://ieeexplore.ieee.org/document/8830400)||
|CNN-based seq2seq|2019|[[Chinese Grammatical Error Correction Based on Convolutional Sequence to Sequence Model]](https://ieeexplore.ieee.org/document/8717692)||
|MaskGEC| 2020| [[MaskGEC: Improving Neural Grammatical Error Correction via Dynamic Masking]](https://ojs.aaai.org/index.php/AAAI/article/view/5476)||
||2020| [[Chinese Grammatical Error Detection Based on BERT Model]](https://aclanthology.org/2020.nlptea-1.15/)||
||2020| [[BERT Enhanced Neural Machine Translation and Sequence Tagging Model for Chinese Grammatical Error Diagnosis]](https://aclanthology.org/2020.nlptea-1.8/)||
||2020|[[Heterogeneous Recycle Generation for Chinese Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.199/)||
|NLPTEA-2020 Shared Task|2020|[[Overview of NLPTEA-2020 Shared Task for Chinese Grammatical Error Diagnosis]](https://aclanthology.org/2020.nlptea-1.4/)||
|Tail-to-Tail Non-Autoregressive Sequence Prediction| 2021| [[Tail-to-Tail Non-Autoregressive Sequence Prediction for Chinese Grammatical Error Correction]](https://aclanthology.org/2021.acl-long.385/)||
||2021|["Is Whole Word Masking Always Better for Chinese BERT?": Probing on Chinese Grammatical Error Correction](https://aclanthology.org/2022.findings-acl.1/)||
||2022|[Pre-Training-Based Grammatical Error Correction Model for the Written Language of Chinese Hearing Impaired Students](https://ieeexplore.ieee.org/document/9734023)||
||2022|[MuCGEC: a Multi-Reference Multi-Source Evaluation Dataset for Chinese Grammatical Error Correction](https://aclanthology.org/2022.naacl-main.227/)|[[code]](https://github.com/hillzhang1999/mucgec)|
||2022|[Improving Chinese Grammatical Error Detection via Data augmentation by Conditional Error Generation](https://aclanthology.org/2022.findings-acl.233/)|[[code]](https://github.com/tc-yue/DA_CGED)|
||2022|[String Editing Based Chinese Grammatical Error Diagnosis](https://aclanthology.org/2022.coling-1.474/)||
|CLG|2022|[Linguistic Rules-Based Corpus Generation for Native Chinese Grammatical Error Correction](https://aclanthology.org/2022.findings-emnlp.40/)|[[code]](https://github.com/masr2000/CLG-CGEC)|
||2022|[From Spelling to Grammar: A New Framework for Chinese Grammatical Error Correction](https://aclanthology.org/2022.findings-emnlp.63/)||
|FCGEC|2022|[FCGEC: Fine-Grained Corpus for Chinese Grammatical Error Correction](https://aclanthology.org/2022.findings-emnlp.137/)|[[code]](https://github.com/xlxwalex/FCGEC)|
||2023|[Are Pre-trained Language Models Useful for Model Ensemble in Chinese Grammatical Error Correction?](https://aclanthology.org/2023.acl-short.77)|[[code]](https://github.com/JamyDon/PLM-based-CGEC-Model-Ensemble)|
||2023|[Focal Training and Tagger Decouple for Grammatical Error Correction](https://aclanthology.org/2023.findings-acl.370)||
|NaSGEC|2023|[NaSGEC: a Multi-Domain Chinese Grammatical Error Correction Dataset from Native Speaker Texts](https://aclanthology.org/2023.findings-acl.630)|[[code]](https://github.com/HillZhang1999/NaSGEC)|
|TLM|2023|[TLM: Token-Level Masking for Transformers](https://aclanthology.org/2023.emnlp-main.871/)|[[code]](https://github.com/Young1993/tlm)|
||2024|[LM-Combiner: A Contextual Rewriting Model for Chinese Grammatical Error Correction](https://aclanthology.org/2024.lrec-main.934/)|[[code]](https://github.com/wyxstriker/LM-Combiner)|
|Alirector|2024|[Alirector: Alignment-Enhanced Chinese Grammatical Error Corrector](https://aclanthology.org/2024.findings-acl.148)|[[code]](https://github.com/yanghh2000/Alirector)|
||2024|[Towards Better Utilization of Multi-Reference Training Data for Chinese Grammatical Error Correction](https://aclanthology.org/2024.findings-acl.180)|[[code]](https://github.com/ymliucs/MrGEC)|
||2024|[Towards Explainable Chinese Native Learner Essay Fluency Assessment: Dataset, Tasks, and Method](https://aclanthology.org/2024.findings-emnlp.910/)|[[code]](https://github.com/cubenlp/CEFA)|
||2025|[Improving Automatic Grammatical Error Annotation for Chinese Through Linguistically-Informed Error Typology](https://aclanthology.org/2025.coling-main.189/)|[[website]](https://open-writing-evaluation.github.io/)|
||2025|[A Chain-of-Task Framework for Instruction Tuning of LLMs Based on Chinese Grammatical Error Correction](https://aclanthology.org/2025.coling-main.577/)|[[code]](https://github.com/lxp991108/CoCGEC)|
|VisCGEC|2025|[VisCGEC: Benchmarking the Visual Chinese Grammatical Error Correction](https://aclanthology.org/2025.naacl-long.261/)|[[code]](https://github.com/xiaoAugenstern/VisCGEC)|
||2025|[Rethinking the Roles of Large Language Models in Chinese Grammatical Error Correction](https://aclanthology.org/2025.acl-industry.39/)|[[code]](https://github.com/THUKElab/LLM4CGEC)|

### Czech

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|AKCES-GEC dataset| 2019| [[Grammatical Error Correction in Low-Resource Scenarios]](https://aclanthology.org/D19-5545)| [[data]](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-3057)|
|Grammar Error Correction Corpus for Czech (GECCC)|2022|[Czech Grammar Error Correction with a Large and Diverse Corpus](https://arxiv.org/abs/2201.05590)|[[data]](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-4639)|

### Estonian

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2025|[Paragraph-level Error Correction and Explanation Generation: Case Study for Estonian](https://aclanthology.org/2025.bea-1.72/)|[[data]](https://github.com/tlu-dt-nlp/EstGEC-L2-Corpus/)|

### Finnish
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2024|[Correcting Challenging Finnish Learner Texts With Claude, GPT-3.5 and GPT-4 Large Language Models](https://aclanthology.org/2024.wnut-1.1/)
||

### Geek

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Greek Learner Corpus|2018|[[Stand-off annotation in learner corpora: compiling the Greek Learner Corpus (GLC)]](https://www.researchgate.net/publication/328542477_Stand-off_annotation_in_learner_corpora_compiling_the_Greek_Learner_Corpus_GLC)||
|ELERRANT|2021|[[ELERRANT: Automatic Grammatical Error Type Classification for Greek]](https://aclanthology.org/2021.ranlp-1.81/)|[[code]](https://github.com/katkorre/elerrant)|

### German

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Falko-MERLIN dataset|2018| [[Using Wikipedia Edits in Low Resource Grammatical Error Correction]](https://aclanthology.org/W18-6111/)| [[data]](https://github.com/adrianeboyd/boyd-wnut2018/)|

### Indian

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2014|[[Detection and correction of non word spelling errors in Hindi language]](https://ieeexplore.ieee.org/abstract/document/6954235)||
|HiWikiEd dataset|2020|[[Generating Inflectional Errors for Grammatical Error Correction in Hindi]](https://aclanthology.org/2020.aacl-srw.24/)|[[data]](https://github.com/s-ankur/hindi_grammar_correction)|
|Hi-GEC|2025|[Hi-GEC: Hindi Grammar Error Correction in Low Resource Scenario](https://aclanthology.org/2025.coling-main.406/)|[[code]](https://github.com/ujjwalsharmaIITB/Hi-GEC)|
|IndiGEC|2025|[IndiGEC: Multilingual Grammar Error Correction for Low-Resource Indian Languages](https://aclanthology.org/2025.emnlp-main.1139/)|[[code]](https://github.com/ujjwalsharmaIITB/IndiGEC)|

### Icelandic
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Byte-level approach|2023|[Byte-Level Grammatical Error Correction Using Synthetic and Curated Corpora](https://aclanthology.org/2023.acl-long.402)|[[code]](https://github.com/mideind/byte-gec)|


### Japanese

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Character-level RNN-based seq2seq|2018|[[Automatic Error Correction on Japanese Functional Expressions Using Character-based Neural Machine Translation]](https://aclanthology.org/Y18-1046/)||
|Constructing retrieval system for Japanese GEC|2019|[[Grammatical-Error-Aware Incorrect Example Retrieval System for Learners of Japanese as a Second Language]](https://aclanthology.org/W19-4431.pdf)||
|TMU Evaluation Corpus for Japanese Learners|2020| [[Construction of an Evaluation Corpus for Grammatical Error Correction for Learners of Japanese as a Second Language]](https://aclanthology.org/2020.lrec-1.26/)| [[data: Fill this form]](https://docs.google.com/forms/d/e/1FAIpQLSdBOoRuHaDuBuwuuYHrz6ILR6LQqIPw3AUL6XVEmvDFg8z_wQ/viewform)|
|Non-Autoregressive approach|2020|[[Non-Autoregressive Grammatical Error Correction Toward a Writing Support System]](https://aclanthology.org/2020.nlptea-1.1/)||
||2022|[Construction of a Quality Estimation Dataset for Automatic Evaluation of Japanese Grammatical Error Correction](https://arxiv.org/abs/2201.08038)||

### Korean
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|KAGAS|2023|[Towards standardizing Korean Grammatical Error Correction: Datasets and Annotation](https://aclanthology.org/2023.acl-long.371)|[[code]](https://github.com/soyoung97/Standard_Korean_GEC) [[data request form]](https://docs.google.com/forms/d/e/1FAIpQLSfewjAmqcrKF5GDYuIWOfyMVBI3FN6tCwI8jalzQNhGoVAlRg/viewform)|
||2024|[Search if you don’t know! Knowledge-Augmented Korean Grammatical Error Correction with Large Language Models](https://aclanthology.org/2024.findings-emnlp.6/)||
||2025|[Unified Automated Essay Scoring and Grammatical Error Correction](https://aclanthology.org/2025.findings-naacl.250/)||

### Lithuanian
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2022|[Towards Lithuanian grammatical error correction](https://arxiv.org/abs/2203.09963)|[[code]](https://github.com/lukasstankevicius/towards-lithuanian-grammatical-error-correction)|

### Romain

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2020|[[Neural Grammatical Error Correction for Romanian]](https://ieeexplore.ieee.org/abstract/document/9288338)|[[code]](https://github.com/teodor-cotet/RoGEC)|

### Russian

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|RULEC-GEC dataset|2019| [[Grammar Error Correction in Morphologically Rich Languages: The Case of Russian]](https://aclanthology.org/Q19-1001/)| [[data]](https://github.com/arozovskaya/RULEC-GEC)|
|RU-Lang8 dataset|2021| [[New Dataset and Strong Baselines for the Grammatical Error Correction of Russian]](https://aclanthology.org/2021.findings-acl.359/)| [[data]](https://github.com/arozovskaya/RU-Lang8)|
|Additional annotations for RULEC and RU-Lang8|2024|[Multi-Reference Benchmarks for Russian Grammatical Error Correction](https://aclanthology.org/2024.eacl-long.76/)|[[RULEC]](https://github.com/arozovskaya/RULEC-GEC) [[RU-Lang8]](https://github.com/arozovskaya/RU-Lang8)|
||2024|[Universal Dependencies for Learner Russian](https://aclanthology.org/2024.lrec-main.1486/)|[[code]](https://github.com/arozovskaya/dependency-learner-russian)|
||2025|[Grammatical Error Correction via Sequence Tagging for Russian](https://aclanthology.org/2025.acl-srw.82/)|[[code]](https://github.com/ReginaNasyrova/RussianGEC_SeqTagger)|
|LORuGEC|2025|[LLMs in alliance with Edit-based models: advancing In-Context Learning for Grammatical Error Correction by Specific Example Selection](https://aclanthology.org/2025.bea-1.38/)|[[data]](https://github.com/ReginaNasyrova/LORuGEC) [[code]](https://github.com/AlexeySorokin/LORuGEC)|

### Spanish

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|COWS-L2H|2020|[[Developing NLP Tools with a New Corpus of Learner Spanish]](https://aclanthology.org/2020.lrec-1.894/)|[[data]](https://github.com/ucdaviscl/cowsl2h)|

### Swedish

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2024|[Evaluation of Really Good Grammatical Error Correction](https://aclanthology.org/2024.lrec-main.584/)|[code](https://github.com/robertostling/gec-evaluation)|

### Turkish
|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|ERRANT-TR|2023|[Towards Automatic Grammatical Error Type Classification for Turkish](https://aclanthology.org/2023.eacl-srw.14)|[[code]](https://github.com/harunuz/erranttr)|
|GECTurk WEB|2025|[GECTurk WEB: An Explainable Online Platform for Turkish Grammatical Error Detection and Correction](https://aclanthology.org/2025.coling-demos.16/)|[[website]](https://www.gecturk.net/)|

### Ukrainian

Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|UA-GEC|2023|[[UA-GEC: Grammatical Error Correction and Fluency Corpus for the Ukrainian Language]](https://aclanthology.org/2023.unlp-1.12/)|[[data]](https://github.com/grammarly/ua-gec)|
|UNLP 2023 Shared Task|2023|[The UNLP 2023 Shared Task on Grammatical Error Correction for Ukrainian](https://aclanthology.org/2023.unlp-1.16)||
||2023|[Comparative Study of Models Trained on Synthetic Data for Ukrainian Grammatical Error Correction](https://aclanthology.org/2023.unlp-1.13)|UNLP-2023: Pravopysnyk|
||2023|[A Low-Resource Approach to the Grammatical Error Correction of Ukrainian](https://aclanthology.org/2023.unlp-1.14)|UNLP-2023: QC-NLP|
||2023|[RedPenNet for Grammatical Error Correction: Outputs to Tokens, Attentions to Spans](https://aclanthology.org/2023.unlp-1.15)|UNLP-2023: WebSpellChecker|
