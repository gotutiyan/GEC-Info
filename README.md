# GEC-Info

Something information of grammatical error correction :)  
If the string in the `""` is the title of paper. Otherwise, it indicates method/dataset name or keywords.

## Shared Tasks
* HOO 2011 [[paper]](https://aclanthology.org/W11-2838/) [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2011)
* HOO 2012 [[paper]](https://aclanthology.org/W12-2006) [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2012-shared-task-on-preposition-and-determiner-error-correction)
* CoNLL-2013 [[paper]](https://aclanthology.org/W13-3601/) [[website]](https://www.comp.nus.edu.sg/~nlp/conll13st.html)
* CoNLL-2014 [[paper]](https://aclanthology.org/W14-1701/) [[website]](https://www.comp.nus.edu.sg/~nlp/conll14st.html)
* BEA-2019 [[paper]](https://aclanthology.org/W19-4406/) [[website]](https://www.cl.cam.ac.uk/research/nl/bea2019st/)

## Datasets

#### For training
* EFCamDat [[paper v1]](https://www.semanticscholar.org/paper/Automatic-Linguistic-Annotation-ofLarge-Scale-L2-Geertzen-Alexopoulou/3261659127bebca4d805e8592906b37ece8d0ca3) [[paper v2]](https://corpus.mml.cam.ac.uk/faq/EFCamDat-Intro_release2.pdf) [[data v2]](https://philarion.mml.cam.ac.uk)
* GitHub Typo Corpus [[paper]](https://arxiv.org/abs/1911.12893) [[data]](https://github.com/mhagiwara/github-typo-corpus)
* W&I+LOCNESS on BEA2019 Shared Task [[paper]](https://www.cl.cam.ac.uk/~hy260/WI-cefr.pdf) [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/wi+locness_v2.1.bea19.tar.gz)
* FCE [[paper]](https://www.aclweb.org/anthology/P11-1019) [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/fce_v2.1.bea19.tar.gz)
* NUCLE [[paper]](https://www.aclweb.org/anthology/W13-1703) [[data]](https://www.comp.nus.edu.sg/~nlp/corpora.html)
* ICNALE [[paper]](http://www.lib.kobe-u.ac.jp/infolib/meta_pub/G0000003kernel_81006678) [[data]](http://language.sakura.ne.jp/icnale/)
* Lang-8 [[paper]](https://aclanthology.org/I11-1017) [[website]](https://sites.google.com/site/naistlang8corpora/) [[data: Fill this form]](https://docs.google.com/forms/d/17gZZsC_rnaACMXmPiab3kjqBEtRHPMz0UG9Dk-x_F0k/viewform?edit_requested=true)  
  Related tools are useful. See the [[Other Tools]](https://github.com/gotutiyan/GEC-Info#other-tool) for the details.
* PIE-synthetic [[paper]](https://aclanthology.org/D19-1435) [[generated synthetic data]](https://drive.google.com/open?id=1bl5reJ-XhPEfEaPjvO45M7w0yN-0XGOA)

#### For evaluation
* KJ [[paper]](https://aclanthology.org/P11-1121/) [[website]](https://www.gsk.or.jp/catalog/gsk2019-a/)
* CLC-FCE [[paper]](https://aclanthology.org/P11-1019/) [[download]](https://ilexir.co.uk/datasets/index.html)
* CoNLL-2013 [[paper]](https://aclanthology.org/W13-3601/) [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll13st/release2.3.1.tar.gz)
* CoNLL-2014 [[paper]](https://aclanthology.org/W14-1701/)  [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll14st/conll14st-test-data.tar.gz)
* 10 additional annotations for the CoNLL-2014 Shared Task [[paper]](https://aclanthology.org/P15-1068/) [[direct download]](https://aclanthology.org/attachments/P15-1068.Datasets.zip)
* 8 additional annotations for the CoNLL-2014 Shared Task [[paper]](https://aclanthology.org/Q16-1013) [[download]](https://github.com/keisks/reassess-gec)
* JFLEG [[paper]](https://aclanthology.org/E17-2037/) [[data]](https://github.com/keisks/jfleg)
* GMEG-Data [[paper]](https://aclanthology.org/Q19-1032) [[code]](https://github.com/grammarly/GMEG)
* CWEB [[paper]](https://www.aclweb.org/anthology/2020.emnlp-main.680) [[data]](https://github.com/SimonHFL/CWEB)

## Performance measures

#### Reference-based
* M^2 Scorer [[paper]](https://aclanthology.org/N12-1067/) [[code]](https://github.com/nusnlp/m2scorer)  
  It is often used to evaluate CoNLL-2013 and CoNLL-2014.
* GLEU [[paper 1]](https://aclanthology.org/P15-2097) [[paper 2]](https://arxiv.org/abs/1605.02592) [[code]](https://github.com/cnap/gec-ranking)  
  It is often used to evaluate JFLEG.
* I-measure [[paper]](https://aclanthology.org/N15-1060/) [[code]](https://github.com/mfelice/imeasure)  
  Code is available only python 2.x.
* ERRANT [[paper 1]](https://www.aclweb.org/anthology/C16-1079) [[paper 2]](https://www.aclweb.org/anthology/P17-1074) [[code]](https://github.com/chrisjbryant/errant)  
  It is often used to evaluate BEA-2019.
* GMEG-Metric [[paper]](https://aclanthology.org/Q19-1032) [[code]](https://github.com/grammarly/GMEG)  
  Ridge regression using existing metrics (e.g. ERRANT, GLEU) as features.
* GoToScorer [[paper]](https://www.aclweb.org/anthology/2020.coling-main.188) [[code]](https://github.com/gotutiyan/GTS)  
  It can be evaluated systems considering error correction difficulty.

#### Reference-less
* "There’s No Comparison: Reference-less Evaluation Metrics in Grammatical Error Correction" (2016) [[paper]](https://aclanthology.org/D16-1228)[[code]](https://github.com/cnap/grammaticality-metrics)
* Fluency + grammaticality +  meaning preservation (2017) [[paper]](https://aclanthology.org/I17-2058)
* USim (2018) [[paper]](https://aclanthology.org/N18-2020/) [[code]](https://github.com/borgr/USim)
* SOME (2020) [[paper]](https://aclanthology.org/2020.coling-main.573) [[code]](https://github.com/kokeman/SOME)

## Models / Architectures

#### Supervised
* Phrase-based SMT (2016) [[paper]](https://aclanthology.org/D16-1161/) [[code]](https://github.com/grammatical/baselines-emnlp2016)
* First NMT-based approach (2016) [[paper]](https://aclanthology.org/N16-1042/)
* SMEG (2017) [[paper]](https://aclanthology.org/W17-5039) [[code]](https://github.com/cnap/smt-for-gec)
* CNN-based Encder-Decoder approach (2018) [[paper]](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/17308/16137)
* Copy-Augmented Architecture (2019) [[paper]](https://aclanthology.org/N19-1014) [[code]](https://github.com/yuantiku/fairseq-gec)
* Cross-sentence GEC [[paper]](https://aclanthology.org/P19-1042) [[code]](https://github.com/nusnlp/crosentgec)
* PIE (2019) [[paper]](https://aclanthology.org/D19-1435/) [[code]](https://github.com/awasthiabhijeet/PIE)
* LaserTagger (2019) [[paper]](https://arxiv.org/abs/1909.01187) [[code]](https://github.com/google-research/lasertagger)
* Using sentence-level error dectection (2019) (BEA-2019, AIP-Tohoku) [[paper]](https://aclanthology.org/W19-4418)
* Using Finite State Transducers (2019) [[paper]](https://aclanthology.org/N19-1406)
* GECToR (2020) [[paper]](https://aclanthology.org/2020.bea-1.16/) [[code]](https://github.com/grammarly/gector)
* BERT-fuse (2020) [[paper]](https://aclanthology.org/2020.acl-main.391/) [[code]](https://github.com/kanekomasahiro/bert-gec)
* Adversarial approach (2020) [[paper]](https://aclanthology.org/2020.findings-emnlp.275)
* Erroneous span correction and detection (2020) [[paper]](https://aclanthology.org/2020.emnlp-main.581/)
* Document-level approach (2020) [[paper]](https://aclanthology.org/2021.bea-1.8/) [[code]](https://github.com/chrisjbryant/doc-gec)
* Seq2Edits (2020) [[paper]](https://aclanthology.org/2020.emnlp-main.418/) 
* Beam search considering copy probability (2020) [[paper]](https://aclanthology.org/2020.coling-main.193)
* BART-based (2020) [[paper]](https://aclanthology.org/2020.aacl-main.83) [[code]](https://github.com/Katsumata420/generic-pretrained-GEC)
* VERNet (2021) [[paper]](https://aclanthology.org/2021.naacl-main.429) [[code]](https://github.com/thunlp/VERNet)
* Shallow Aggressive Decoding (2021) [[paper]](https://aclanthology.org/2021.acl-long.462/) 
* GECToR large (2021) [[paper]](https://drive.google.com/file/d/17-qXILfafHR8Uv2Y9plcB9WVRdZLazzp/view) [[code]](https://github.com/MaksTarnavskyi/gector-large)
* T5-based (2021)  [[paper]](https://arxiv.org/abs/2106.03830) [[code]](https://github.com/google-research-datasets/clang8)
* GAN-like sequence labeling (2021) [[paper]](https://aclanthology.org/2021.findings-acl.290/) 

#### Unsupervised
* LM-based approach (2018) [[paper]](https://aclanthology.org/W18-0529/) [[code]](https://github.com/chrisjbryant/lmgec-lite)
* Using Finite State Transducers (2019) [[paper]](https://aclanthology.org/N19-1406)
* LM-Critic (2021) [[paper]](https://arxiv.org/abs/2109.06822) [[code]](https://github.com/michiyasunaga/LM-Critic)

## Strategies
* Neural reinforcement learning (2017) [[paper]](https://aclanthology.org/I17-2062/) 
* Fluency boosting learning (2018) [[paper]](https://arxiv.org/abs/1807.01270)
* Some methods that can be adapted neural MT (2018) [[paper]](https://aclanthology.org/N18-1055/)
* Iterative decoding (2018) [[paper]](https://arxiv.org/abs/1811.01710)
* "Learning to combine Grammatical Error Corrections" (2019) [[paper]](https://aclanthology.org/W19-4414/)
* Pretrain by DAE + sequential transfer learning (2019) [[paper]](https://aclanthology.org/W19-4423/) [[code]](https://github.com/kakaobrain/helo_word)
* Cross-lingual Transfer Learning [[paper]](https://aclanthology.org/2020.coling-main.415)
* "Data Weighted Training Strategies for Grammatical Error Correction" (2020) [[paper]](https://aclanthology.org/2020.tacl-1.41/)
* "A Self-Refinement Strategy for Noise Reduction in Grammatical Error Correction" (2020) [[paper]](https://aclanthology.org/2020.findings-emnlp.26/)

## Data Augmentation
* Back translation (2016) [[paper]](https://aclanthology.org/P16-1009/)
* Diverse back translation with noisy beam search (2018) [[paper]](https://aclanthology.org/N18-1057/)
* DirectNoise (2019) [[paper]](https://aclanthology.org/N19-1014/)  
The method was first called "DirectNoise" by [[kiyono+ 2019]](https://aclanthology.org/D19-1119/) ?
* An emprical study of incorporating pseudo data (2019) [[paper]](https://aclanthology.org/D19-1119/) [[code]](https://github.com/butsugiri/gec-pseudodata)
* Substituting words using confusion sets. 1st in BEA-19 (2019) [[paper]](https://aclanthology.org/W19-4427) [[synthetic data]](https://github.com/grammatical/pretraining-bea2019/issues/6)
* Wikipedia revision & Wikipedia round-trip translation (2019) [[paper]](https://aclanthology.org/N19-1333)
* Using machine translation pairs (2020) [[paper]](https://aclanthology.org/2020.findings-emnlp.30/)
* Editing latent representation (2020) [[paper]](https://aclanthology.org/2020.coling-main.200/)
* Considering learner’s error tendency (2020) [[paper]](https://aclanthology.org/2020.acl-srw.5/)
* Tagged corruption model (2021) [[paper]](https://aclanthology.org/2021.bea-1.4/) [[code]](https://github.com/google-research-datasets/C4_200M-synthetic-dataset-for-grammatical-error-correction)

#### Data Cleaning
* cLang8 (Cleaned Lang-8)  [[paper]](https://arxiv.org/abs/2106.03830) [[code]](https://github.com/google-research-datasets/clang8)

## Other Tools
* Lang8-NAIST-extractor [[code]](https://github.com/tomo-wb/Lang8-NAIST-extractor)  
The scripts for extracting error-correct pairs from the Lang-8 Corpus.
* M2Converter [[code]](https://github.com/Jason3900/M2Convertor)  
The scripts for converting m2 file into source file and target file.
* EFCamDat-Preprocess [[code]](https://github.com/NTHU-NLPLAB/EFCamDat-Preprocess)

## Analyses / Findings
* "Human Evaluation of Grammatical Error Correction Systems" (2015) [[paper]](https://aclanthology.org/D15-1052/)
* "How Far are We from Fully Automatic High Quality Grammatical Error Correction?" (2015) [[paper]](https://aclanthology.org/P15-1068)
* "Reassessing the Goals of Grammatical Error Correction: Fluency Instead of Grammaticality" (2016) [[paper]](https://aclanthology.org/Q16-1013)
* "GEC into the future: Where are we going and how do we get there?" (2017) [[paper]](https://aclanthology.org/W17-5019/)
* MEAGE (2018) [[paper]](https://aclanthology.org/P18-1127) [[code]](https://github.com/borgr/EoE)
* "Inherent Biases in Reference-based Evaluation for Grammatical Error Correction" (2018) [[paper]](https://aclanthology.org/P18-1059/) [[code]](https://github.com/borgr/IBGEC)
* "Cross-Corpora Evaluation and Analysis of Grammatical Error Correction Models — Is Single-Corpus Evaluation Enough?" (2019) [[paper]](https://aclanthology.org/N19-1132/)  
* "How Good (really) are Grammatical Error Correction Systems?" (2021) [[paper]](https://aclanthology.org/2021.eacl-main.231/)
* "Do Grammatical Error Correction Models Realize Grammatical Generalization?" (2021) [[paper]](https://aclanthology.org/2021.findings-acl.399/)
* "Comparison of Grammatical Error Correction Using Back-Translation Models"  (2021) [[paper]](https://aclanthology.org/2021.naacl-srw.16/)

## Surveys
* "A Comprehensive Survey of Grammar Error Correction" [Wang+ 2020] [[paper]](https://arxiv.org/abs/2005.06600)
* 私のブックマーク 「自然言語処理による文法誤り訂正」[[website]](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol33-no6/) [[pdf]](https://www.jstage.jst.go.jp/article/jjsai/33/6/33_893/_pdf/-char/ja)  
  Written in Japanese. 2018年までの文法誤り訂正の動向を追うのに有用．

## Applications
* GECko++ [[website]](https://gecko-app.azurewebsites.net) [[paper]](https://aclanthology.org/2021.jeptalnrecital-demo.3) [[code]](https://github.com/psawa/gecko-app)  
  An English assiting tool. Correction grammatical error and re-ordering sentences automatically.

## Other materials
* NLP-progress [[website]](http://nlpprogress.com/english/grammatical_error_correction.html)  
  The performance ranking on some datasets.
* A Crash Course in Automatic Grammatical Error Correction [[paper]](https://www.aclweb.org/anthology/2020.coling-tutorials.6/) [[materials]](https://github.com/grammatical/coling2020-tutorial)  
  The tutorial about GEC in COLING2020.
* Chunngai/gec-papers [[github]](https://github.com/Chunngai/gec-papers/blob/master/README.md)  
  The papers are being compiled around 2019-2020?

## Grammatical Error Detection
* "Wronging a Right: Generating Better Errors to Improve Grammatical Error Detection" (2018) [[paper]](https://aclanthology.org/D18-1541/) [[code]](https://github.com/skasewa/wronging)
* Multi-head and multi-layer attention (2019) [[paper]](https://arxiv.org/abs/1904.07334)
* "Exploring the Capacity of a Large-scale Masked Language Model to Recognize Grammatical Errors" (2021) [[paper]](https://arxiv.org/abs/2108.12216) 

## Other Languages

### Chinese
* NLPCC-2018 Shared Task (2018) [[paper]](http://tcci.ccf.org.cn/conference/2018/papers/EV11.pdf) [[data]](https://github.com/zhaoyyoo/NLPCC2018_GEC)
* MaskGEC  (2020)[[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/5476)
* "Chinese Grammatical Error Detection Based on BERT Model" (2020) [[paper]](https://aclanthology.org/2020.nlptea-1.15/)
* Tail-to-Tail Non-Autoregressive Sequence Prediction (2021)[[paper]](https://arxiv.org/abs/2106.01609)

### Arabic
* QALB 2014 Shared Task (2014) [[paper]](https://aclanthology.org/W14-3605/) [[website]](http://nlp.qatar.cmu.edu/qalb/sharedtask/shared_task.html)
* QALB 2015 Shared Task (2015) [[paper]](https://aclanthology.org/W15-3204/)
* Automatic Error Type Annotation for Arabic (2021) [[paper]](https://arxiv.org/abs/2109.08068)