# GEC-Info

Something information of grammatical error correction :)

## Shared Task

* HOO 2011 [[paper]](https://aclanthology.org/W11-2838/) [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2011)

* HOO 2012 [[paper]](https://aclanthology.org/W12-2006) [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2012-shared-task-on-preposition-and-determiner-error-correction)

* CoNLL-2013 [[paper]](https://aclanthology.org/W13-3601/) [[website]](https://www.comp.nus.edu.sg/~nlp/conll13st.html)

* CoNLL-2014 [[paper]](https://aclanthology.org/W14-1701/) [[website]](https://www.comp.nus.edu.sg/~nlp/conll14st.html)

* BEA-2019 [[paper]](https://aclanthology.org/W19-4406/) [[website]](https://www.cl.cam.ac.uk/research/nl/bea2019st/)

## Dataset

#### For training

* GitHub Typo Corpus [[paper]](https://arxiv.org/abs/1911.12893) [[data]](https://github.com/mhagiwara/github-typo-corpus)

* W&I+LOCNESS on BEA2019 Shared Task [[paper]](https://www.cl.cam.ac.uk/~hy260/WI-cefr.pdf) [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/wi+locness_v2.1.bea19.tar.gz)

* FCE [[paper]](https://www.aclweb.org/anthology/P11-1019) [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/fce_v2.1.bea19.tar.gz)

* NUCLE [[paper]](https://www.aclweb.org/anthology/W13-1703) [[data]](https://www.comp.nus.edu.sg/~nlp/corpora.html)

* ICNALE [[paper]](http://www.lib.kobe-u.ac.jp/infolib/meta_pub/G0000003kernel_81006678) [[data]](http://language.sakura.ne.jp/icnale/)

* Lang-8 [[paper]](https://aclanthology.org/I11-1017) [[website]](https://sites.google.com/site/naistlang8corpora/) [[data: Fill this form]](https://docs.google.com/forms/d/17gZZsC_rnaACMXmPiab3kjqBEtRHPMz0UG9Dk-x_F0k/viewform?edit_requested=true)  
  Related tools are useful. See the [Tools](### Tools) for the details.

* PIE [[paper]](https://aclanthology.org/D19-1435) [[generated synthetic data]](https://drive.google.com/open?id=1bl5reJ-XhPEfEaPjvO45M7w0yN-0XGOA)

#### For evaluation

* KJ [[paper]](https://aclanthology.org/P11-1121/) [[website]](https://www.gsk.or.jp/catalog/gsk2019-a/)
* CLC-FCE [[paper]](https://aclanthology.org/P11-1019/) [[download]](https://ilexir.co.uk/datasets/index.html)
* CoNLL-2013 [[paper]](https://aclanthology.org/W13-3601/) [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll13st/release2.3.1.tar.gz)
* CoNLL-2014 [[paper]](https://aclanthology.org/W14-1701/)  [[direct download]](https://www.comp.nus.edu.sg/~nlp/conll14st/conll14st-test-data.tar.gz)
* 10 additional annotations for the CoNLL-2014 Shared Task [[paper]](https://aclanthology.org/P15-1068/) [[direct download]](https://aclanthology.org/attachments/P15-1068.Datasets.zip)
* 8 additional annotations for the CoNLL-2014 Shared Task [[paper]](https://aclanthology.org/Q16-1013) [[download]](https://github.com/keisks/reassess-gec)
* JFLEG [[paper]](https://aclanthology.org/E17-2037/) [[data]](https://github.com/keisks/jfleg)
* CWEB [[paper]](https://github.com/SimonHFL/CWEB/tree/master/data) [[data]]( https://github.com/SimonHFL/CWEB)

## Performance measure

#### Reference-based

* M^2 Scorer [[paper]](https://aclanthology.org/N12-1067/) [[code]](https://github.com/nusnlp/m2scorer)  
  It is often used to evaluate CoNLL-2013 and CoNLL-2014.

* GLEU [[paper]](https://aclanthology.org/P15-2097) [[code]](https://github.com/cnap/gec-ranking)  
  It is often used to evaluate JFLEG.

* I-measure [[paper]](https://aclanthology.org/N15-1060/) [[code]](https://github.com/mfelice/imeasure)  
  Code is available only python 2.x.

* ERRANT [[paper 1]](https://www.aclweb.org/anthology/C16-1079) [[paper 2]](https://www.aclweb.org/anthology/P17-1074) [[code]](https://github.com/chrisjbryant/errant)  
  It is often used to evaluate BEA-2019.

* GoToScorer [[paper]](https://www.aclweb.org/anthology/2020.coling-main.188) [[code]](https://github.com/gotutiyan/GTS)  
  It can be evaluated systems considering error correction difficulty.

#### Reference-less

* "There’s No Comparison: Reference-less Evaluation Metrics in Grammatical Error Correction" (2016) [[paper]](https://aclanthology.org/D16-1228)[[code]](https://github.com/cnap/grammaticality-metrics)

* Fluency + grammaticality +  meaning preservation (2017) [[paper]](https://aclanthology.org/I17-2058)

* USim (2018) [[paper]](https://aclanthology.org/N18-2020/) [[code]](https://github.com/borgr/USim)
* SOME (2020) [[paper]](https://aclanthology.org/2020.coling-main.573) [[code]](https://github.com/kokeman/SOME)

## Model / Architecture

#### Supervised

* Phrase-based SMT (2016) [[paper]](https://aclanthology.org/D16-1161/) [[code]](https://github.com/grammatical/baselines-emnlp2016)
* First NMT-based approach (2016) [[paper]](https://aclanthology.org/N16-1042/)
* CNN-based Encder-Decoder approach (2018) [[paper]](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/17308/16137)
* Copy-Augmented Architecture (2019) [[paper]](https://aclanthology.org/N19-1014) [[code]](https://github.com/yuantiku/fairseq-gec)
* PIE (2019) [[paper]](https://aclanthology.org/D19-1435/) [[code]](https://github.com/awasthiabhijeet/PIE)
* LaserTagger (2019) [[paper]](https://arxiv.org/abs/1909.01187) [[code]](https://github.com/google-research/lasertagger)
* GECToR (2020) [[paper]](https://aclanthology.org/2020.bea-1.16/) [[code]](https://github.com/grammarly/gector)
* BERT-fuse (2020) [[paper]](https://aclanthology.org/2020.acl-main.391/) [[code]](https://github.com/kanekomasahiro/bert-gec)
* Adversarial approach (2020) [[paper]](https://aclanthology.org/2020.findings-emnlp.275)
* Erroneous span correction and detection (2020) [[paper]](https://aclanthology.org/2020.emnlp-main.581/)
* Document-level approach (2020) [[paper]](https://aclanthology.org/2021.bea-1.8/) [[code]](https://github.com/chrisjbryant/doc-gec)
* Seq2Edits (2020) [[paper]](https://aclanthology.org/2020.emnlp-main.418/) 
* Beam search considering copy probability (2020) [[paper]](https://aclanthology.org/2020.coling-main.193)
* BART-based [[paper]](https://aclanthology.org/2020.aacl-main.83.pdf) [[code]](https://github.com/Katsumata420/generic-pretrained-GEC)
* Shallow Aggressive Decoding (2021) [[paper]](https://aclanthology.org/2021.acl-long.462/) 
* GECToR large (2021) [[paper]](https://drive.google.com/file/d/17-qXILfafHR8Uv2Y9plcB9WVRdZLazzp/view) [[code]](https://github.com/MaksTarnavskyi/gector-large)
* T5 based (2021)  [[paper]](https://arxiv.org/abs/2106.03830) [[code]](https://github.com/google-research-datasets/clang8)

#### Unsupervised

* LM-based approach (2018) [[paper]](https://aclanthology.org/W18-0529/) [[code]](https://github.com/chrisjbryant/lmgec-lite)

* LM-Critic (2021) [[paper]](https://arxiv.org/abs/2109.06822) [[code]](https://github.com/michiyasunaga/LM-Critic)

## Data Augmentation

* Back translation (2016) [[paper]](https://aclanthology.org/P16-1009/)

* Diverse back translation (2018) [[paper]](https://aclanthology.org/N18-1057/)

* DirectNoise (2019) [[paper]](https://aclanthology.org/N19-1014/)  
The method was first called "DirectNoise" by [[kiyono+ 2019]](https://aclanthology.org/D19-1119/) ?

* An emprical study of incorporating pseudo data (2019) [[paper]](https://aclanthology.org/D19-1119/) [[code]](https://github.com/butsugiri/gec-pseudodata)

* Substituting words using confusion sets (2019) [[paper]](https://aclanthology.org/W19-4427)

* Wikipedia revision & Wikipedia round-trip translation (2019) [[paper]](https://aclanthology.org/N19-1333)

* Using machine translation pairs (2020) [[paper]](https://aclanthology.org/2020.findings-emnlp.30/)

* Editing latent representation (2020) [[paper]](https://aclanthology.org/2020.coling-main.200/)

* Considering learner’s error tendency (2020) [[paper]](https://aclanthology.org/2020.acl-srw.5/)

* Tagged corruption model (2021) [[paper]](https://aclanthology.org/2021.bea-1.4/) [[code]](https://github.com/google-research-datasets/C4_200M-synthetic-dataset-for-grammatical-error-correction)

## Other Tool

* Lang8-NAIST-extractor [[code]](https://github.com/tomo-wb/Lang8-NAIST-extractor)  
The scripts for extracting error-correct pairs from the Lang-8 Corpus.

* cLang8 (Cleaned Lang-8)  [[paper]](https://arxiv.org/abs/2106.03830) [[code]](https://github.com/google-research-datasets/clang8)

* M2Converter [[code]](https://github.com/Jason3900/M2Convertor)  
The scripts for converting m2 file into source file and target file.

## Analysis / Finding

* "Human Evaluation of Grammatical Error Correction Systems" (2015) [[paper]](https://aclanthology.org/D15-1052/)
* "How Far are We from Fully Automatic High Quality Grammatical Error Correction?" (2015) [[paper]](https://aclanthology.org/P15-1068)
* "Cross-Corpora Evaluation and Analysis of Grammatical Error Correction Models — Is Single-Corpus Evaluation Enough?" (2019) [[paper]](https://aclanthology.org/N19-1132/)  
* "How Good (really) are Grammatical Error Correction Systems?" (2021) [[paper]](https://aclanthology.org/2021.eacl-main.231/)
* "Do Grammatical Error Correction Models Realize Grammatical Generalization?" (2021) [[paper]](https://aclanthology.org/2021.findings-acl.399/)
* "Comparison of Grammatical Error Correction Using Back-Translation Models"  (2021) [[paper]](https://aclanthology.org/2021.naacl-srw.16/)

## Survey

* "A Comprehensive Survey of Grammar Error Correction" [Wang+ 2020] [[paper]](https://arxiv.org/abs/2005.06600)

* 私のブックマーク 「自然言語処理による文法誤り訂正」[[website]](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol33-no6/) [[pdf]](https://www.jstage.jst.go.jp/article/jjsai/33/6/33_893/_pdf/-char/ja)  
  Written in Japanese. 2018年までの文法誤り訂正の動向を追うのに有用．

## Application

* GECko++ [[website]](https://gecko-app.azurewebsites.net) [[paper]](https://aclanthology.org/2021.jeptalnrecital-demo.3) [[code]](https://github.com/psawa/gecko-app)  
  An English assiting tool. Correction grammatical error and re-ordering sentences automatically.

## Other material

* NLP-progress [[website]](http://nlpprogress.com/english/grammatical_error_correction.html)  
  The performance ranking on some datasets.
* A Crash Course in Automatic Grammatical Error Correction [[paper]](https://www.aclweb.org/anthology/2020.coling-tutorials.6/) [[materials]](https://github.com/grammatical/coling2020-tutorial)  
  The tutorial in COLING2020.
* Chunngai/gec-papers [[github]](https://github.com/Chunngai/gec-papers/blob/master/README.md)  
  The papers are being compiled around 2019-2020?

## Grammatical Error Detection

* "Wronging a Right: Generating Better Errors to Improve Grammatical Error Detection" (2018) [[paper]](https://aclanthology.org/D18-1541/) [[code]](https://github.com/skasewa/wronging)

* Multi-head and multi-layer attention (2019) [[paper]](https://arxiv.org/abs/1904.07334)

* "Exploring the Capacity of a Large-scale Masked Language Model to Recognize Grammatical Errors" (2021) [[paper]](https://arxiv.org/abs/2108.12216) 
