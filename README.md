# GEC Information

### Policy
- This repository aims to collect and categorize GEC (Grammatical Error Correction) papers.
- Unlike NLP-progress, we do not consider performances on benchmarks.
- The papers are limited to refereed-papers for now (This is not the case with survey papers).

### Contributing
- Pull Requests for adding papers are accepted. Please make a commit changing only lines regarding the addition of papers (and take care of changing by auto-formatting).
- You can also request to add papers as an [issue](https://github.com/gotutiyan/GEC-Info/issues).

It can also be viewed on [GitHub Pages](https://gotutiyan.github.io/GEC-Info/)

# Overview

* [Surveys](https://github.com/gotutiyan/GEC-Info#surveys)
* [Shared Tasks](https://github.com/gotutiyan/GEC-Info#shared-tasks)
* [Datasets](https://github.com/gotutiyan/GEC-Info#datasets)
  * [For Training](https://github.com/gotutiyan/GEC-Info#for-training-real-data)
  * [For Evaluation](https://github.com/gotutiyan/GEC-Info#for-evaluation)
* [Performance Measures](https://github.com/gotutiyan/GEC-Info#performance-measures)
  * [Reference-based](https://github.com/gotutiyan/GEC-Info#reference-based)
  * [Reference-less](https://github.com/gotutiyan/GEC-Info#reference-less)
* [Quality Estimation](https://github.com/gotutiyan/GEC-Info#quality-estimation)
* [Models / Methods](https://github.com/gotutiyan/GEC-Info#models--methods)
  * [Supervised](https://github.com/gotutiyan/GEC-Info#supervised)
  * [Unsupervised](https://github.com/gotutiyan/GEC-Info#unsupervised)
* [Ensemble Methods](https://github.com/gotutiyan/GEC-Info#ensemble-methods)
* [Strategies](https://github.com/gotutiyan/GEC-Info#strategies)
* [Data Augmentation](https://github.com/gotutiyan/GEC-Info#data-augmentation)
* [Analyses / Findings](https://github.com/gotutiyan/GEC-Info#analyses--findings)
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
  * [Japanese](https://github.com/gotutiyan/GEC-Info#japanese)
  * [Lithuanian](https://github.com/gotutiyan/GEC-Info#lithuanian)
  * [Romain](https://github.com/gotutiyan/GEC-Info#romain)
  * [Russian](https://github.com/gotutiyan/GEC-Info#russian)
  * [Spanish](https://github.com/gotutiyan/GEC-Info#spanish)
  * [Ukrainian](https://github.com/gotutiyan/GEC-Info#ukrainian)


# Surveys

|Title|Year|Page|Note|
|:--|:--|:--|:--|
|"Automated Grammatical Error Correction: A Comprehensive Review"|2017|[[paper]](https://www.journals.nust.edu.pk/index.php/njes/article/download/219/100)||
|"A Comprehensive Survey of Grammar Error Correction"|2020|[[paper]](https://arxiv.org/abs/2005.06600)||
|"Recent Trends in the Use of Deep Learning Models for Grammar Error Handling" |2020|[[paper]](https://arxiv.org/abs/2009.02358)||

# Shared Tasks

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|HOO 2011|2011| [[paper]](https://aclanthology.org/W11-2838/)| [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2011)|
|HOO 2012|2012| [[paper]](https://aclanthology.org/W12-2006)| [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2012-shared-task-on-preposition-and-determiner-error-correction)|
|CoNLL-2013|2013| [[paper]](https://aclanthology.org/W13-3601/)| [[website]](https://www.comp.nus.edu.sg/~nlp/conll13st.html)|
|CoNLL-2014|2014| [[paper]](https://aclanthology.org/W14-1701/)| [[website]](https://www.comp.nus.edu.sg/~nlp/conll14st.html) [[system outputs]](https://www.comp.nus.edu.sg/~nlp/conll14st/official_submissions.tar.gz)|
|BEA-2019|2019| [[paper]](https://aclanthology.org/W19-4406/)| [[website]](https://www.cl.cam.ac.uk/research/nl/bea2019st/) [[system outpus]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/system_output.bea19.tar.gz)|


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

### Reference-less

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Scoring by counting the errors|2016|[[There’s No Comparison: Reference-less Evaluation Metrics in Grammatical Error Correction]](https://aclanthology.org/D16-1228)|[[code]](https://github.com/cnap/grammaticality-metrics)|
|Fluency + grammaticality + meaning preservation| 2017| [[Reference-based Metrics can be Replaced with Reference-less Metrics in Evaluating Grammatical Error Correction Systems]](https://aclanthology.org/I17-2058)||
|USim| 2018| [[Reference-less Measure of Faithfulness for Grammatical Error Correction]](https://aclanthology.org/N18-2020/)| [[code]](https://github.com/borgr/USim)|
|SOME|2020| [[SOME: Reference-less Sub-Metrics Optimized for Manual Evaluations of Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.573)| [[code]](https://github.com/kokeman/SOME)|
|Scribendi Score|2021|[[Is this the end of the gold standard? A straightforward reference-less grammatical error correction metric]](https://aclanthology.org/2021.emnlp-main.239/)|[[Unofficial code]](https://github.com/gotutiyan/scribendi_score)|

# Quality Estimation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2022|[Proficiency Matters Quality Estimation in Grammatical Error Correction](https://arxiv.org/abs/2201.06199)||


# Models / Architectures

### Supervised

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
|Neural reinforcement learning|2017|[[Grammatical Error Correction with Neural Reinforcement Learning]](https://aclanthology.org/I17-2062/)|[[code]](https://github.com/keisks/nematus/tree/nrl-gleu)|
|Word-level SMT enhanced NNJMs + char-based SMT|2017|[[Connecting the Dots: Towards Human-Level Grammatical Error Correction]](https://aclanthology.org/W17-5037)|[[code]](https://github.com/nusnlp/smtgec2017)|
|First NMT-based approach|2016|[[Grammatical error correction using neural machine translation]](https://aclanthology.org/N16-1042/)||
||2016|[Neural Network Translation Models for Grammatical Error Correction](https://arxiv.org/abs/1606.00189)||
|SMEG|2017|[[Systematically Adapting Machine Translation for Grammatical Error Correction]](https://aclanthology.org/W17-5039)|[[code]](https://github.com/cnap/smt-for-gec)|
|A nested attention (word and char attention)|2017|[[A Nested Attention Neural Hybrid Model for Grammatical Error Correction]](https://aclanthology.org/P17-1070)||
|Re-ranking N-best sentence (by SMT) with LSTM-based GED|2017|[[Neural Sequence-Labelling Models for Grammatical Error Correction]](https://aclanthology.org/D17-1297/)||
|CNN-based Encder-Decoder approach| 2018|[[A Multilayer Convolutional Encoder-Decoder Neural Network for Grammatical Error Correction]](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/17308/16137)|[[code]](https://github.com/nusnlp/mlconvgec2018)|
|Fluency boosting learning|2018|[[Fluency Boost Learning and Inference for Neural Grammatical Error Correction]](https://aclanthology.org/P18-1097)|[[code]](https://github.com/getao/human-performance-gec)<br>ACL2018|
|Fluency boosting learning (added round-way error correction)|2018|[[Reaching Human-level Performance in Automatic Grammatical Error Correction: An Empirical Study]](https://arxiv.org/abs/1807.01270)|[[code]](https://github.com/getao/human-performance-gec)<br>Microsoft Research Technical Report|
|Hybrid SMT and NMT|2018|[[Near Human-Level Performance in Grammatical Error Correction with Hybrid Machine Translation]](https://aclanthology.org/N18-2046)||
|Copy-Augmented Architecture|2019|[[Improving Grammatical Error Correction via Pre-Training a Copy-Augmented Architecture with Unlabeled Data]](https://aclanthology.org/N19-1014)|[[code]](https://github.com/yuantiku/fairseq-gec)|
|Consider a few previous sentences|2019|[[Cross-Sentence Grammatical Error Correction]](https://aclanthology.org/P19-1042)|[[code]](https://github.com/nusnlp/crosentgec)|
|PIE|2019|[[Parallel Iterative Edit Models for Local Sequence Transduction]](https://aclanthology.org/D19-1435/)|[[code]](https://github.com/awasthiabhijeet/PIE)|
|LaserTagger|2019|[[Encode, Tag, Realize: High-Precision Text Editing]](https://aclanthology.org/D19-1510/)|[[code]](https://github.com/google-research/lasertagger)|
|Pretrain by DAE + sequential transfer learning|2019|[[A Neural Grammatical Error Correction System Built On Better Pre-training and Sequential Transfer Learning]](https://aclanthology.org/W19-4423/)|[[code]](https://github.com/kakaobrain/helo_word)<br>BEA-2019: Kakao&Brain|
|Use sentence-level error dectection| 2019|[[The AIP-Tohoku System at the BEA-2019 Shared Task]](https://aclanthology.org/W19-4418)|BEA-2019: AIP-Tohoku||
|Four CNN + eight Transformer|2019|[[The LAIX Systems in the BEA-2019 GEC Shared Task]](https://aclanthology.org/W19-4416)|BEA-2019: LAIX|
|Combine Transformer+CNN with FST + Re-ranking|2019|[[Neural and FST-based approaches to grammatical error correction]](https://aclanthology.org/W19-4424)|BEA-2019: CAMB-CLED|
|Transformer seq2seq + BERT re-ranker|2019|[[TMU Transformer System Using BERT for Re-ranking at BEA 2019 Grammatical Error Correction on Restricted Track]](https://aclanthology.org/W19-4422)|BEA-2019: TMU|
|Apply noisy channel with BERT and GPT-2 as LM|2019|[[Noisy Channel for Low Resource Grammatical Error Correction]](https://aclanthology.org/W19-4420.pdf)|BEA-2019: Siteimprove|
|Use Finite State Transducers|2019|[[Neural Grammatical Error Correction with Finite State Transducers]](https://aclanthology.org/N19-1406)||
|GECToR|2020|[[GECToR – Grammatical Error Correction: Tag, Not Rewrite]](https://aclanthology.org/2020.bea-1.16/)|[[code]](https://github.com/grammarly/gector)|
|BERT-fuse|2020|[[Encoder-Decoder Models Can Benefit from Pre-trained Masked Language Models in Grammatical Error Correction]](https://aclanthology.org/2020.acl-main.391/)|[[code]](https://github.com/kanekomasahiro/bert-gec)|
|Adversarial approach (G:seq2seq D:sentence-pair classification)|2020|[[Adversarial Grammatical Error Correction]](https://aclanthology.org/2020.findings-emnlp.275)||
|Erroneous span correction and detection|2020|[[Improving the Efficiency of Grammatical Error Correction with Erroneous Span Detection and Correction]](https://aclanthology.org/2020.emnlp-main.581/)||
|Document-level approach|2020|[[Document-level grammatical error correction]](https://aclanthology.org/2021.bea-1.8/)|[[code]](https://github.com/chrisjbryant/doc-gec)|
|Seq2Edits|2020|[[Seq2Edits: Sequence Transduction Using Span-level Edit Operations]](https://aclanthology.org/2020.emnlp-main.418/)|[[code]](https://github.com/tensorflow/tensor2tensor/blob/master/tensor2tensor/models/research/transformer_seq2edits.py)|
|Beam search considering copy probability|2020|[[Generating Diverse Corrections with Local Beam Search for Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.193)||
|BART-based|2020|[[Stronger Baselines for Grammatical Error Correction Using a Pretrained Encoder-Decoder Model]](https://aclanthology.org/2020.aacl-main.83)|[[code]](https://github.com/Katsumata420/generic-pretrained-GEC)|
|VERNet|2021|[[Neural Quality Estimation with Multiple Hypotheses for Grammatical Error Correction]](https://aclanthology.org/2021.naacl-main.429)|[[code]](https://github.com/thunlp/VERNet)|
|Shallow Aggressive Decoding|2021|[[Instantaneous Grammatical Error Correction with Shallow Aggressive Decoding]](https://aclanthology.org/2021.acl-long.462/)|[[code]](https://github.com/AutoTemp/Shallow-Aggressive-Decoding)|
|T5-based|2021|[[A Simple Recipe for Multilingual Grammatical Error Correction]](https://arxiv.org/abs/2106.03830)|[[code]](https://github.com/google-research-datasets/clang8)|
|GAN-like sequence labeling|2021|[[Grammatical Error Correction as GAN-like Sequence Labeling]](https://aclanthology.org/2021.findings-acl.290/)||
|Use multiclass GED for Transformer seq2seq and reranking|2021|[[Multi-Class Grammatical Error Detection for Correction: A Tale of Two Systems]](https://aclanthology.org/2021.emnlp-main.687/)||
|GEC for writing improvement model adapted to the writer’s L1|2021|[[Beyond Grammatical Error Correction: Improving L1-influenced research writing in English using pre-trained encoder-decoder models]](https://aclanthology.org/2021.findings-emnlp.216/)|[[code]](https://github.com/gzomer/BeyondGEC)|
|Constrastive Leaning approach|2021|[[Grammatical Error Correction with Contrastive Learning in Low Error Density Domains]](https://aclanthology.org/2021.findings-emnlp.419/)|[[code]](https://github.com/nusnlp/geccl)|
|Sequence Span Rewriting|2021|[[Improving Sequence-to-Sequence Pre-training via Sequence Span Rewriting]](https://aclanthology.org/2021.emnlp-main.45/)||
|Dependent Self-Attention (DSA)|2021|[[Grammatical Error Correction with Dependency Distance]](https://dl.acm.org/doi/abs/10.1145/3459637.3482348)||
||2021|[Efficient Grammatical Error Correction with Hierarchical Error Detections and Correction](https://ieeexplore.ieee.org/document/9590395)|[[code]](https://github.com/AnticPan/Hierarchical-GEC)|
|A GEC model using only 11.6MB|2021|[An efficient system for grammatical error correction on mobile devices](https://ieeexplore.ieee.org/document/9364435)||
||2022|[Interpretability for Language Learners Using Example-Based Grammatical Error Correction](https://aclanthology.org/2022.acl-long.496/)|[[code]](https://github.com/kanekomasahiro/eb-gec)|
||2022|[Type-Driven Multi-Turn Corrections for Grammatical Error Correction](https://aclanthology.org/2022.findings-acl.254/)|[[code]](https://github.com/deeplearnxmu/tmtc)|
|GECToR Large|2022|[Ensembling and Knowledge Distilling of Large Sequence Taggers for Grammatical Error Correction](https://aclanthology.org/2022.acl-long.266/)|[[code]](https://github.com/makstarnavskyi/gector-large) [[Author's Master Thesis]](https://drive.google.com/file/d/17-qXILfafHR8Uv2Y9plcB9WVRdZLazzp/view)|

### Unsupervised

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|5-gram LM based approach| 2018| [[Language Model Based Grammatical Error Correction without Annotated Training Data]](https://aclanthology.org/W18-0529/)| [[code]](https://github.com/chrisjbryant/lmgec-lite)|
|Train GRU models for each of five error types|2018|[[A Simple but Effective Classification Model for Grammatical Error Correction]](https://arxiv.org/abs/1807.00488)||
|Use Finite State Transducers|2019| [[Neural Grammatical Error Correction with Finite State Transducers]](https://aclanthology.org/N19-1406)||
|LSTM tagger for word coice task|2019|[[Choosing the Right Word: Using Bidirectional LSTM Tagger for Writing Support Systems]](https://arxiv.org/abs/1901.02490)|[[code]](https://github.com/vicmak/Exploiting-BiLSTM-for-Proper-Word-Choice)|
|Use LM (BERT, GPT-1,2)|2019|[[The Unreasonable Effectiveness of Transformer Language Models in Grammatical Error Correction]](https://aclanthology.org/W19-4412/)||
|Create erroneous data from monolingual data|2019|[[Minimally-Augmented Grammatical Error Correction]](https://aclanthology.org/D19-5546)|Supervised setting is also performed|
|LM-Critic| 2021| [[LM-Critic: Language Models for Unsupervised Grammatical Error Correction]](https://aclanthology.org/2021.emnlp-main.611/)| [[code]](https://github.com/michiyasunaga/LM-Critic)<br>Supervised setting is also performed|

# Ensemble Methods

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Use MENT|2014|[System Combination for Grammatical Error Correction](https://aclanthology.org/D14-1102/)||
||2016|[Grammatical Error Correction: Machine Translation and Classifiers](https://aclanthology.org/P16-1208)||
||2019|[[Learning to combine Grammatical Error Corrections]](https://aclanthology.org/W19-4414/)|[[code]](https://github.com/IBM/learning-to-combine-grammatical-error-corrections)|
|Diversity-Driven Combination (DDC)|2021|[[Diversity-Driven Combination for Grammatical Error Correction]](https://arxiv.org/abs/2110.15149)|[[code]](https://github.com/nusnlp/gec-ddc)|
|Select a system for each error type with IP|2021|[[System Combination for Grammatical Error Correction Based on Integer Programming]](https://aclanthology.org/2021.ranlp-1.94/)|[[code]](https://github.com/nusnlp/gec_ip)|
||2022|[Frustratingly Easy System Combination for Grammatical Error Correction](https://aclanthology.org/2022.naacl-main.143/)|[[code]](https://github.com/nusnlp/esc)|


# Strategies

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

# Data Augmentation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Make artificial errors in a probabilistic manner|2014|[[Generating artificial errors for grammatical error correction]](https://aclanthology.org/E14-3013/)||
|Back translation|2016|[[Improving Neural Machine Translation Models with Monolingual Data]](https://aclanthology.org/P16-1009/)||
|SMT based MT + pattern extraction|2017|[[Artificial Error Generation with Machine Translation and Syntactic Patterns]](https://aclanthology.org/W17-5032)||
|Diverse back translation with noisy beam search|2018|[[Noising and Denoising Natural Language: Diverse Backtranslation for Grammar Correction]](https://aclanthology.org/N18-1057/)||
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

### Data Cleaning

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|A Self-Refinement Strategy for Noise Reduction|2020|[[A Self-Refinement Strategy for Noise Reduction in Grammatical Error Correction]](https://aclanthology.org/2020.findings-emnlp.26/)||
|cLang8 (Cleaned Lang-8)|2021| [[A Simple Recipe for Multilingual Grammatical Error Correction]](https://aclanthology.org/2021.acl-short.89/)| [[code]](https://github.com/google-research-datasets/clang8)|


# Analyses / Findings

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2011|[Algorithm Selection and Model Adaptation for ESL Correction Tasks](https://aclanthology.org/P11-1093.pdf)||
||2012|[The Effect of Learner Corpus Size in Grammatical Error Correction of ESL Writings](https://aclanthology.org/C12-2084/)||
|Re-rank the CoNLL14 systems by human evaluation|2015| [[Human Evaluation of Grammatical Error Correction Systems]](https://aclanthology.org/D15-1052/)| [[code]](https://github.com/grammatical/evaluation/)|
||2015| [[How Far are We from Fully Automatic High Quality Grammatical Error Correction?]](https://aclanthology.org/P15-1068)||
|Human annotation focused on fluency |2016| [[Reassessing the Goals of Grammatical Error Correction: Fluency Instead of Grammaticality]](https://aclanthology.org/Q16-1013)|[[code]](https://github.com/keisks/reassess-gec)|
||2017| [[GEC into the future: Where are we going and how do we get there?]](https://aclanthology.org/W17-5019/)||
|MEAGE| 2018| [[Automatic Metric Validation for Grammatical Error Correction]](https://aclanthology.org/P18-1127)| [[code]](https://github.com/borgr/EoE)|
||2018| [[Inherent Biases in Reference-based Evaluation for Grammatical Error Correction]](https://aclanthology.org/P18-1059/)| [[code]](https://github.com/borgr/IBGEC)|
||2018|[[Assessing Grammatical Correctness in Language Learning]](https://aclanthology.org/2021.bea-1.15/)||
|Reassess M^2, I-measure, GLEU by comparing human evaluation|2018| [[A Reassessment of Reference-Based Grammatical Error Correction Metrics]](https://aclanthology.org/C18-1231) |[[code]](https://github.com/nusnlp/gecmetrics)|
|Quality estimation (and re-ranking using estimated score)|2018|[[Neural Quality Estimation of Grammatical Error Correction]](https://aclanthology.org/D18-1274/)|[[code]](https://github.com/nusnlp/neuqe)|
|Evaluate four systems (SMT, CNN, LSTM, Transformer) for six corpora (CoNLL13&14, FCE, JFLEG, KJ, ICNALE)|2019| [[Cross-Corpora Evaluation and Analysis of Grammatical Error Correction Models — Is Single-Corpus Evaluation Enough?]](https://aclanthology.org/N19-1132/) ||
|Compare CNN, Transformer, PRPN, ON-LSTM as back-translation models|2019|[[The Unbearable Weight of Generating Artificial Errors for Grammatical Error Correction]](https://aclanthology.org/W19-4449)||
|GEC for post-processing|2019|[Automatic Grammatical Error Correction for Sequence-to-sequence Text Generation: An Empirical Study](https://aclanthology.org/P19-1609/)||
|CGOP|2020|[[Comparison of the Evaluation Metrics for Neural Grammatical Error Correction With Overcorrection]](https://ieeexplore.ieee.org/document/9102992)|Metric Considering overcorrection|
|Create new gold data by post-editing system outputs|2021| [[How Good (really) are Grammatical Error Correction Systems?]](https://aclanthology.org/2021.eacl-main.231/)||
|Explore whether models have grammatical knowledge with Known-setting and Unknown-setting|2021| [[Do Grammatical Error Correction Models Realize Grammatical Generalization?]](https://aclanthology.org/2021.findings-acl.399/)||
|Compare CNN, LSTM, transformer or combinations of them as BT models|2021| [[Comparison of Grammatical Error Correction Using Back-Translation Models]](https://aclanthology.org/2021.naacl-srw.16/)||
||2022|[Uncertainty Determines the Adequacy of the Mode and the Tractability of Decoding in Sequence-to-Sequence Models](https://aclanthology.org/2022.acl-long.591/)||

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

### Feedback Comment Generation

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2014|[[Correcting Preposition Errors in Learner English Using Error Case Frames and Feedback Messages]](https://aclanthology.org/P14-1071)||
|English grammar checker with feedback in Japanese|2018|[[Grammatical Error Checker for Japanese Learners of English]](https://dl.acm.org/doi/abs/10.1145/3274856.3274885)|This is not a research as a feedback comment generation, but I classify it here for now|
||2019|[[Toward a Task of Feedback Comment Generation for Writing Learning]](https://aclanthology.org/D19-1316)||
||2020|[[Creating Corpora for Research in Feedback Comment Generation]](https://aclanthology.org/2020.lrec-1.42/)||
||2021|[[Shared Task on Feedback Comment Generation for Language Learners]](https://aclanthology.org/2021.inlg-1.35/)||


# Other Languages

### Arabic

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Arabic Learner Corpus|2013|[[Arabic Learner Corpus v1: A New Resource for Arabic Language Research]](https://www.researchgate.net/publication/267600799_Arabic_Learner_Corpus_v1_A_New_Resource_for_Arabic_Language_Research)|[[website]](https://www.arabiclearnercorpus.com/)|
|QALB|2014|[[Large Scale Arabic Error Annotation: Guidelines and Framework]](https://aclanthology.org/L14-1721/)|[[QALB Project Website]](http://nlp.qatar.cmu.edu/qalb/)|
|QALB 2014 Shared Task| 2014| [[The First QALB Shared Task on Automatic Text Correction for Arabic]](https://aclanthology.org/W14-3605/)| [[website]](http://nlp.qatar.cmu.edu/qalb/sharedtask/shared_task.html)|
|QALB 2015 Shared Task| 2015| [[The Second QALB Shared Task on Automatic Text Correction for Arabic]](https://aclanthology.org/W15-3204/)||
|ARETA| 2021| [[Automatic Error Type Annotation for Arabic]](https://aclanthology.org/2021.conll-1.47/)|[[code]](https://github.com/CAMeL-Lab/arabic_error_type_annotation)|

### Bangla

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2021|[[Development of Bangla Spell and Grammar Checkers: Resource Creation and Evaluation]](https://ieeexplore.ieee.org/document/9568876)||

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

### Czech

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|AKCES-GEC dataset| 2019| [[Grammatical Error Correction in Low-Resource Scenarios]](https://aclanthology.org/D19-5545)| [[data]](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-3057)|
|Grammar Error Correction Corpus for Czech (GECCC)|2022|[Czech Grammar Error Correction with a Large and Diverse Corpus](https://arxiv.org/abs/2201.05590)|[[data]](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-4639)|

### Geek

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Greek Learner Corpus|2018|[[Stand-off annotation in learner corpora: compiling the Greek Learner Corpus (GLC)]](https://www.researchgate.net/publication/328542477_Stand-off_annotation_in_learner_corpora_compiling_the_Greek_Learner_Corpus_GLC)||
|ELERRANT|2021|[[ELERRANT: Automatic Grammatical Error Type Classification for Greek]](https://aclanthology.org/2021.ranlp-1.81/)|[[code]](https://github.com/katkorre/elerrant)|

### German

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Falko-MERLIN dataset|2018| [[Using Wikipedia Edits in Low Resource Grammatical Error Correction]](https://aclanthology.org/W18-6111/)| [[data]](https://github.com/adrianeboyd/boyd-wnut2018/)|

### Hindi

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
||2014|[[Detection and correction of non word spelling errors in Hindi language]](https://ieeexplore.ieee.org/abstract/document/6954235)||
|HiWikiEd dataset|2020|[[Generating Inflectional Errors for Grammatical Error Correction in Hindi]](https://aclanthology.org/2020.aacl-srw.24/)|[[data]](https://github.com/s-ankur/hindi_grammar_correction)|

### Japanese

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|Character-level RNN-based seq2seq|2018|[[Automatic Error Correction on Japanese Functional Expressions Using Character-based Neural Machine Translation]](https://aclanthology.org/Y18-1046/)||
|Constructing retrieval system for Japanese GEC|2019|[[Grammatical-Error-Aware Incorrect Example Retrieval System for Learners of Japanese as a Second Language]](https://aclanthology.org/W19-4431.pdf)||
|TMU Evaluation Corpus for Japanese Learners|2020| [[Construction of an Evaluation Corpus for Grammatical Error Correction for Learners of Japanese as a Second Language]](https://aclanthology.org/2020.lrec-1.26/)| [[data: Fill this form]](https://docs.google.com/forms/d/e/1FAIpQLSdBOoRuHaDuBuwuuYHrz6ILR6LQqIPw3AUL6XVEmvDFg8z_wQ/viewform)|
|Non-Autoregressive approach|2020|[[Non-Autoregressive Grammatical Error Correction Toward a Writing Support System]](https://aclanthology.org/2020.nlptea-1.1/)||
||2022|[Construction of a Quality Estimation Dataset for Automatic Evaluation of Japanese Grammatical Error Correction](https://arxiv.org/abs/2201.08038)||

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

### Spanish

|Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|COWS-L2H|2020|[[Developing NLP Tools with a New Corpus of Learner Spanish]](https://aclanthology.org/2020.lrec-1.894/)|[[data]](https://github.com/ucdaviscl/cowsl2h)|

### Ukrainian

Keywords / Overview|Year|Paper|Note|
|:--|:--|:--|:--|
|UA-GEC|2021|[[UA-GEC: Grammatical Error Correction and Fluency Corpus for the Ukrainian Language]](https://arxiv.org/abs/2103.16997)|[[data]](https://github.com/grammarly/ua-gec)|
