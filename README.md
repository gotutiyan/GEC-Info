# GEC Information

Something information of grammatical error correction :)  
Information will be added sometimes.

It can also be viewed on [GitHub Pages](https://gotutiyan.github.io/GEC-Info/)

# OverView of this page

* [Shared Tasks](https://github.com/gotutiyan/GEC-Info#shared-tasks)
* [Datasets](https://github.com/gotutiyan/GEC-Info#datasets)
* [Performance Measures](https://github.com/gotutiyan/GEC-Info#performance-measures)
* [Model / Architectue](https://github.com/gotutiyan/GEC-Info#models--architectures)
* [Strategies](https://github.com/gotutiyan/GEC-Info#strategies)
* [Data Augmentation](https://github.com/gotutiyan/GEC-Info#data-augmentation)
* [Analyses / Findings](https://github.com/gotutiyan/GEC-Info#analyses--findings)
* [Other Tools](https://github.com/gotutiyan/GEC-Info#other-tools)
* [Surveys](https://github.com/gotutiyan/GEC-Info#surveys)
* [Applications](https://github.com/gotutiyan/GEC-Info#applications)
* [Other Materials](https://github.com/gotutiyan/GEC-Info#other-materials)
* [Grammatical Error Detection](https://github.com/gotutiyan/GEC-Info#grammatical-error-detection)
* [Other Languages](https://github.com/gotutiyan/GEC-Info#other-languages)


# Shared Tasks

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|HOO 2011|2011| [[paper]](https://aclanthology.org/W11-2838/)| [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2011)|
|HOO 2012|2012| [[paper]](https://aclanthology.org/W12-2006)| [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2012-shared-task-on-preposition-and-determiner-error-correction)|
|CoNLL-2013|2013| [[paper]](https://aclanthology.org/W13-3601/)| [[website]](https://www.comp.nus.edu.sg/~nlp/conll13st.html)|
|CoNLL-2014|2014| [[paper]](https://aclanthology.org/W14-1701/)| [[website]](https://www.comp.nus.edu.sg/~nlp/conll14st.html) [[system outputs]](https://www.comp.nus.edu.sg/~nlp/conll14st/official_submissions.tar.gz)|
|BEA-2019|2019| [[paper]](https://aclanthology.org/W19-4406/)| [[website]](https://www.cl.cam.ac.uk/research/nl/bea2019st/) [[system outpus]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/system_output.bea19.tar.gz)|


# Datasets

### For training

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|EFCamDat|2014| [[paper v1]](https://www.semanticscholar.org/paper/Automatic-Linguistic-Annotation-ofLarge-Scale-L2-Geertzen-Alexopoulou/3261659127bebca4d805e8592906b37ece8d0ca3) [[paper v2]](https://corpus.mml.cam.ac.uk/faq/EFCamDat-Intro_release2.pdf)| [[data v2]](https://philarion.mml.cam.ac.uk)|
|GitHub Typo Corpus| 2019|[[paper]](https://arxiv.org/abs/1911.12893)| [[data]](https://github.com/mhagiwara/github-typo-corpus)|
|W&I+LOCNESS on BEA2019 Shared Task| 2019|[[paper]](https://www.cl.cam.ac.uk/~hy260/WI-cefr.pdf)| [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/wi+locness_v2.1.bea19.tar.gz)
|FCE|2011| [[paper]](https://www.aclweb.org/anthology/P11-1019)| [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/fce_v2.1.bea19.tar.gz)|
|NUCLE|2013| [[paper]](https://www.aclweb.org/anthology/W13-1703)| [[data]](https://www.comp.nus.edu.sg/~nlp/corpora.html)|
|ICNALE|2013| [[paper]](http://www.lib.kobe-u.ac.jp/infolib/meta_pub/G0000003kernel_81006678)| [[data]](http://language.sakura.ne.jp/icnale/)|
|Lang-8|2011| [[paper]](https://aclanthology.org/I11-1017)| [[website]](https://sites.google.com/site/naistlang8corpora/) [[data: Fill this form]](https://docs.google.com/forms/d/17gZZsC_rnaACMXmPiab3kjqBEtRHPMz0UG9Dk-x_F0k/viewform?edit_requested=true)<br>Related tools are useful. See the [[Other Tools]](https://github.com/gotutiyan/GEC-Info#other-tool) for the details.|
|PIE-synthetic|2019| [[paper]](https://aclanthology.org/D19-1435)| [[generated synthetic data]](https://drive.google.com/open?id=1bl5reJ-XhPEfEaPjvO45M7w0yN-0XGOA)|

### For evaluation

|Name|Year|Paper|Note|
|:--|:--|:--|:--|
|KJ|2011| [[paper]](https://aclanthology.org/P11-1121/)| [[website]](https://www.gsk.or.jp/catalog/gsk2019-a/)|
|CLC-FCE|2011| [[paper]](https://aclanthology.org/P11-1019/)| [[download]](https://ilexir.co.uk/datasets/index.html)|
|CoNLL-2013|2013| [[paper]](https://aclanthology.org/W13-3601/)| [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll13st/release2.3.1.tar.gz)|
|CoNLL-2014|2014| [[paper]](https://aclanthology.org/W14-1701/)| [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll14st/conll14st-test-data.tar.gz)|
|10 additional annotations for the CoNLL14 |2015| [[paper]](https://aclanthology.org/P15-1068/)| [[direct download]](https://aclanthology.org/attachments/P15-1068.Datasets.zip)|
|8 additional annotations for the CoNLL14|2016| [[paper]](https://aclanthology.org/Q16-1013)| [[download]](https://github.com/keisks/reassess-gec)|
|JFLEG|2017| [[paper]](https://aclanthology.org/E17-2037/)| [[data]](https://github.com/keisks/jfleg)|
|GMEG-Data|2019| [[paper]](https://aclanthology.org/Q19-1032)| [[code]](https://github.com/grammarly/GMEG)|
|CWEB|2020| [[paper]](https://www.aclweb.org/anthology/2020.emnlp-main.680)| [[data]](https://github.com/SimonHFL/CWEB)|


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

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|Scoring by counting the errors|2016|[[There’s No Comparison: Reference-less Evaluation Metrics in Grammatical Error Correction]](https://aclanthology.org/D16-1228)|[[code]](https://github.com/cnap/grammaticality-metrics)|
|Fluency + grammaticality + meaning preservation| 2017| [[Reference-based Metrics can be Replaced with Reference-less Metrics in Evaluating Grammatical Error Correction Systems]](https://aclanthology.org/I17-2058)||
|USim| 2018| [[Reference-less Measure of Faithfulness for Grammatical Error Correction]](https://aclanthology.org/N18-2020/)| [[code]](https://github.com/borgr/USim)|
|SOME|2020| [[SOME: Reference-less Sub-Metrics Optimized for Manual Evaluations of Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.573)| [[code]](https://github.com/kokeman/SOME)|


# Models / Architectures

### Supervised

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|Phrase-based SMT| 2016| [[Phrase-based Machine Translation is State-of-the-Art for Automatic Grammatical Error Correction]](https://aclanthology.org/D16-1161/)| [[code]](https://github.com/grammatical/baselines-emnlp2016)|
|Word-level SMT enhanced NNJMs + char-based SMT|2017|[[Connecting the Dots: Towards Human-Level Grammatical Error Correction]](https://aclanthology.org/W17-5037)|[[code]](https://github.com/nusnlp/smtgec2017)|
|First NMT-based approach|2016|[[Grammatical error correction using neural machine translation]](https://aclanthology.org/N16-1042/)||
|SMEG|2017|[[Systematically Adapting Machine Translation for Grammatical Error Correction]](https://aclanthology.org/W17-5039)|[[code]](https://github.com/cnap/smt-for-gec)|
|CNN-based Encder-Decoder approach| 2018|[[A Multilayer Convolutional Encoder-Decoder Neural Network for Grammatical Error Correction]](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/17308/16137)||
|Hybrid SMT and NMT|2018|[[Near Human-Level Performance in Grammatical Error Correction with Hybrid Machine Translation]](https://aclanthology.org/N18-2046)||
|Copy-Augmented Architecture|2019|[[Improving Grammatical Error Correction via Pre-Training a Copy-Augmented Architecture with Unlabeled Data]](https://aclanthology.org/N19-1014)|[[code]](https://github.com/yuantiku/fairseq-gec)|
|Consider a few previous sentences|2019|[[Cross-Sentence Grammatical Error Correction]](https://aclanthology.org/P19-1042)|[[code]](https://github.com/nusnlp/crosentgec)|
|PIE|2019|[[Parallel Iterative Edit Models for Local Sequence Transduction]](https://aclanthology.org/D19-1435/)|[[code]](https://github.com/awasthiabhijeet/PIE)|
|LaserTagger|2019|[[Encode, Tag, Realize: High-Precision Text Editing]](https://arxiv.org/abs/1909.01187)|[[code]](https://github.com/google-research/lasertagger)|
|Use sentence-level error dectection| 2019|[[The AIP-Tohoku System at the BEA-2019 Shared Task]](https://aclanthology.org/W19-4418)|BEA-2019: AIP-Tohoku||
|Ensemble four CNN + eight Transformer|2019|[[The LAIX Systems in the BEA-2019 GEC Shared Task]](https://aclanthology.org/W19-4416)|BEA-2019: LAIX|
|Transformer seq2seq + BERT re-ranker|2019|[[TMU Transformer System Using BERT for Re-ranking at BEA 2019 Grammatical Error Correction on Restricted Track]](https://aclanthology.org/W19-4422)|BEA-2019: TMU|
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
|Shallow Aggressive Decoding|2021|[[Instantaneous Grammatical Error Correction with Shallow Aggressive Decoding]](https://aclanthology.org/2021.acl-long.462/)||
|GECToR large|2021|[[Improving Sequence Tagging for Grammatical Error Correction]](https://drive.google.com/file/d/17-qXILfafHR8Uv2Y9plcB9WVRdZLazzp/view)|[[code]](https://github.com/MaksTarnavskyi/gector-large)|
|T5-based|2021|[[A Simple Recipe for Multilingual Grammatical Error Correction]](https://arxiv.org/abs/2106.03830)|[[code]](https://github.com/google-research-datasets/clang8)|
|GAN-like sequence labeling|2021|[[Grammatical Error Correction as GAN-like Sequence Labeling]](https://aclanthology.org/2021.findings-acl.290/)||

### Unsupervised

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|5-gram LM based approach| 2018| [[Language Model Based Grammatical Error Correction without Annotated Training Data]](https://aclanthology.org/W18-0529/)| [[code]](https://github.com/chrisjbryant/lmgec-lite)|
|Use Finite State Transducers| 2019| [[Neural Grammatical Error Correction with Finite State Transducers]](https://aclanthology.org/N19-1406)||
|LM-Critic| 2021| [[LM-Critic: Language Models for Unsupervised Grammatical Error Correction]](https://arxiv.org/abs/2109.06822)| [[code]](https://github.com/michiyasunaga/LM-Critic)|


# Strategies

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|Neural reinforcement learning|2017|[[Grammatical Error Correction with Neural Reinforcement Learning]](https://aclanthology.org/I17-2062/)||
|Fluency boosting learning|2018|[[Reaching Human-level Performance in Automatic Grammatical Error Correction: An Empirical Study]](https://arxiv.org/abs/1807.01270)|[[code]](https://github.com/getao/human-performance-gec)|
|Some methods that can be adapted neural MT|2018|[[Approaching Neural Grammatical Error Correction as a Low-Resource Machine Translation Task]](https://aclanthology.org/N18-1055/)|[[code]](https://github.com/grammatical/neural-naacl2018)|
|Iterative decoding|2018|[[Weakly Supervised Grammatical Error Correction using Iterative Decoding]](https://arxiv.org/abs/1811.01710)||
|Combine systems automatically|2019|[[Learning to combine Grammatical Error Corrections]](https://aclanthology.org/W19-4414/)|[[code]](https://github.com/IBM/learning-to-combine-grammatical-error-corrections)|
|Pretrain by DAE + sequential transfer learning|2019|[[A Neural Grammatical Error Correction System Built On Better Pre-training and Sequential Transfer Learning]](https://aclanthology.org/W19-4423/)|[[code]](https://github.com/kakaobrain/helo_word)<br>BEA-2019: Kakao&Brain|
|Cross-lingual Transfer Learning|2020|[[Cross-lingual Transfer Learning for Grammatical Error Correction]](https://aclanthology.org/2020.coling-main.415)||
|Data Weighted Training Strategies|2020|[[Data Weighted Training Strategies for Grammatical Error Correction]](https://aclanthology.org/2020.tacl-1.41/)||
|Combine Transformer + CNN with FST + Re-ranking|2019|[[Neural and FST-based approaches to grammatical error correction]](https://aclanthology.org/W19-4424)|BEA-2019: CAMB-CLED|
|A Self-Refinement Strategy for Noise Reduction|2020|[[A Self-Refinement Strategy for Noise Reduction in Grammatical Error Correction]](https://aclanthology.org/2020.findings-emnlp.26/)||


# Data Augmentation

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|Back translation|2016|[[Improving Neural Machine Translation Models with Monolingual Data]](https://aclanthology.org/P16-1009/)||
|Diverse back translation with noisy beam search|2018|[[Noising and Denoising Natural Language: Diverse Backtranslation for Grammar Correction]](https://aclanthology.org/N18-1057/)||
|DirectNoise| 2019|[[Improving Grammatical Error Correction via Pre-Training a Copy-Augmented Architecture with Unlabeled Data]](https://aclanthology.org/N19-1014/)|The method was first called "DirectNoise" by [[kiyono+ 2019]](https://aclanthology.org/D19-1119/)?|
|An emprical study of incorporating pseudo data|2019|[[An Empirical Study of Incorporating Pseudo Data into Grammatical Error Correction]](https://aclanthology.org/D19-1119/)|[[code]](https://github.com/butsugiri/gec-pseudodata)|
|Substituting words using confusion sets|2019|[[Neural Grammatical Error Correction Systems with Unsupervised Pre-training on Synthetic Data]](https://aclanthology.org/W19-4427)|[[synthetic data]](https://github.com/grammatical/pretraining-bea2019/issues/6)<br>BEA-2019: UEDIN-MS|
|Error+Context Dictionary + CNN EncDEc|2019|[[Improving Precision of Grammatical Error Correction with a Cheat Sheet]](https://aclanthology.org/W19-4425)|BEA-2019: 	Buffalo|
|Inverted Spellchecker + Patterns+POS|2019|[[A Comparative Study of Synthetic Data Generation Methods for Grammatical Error Correction]](https://aclanthology.org/2020.bea-1.21)||
|Methods for erroneous data generation|2019|[[Erroneous data generation for Grammatical Error Correction]](https://aclanthology.org/W19-4415)|BEA-2019: Shuyao|
|Wikipedia revision & Wikipedia round-trip translation|2019|[[Corpora Generation for Grammatical Error Correction]](https://aclanthology.org/N19-1333)||
|Use machine translation pairs|2020|[[Improving Grammatical Error Correction with Machine Translation Pairs]](https://aclanthology.org/2020.findings-emnlp.30/)||
|Edit latent representation|2020|[[Improving Grammatical Error Correction with Data Augmentation by Editing Latent Representation]](https://aclanthology.org/2020.coling-main.200/)||
|Consider learner’s error tendency|2020|[[Grammatical Error Correction Using Pseudo Learner Corpus Considering Learner’s Error Tendency]](https://aclanthology.org/2020.acl-srw.5/)||
|Tagged corruption|2021|[[Synthetic Data Generation for Grammatical Error Correction with Tagged Corruption Models]](https://aclanthology.org/2021.bea-1.4/)|[[code]](https://github.com/google-research-datasets/C4_200M-synthetic-dataset-for-grammatical-error-correction)|

### Data Cleaning

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|cLang8 (Cleaned Lang-8)|2021| [[A Simple Recipe for Multilingual Grammatical Error Correction]](https://arxiv.org/abs/2106.03830)| [[code]](https://github.com/google-research-datasets/clang8)|


# Analyses / Findings

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|Re-rank the CoNLL14 systems by human evaluation|2015| [[Human Evaluation of Grammatical Error Correction Systems]](https://aclanthology.org/D15-1052/)| [[code]](https://github.com/grammatical/evaluation/)|
||2015| [[How Far are We from Fully Automatic High Quality Grammatical Error Correction?]](https://aclanthology.org/P15-1068)||
|Human annotation focused on fluency |2016| [[Reassessing the Goals of Grammatical Error Correction: Fluency Instead of Grammaticality]](https://aclanthology.org/Q16-1013)||
||2017| [[GEC into the future: Where are we going and how do we get there?]](https://aclanthology.org/W17-5019/)||
|MEAGE| 2018| [[Automatic Metric Validation for Grammatical Error Correction]](https://aclanthology.org/P18-1127)| [[code]](https://github.com/borgr/EoE)|
||2018| [[Inherent Biases in Reference-based Evaluation for Grammatical Error Correction]](https://aclanthology.org/P18-1059/)| [[code]](https://github.com/borgr/IBGEC)|
|Reassess M^2, I-measure, GLEU by comparing human evaluation|2018| [[A Reassessment of Reference-Based Grammatical Error Correction Metrics]](https://aclanthology.org/C18-1231) |[[code]](https://github.com/nusnlp/gecmetrics)|
|Evaluate four systems (SMT, CNN, LSTM, Transformer) for six corpora (CoNLL13&14, FCE, JFLEG, KJ, ICNALE)|2019| [[Cross-Corpora Evaluation and Analysis of Grammatical Error Correction Models — Is Single-Corpus Evaluation Enough?]](https://aclanthology.org/N19-1132/) ||
|Create new gold data by post-editing system outputs|2021| [[How Good (really) are Grammatical Error Correction Systems?]](https://aclanthology.org/2021.eacl-main.231/)||
|Explore whether models have grammatical knowledge with Known-setting and Unknown-setting|2021| [[Do Grammatical Error Correction Models Realize Grammatical Generalization?]](https://aclanthology.org/2021.findings-acl.399/)||
|Compare CNN, LSTM, transformer or combinations of them as BT models|2021| [[Comparison of Grammatical Error Correction Using Back-Translation Models]](https://aclanthology.org/2021.naacl-srw.16/)||


# Surveys

|Title|Year|Page|Note|
|:--|:--|:--|:--|
|"A Comprehensive Survey of Grammar Error Correction"|2020|[[paper]](https://arxiv.org/abs/2005.06600)||
|私のブックマーク 「自然言語処理による文法誤り訂正|2018|[[website]](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol33-no6/) [[pdf]](https://www.jstage.jst.go.jp/article/jjsai/33/6/33_893/_pdf/-char/ja)|Written in Japanese. 2011-2018ごろの文法誤り訂正の動向を追うのに有用．|


# Applications

|Name|Paper|Note|
|:--|:--|:--|
|GECko++| [[paper]](https://aclanthology.org/2021.jeptalnrecital-demo.3)|[[website]](https://gecko-app.azurewebsites.net) [[code]](https://github.com/psawa/gecko-app)<br>An English assiting tool. Correction grammatical error and re-ordering sentences automatically.|


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
|Chunngai/gec-papers ||[[github]](https://github.com/Chunngai/gec-papers/blob/master/README.md)<br>The papers are being compiled around 2019-2020?


# Grammatical Error Detection

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|| 2018| [[Wronging a Right: Generating Better Errors to Improve Grammatical Error Detection]](https://aclanthology.org/D18-1541/)| [[code]](https://github.com/skasewa/wronging)|
|Multi-head and multi-layer attention| 2019| [[Multi-Head Multi-Layer Attention to Deep Language Representations for Grammatical Error Detection]](https://arxiv.org/abs/1904.07334)||
||2021| [[Exploring the Capacity of a Large-scale Masked Language Model to Recognize Grammatical Errors]](https://arxiv.org/abs/2108.12216)|

# Other Languages

### Arabic

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|QALB 2014 Shared Task| 2014| [[The First QALB Shared Task on Automatic Text Correction for Arabic]](https://aclanthology.org/W14-3605/)| [[website]](http://nlp.qatar.cmu.edu/qalb/sharedtask/shared_task.html)|
|QALB 2015 Shared Task| 2015| [[The Second QALB Shared Task on Automatic Text Correction for Arabic]](https://aclanthology.org/W15-3204/)||
|Automatic Error Type Annotation for Arabic| 2021| [[Automatic Error Type Annotation for Arabic]](https://arxiv.org/abs/2109.08068)||

### Chinese

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|NLPCC-2018 Shared Task| 2018| [[Overview of the NLPCC 2018 Shared Task: Grammatical Error Correction]](http://tcci.ccf.org.cn/conference/2018/papers/EV11.pdf)| [[data]](https://github.com/zhaoyyoo/NLPCC2018_GEC)
|MaskGEC| 2020| [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/5476)||
|| 2020| [[Chinese Grammatical Error Detection Based on BERT Model]](https://aclanthology.org/2020.nlptea-1.15/)||
||2020| [[BERT Enhanced Neural Machine Translation and Sequence Tagging Model for Chinese Grammatical Error Diagnosis]](https://aclanthology.org/2020.nlptea-1.8/)||
|Tail-to-Tail Non-Autoregressive Sequence Prediction| 2021| [[Tail-to-Tail Non-Autoregressive Sequence Prediction for Chinese Grammatical Error Correction]](https://arxiv.org/abs/2106.01609)||

### Czech

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|AKCES-GEC dataset| 2019| [[Grammatical Error Correction in Low-Resource Scenarios]](https://aclanthology.org/D19-5545)| [[data]](https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-3057)|

### German

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|Falko-MERLIN GEC Corpus|2018| [[Using Wikipedia Edits in Low Resource Grammatical Error Correction]](https://aclanthology.org/W18-6111/)| [[data]](https://github.com/adrianeboyd/boyd-wnut2018/)|

### Japanese

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|TMU Evaluation Corpus for Japanese Learners|2020| [[Construction of an Evaluation Corpus for Grammatical Error Correction for Learners of Japanese as a Second Language]](https://aclanthology.org/2020.lrec-1.26/)| [[data: Fill this form]](https://docs.google.com/forms/d/e/1FAIpQLSdBOoRuHaDuBuwuuYHrz6ILR6LQqIPw3AUL6XVEmvDFg8z_wQ/viewform)|

### Russian

|KeyWords|Year|Paper|Note|
|:--|:--|:--|:--|
|RULEC-GEC dataset|2019| [[Grammar Error Correction in Morphologically Rich Languages: The Case of Russian]](https://aclanthology.org/Q19-1001/)| [[data]](https://github.com/arozovskaya/RULEC-GEC)|
|RU-Lang8 dataset|2021| [[New Dataset and Strong Baselines for the Grammatical Error Correction of Russian]](https://aclanthology.org/2021.findings-acl.359/)| [[data]](https://github.com/arozovskaya/RU-Lang8)|