# GEC-Info

Something information of grammatical error correction :)

## Shared Task

* HOO 2011 [[paper]](https://aclanthology.org/W11-2838/) [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2011)

* HOO 2012 [[paper]](https://aclanthology.org/W12-2006.pdf) [[website]](https://www.mq.edu.au/research/research-centres-groups-and-facilities/innovative-technologies/centres/centre-for-language-technology-clt/research/projects/hoo-helping-our-own/hoo-2012-shared-task-on-preposition-and-determiner-error-correction)

* CoNLL-2013 [[paper]](https://aclanthology.org/W13-3601/) [[website]](https://www.comp.nus.edu.sg/~nlp/conll13st.html)

* CoNLL-2014 [[paper]](https://aclanthology.org/W14-1701/) [[website]](https://www.comp.nus.edu.sg/~nlp/conll14st.html)

* BEA-2019 [[paper]](https://aclanthology.org/W19-4406/) [[website]](https://www.cl.cam.ac.uk/research/nl/bea2019st/)

## Models

* Copy-Augumented Architecture [[paper]](https://aclanthology.org/N19-1014.pdf) [[code]](https://github.com/yuantiku/fairseq-gec)

* PIE [[paper]](https://aclanthology.org/D19-1435/) [[code]](https://github.com/awasthiabhijeet/PIE)
* LaserTagger [[paper]](https://arxiv.org/abs/1909.01187) [[code]](https://github.com/google-research/lasertagger)

* GECToR [[paper]](https://aclanthology.org/2020.bea-1.16/) [[code]](https://github.com/grammarly/gector)
* BERT-fuse [[paper]](https://aclanthology.org/2020.acl-main.391/) [[code]](https://github.com/kanekomasahiro/bert-gec)

## Dataset

#### For training

* W&I + LOCNESS [[paper]](https://www.cl.cam.ac.uk/~hy260/WI-cefr.pdf) [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/wi+locness_v2.1.bea19.tar.gz)

* FCE [[paper]](https://www.aclweb.org/anthology/P11-1019) [[download]](https://www.cl.cam.ac.uk/research/nl/bea2019st/data/fce_v2.1.bea19.tar.gz)

* NUCLE [[paper]](https://www.aclweb.org/anthology/W13-1703) [[data]](https://www.comp.nus.edu.sg/~nlp/corpora.html)

* ICNALE [[paper]](http://www.lib.kobe-u.ac.jp/infolib/meta_pub/G0000003kernel_81006678) [[data]](http://language.sakura.ne.jp/icnale/)

* Lang-8 [[paper]](https://aclanthology.org/I11-1017.pdf) [[website]](https://sites.google.com/site/naistlang8corpora/) [[data: Fill this form]](https://docs.google.com/forms/d/17gZZsC_rnaACMXmPiab3kjqBEtRHPMz0UG9Dk-x_F0k/viewform?edit_requested=true)

  Related tools are useful. See the [Tools](### Tools) for the details.

* PIE [[paper]](https://aclanthology.org/D19-1435.pdf) [[generated synthetic data]](https://drive.google.com/open?id=1bl5reJ-XhPEfEaPjvO45M7w0yN-0XGOA)

#### For evaluation

* KJ (Not public) [[paper]](https://aclanthology.org/P11-1121/) [[website]](https://www.gsk.or.jp/catalog/gsk2019-a/)
* CLC-FCE [[paper]](https://aclanthology.org/P11-1019/) [[website]](https://ilexir.co.uk/datasets/index.html)
* CoNLL-2013 [[download]](https://www.comp.nus.edu.sg/~nlp/conll13st/release2.3.1.tar.gz)

* CoNLL-2014 [[download]](https://www.comp.nus.edu.sg/~nlp/conll14st/conll14st-test-data.tar.gz)

* 8 additional annotations for the CoNLL-2014 Shared Task [[paper]](https://aclanthology.org/P15-1068/) [[download]](https://aclanthology.org/attachments/P15-1068.Datasets.zip)

* JFLEG [[paper]](https://aclanthology.org/E17-2037/) [[data]](https://github.com/keisks/jfleg)

* CWEB [[paper]](https://github.com/SimonHFL/CWEB/tree/master/data) [[data]]( https://github.com/SimonHFL/CWEB)

## Evaluations

#### Reference-based

* M^2 Scorer [[paper]](https://aclanthology.org/N12-1067/) [[code]](https://github.com/nusnlp/m2scorer)

  It is often used to evaluate CoNLL-2013 and CoNLL-2014.

* GLEU [[paper]](https://aclanthology.org/P15-2097.pdf) [[code]](https://github.com/cnap/gec-ranking)

  It is often used to evaluate JFLEG.

* I-measure [[paper]](https://aclanthology.org/N15-1060/) [[code]](https://github.com/mfelice/imeasure)

  Code is available only python 2.x.

* ERRANT [[paper 1]](https://www.aclweb.org/anthology/C16-1079) [[paper 2]](https://www.aclweb.org/anthology/P17-1074) [[code]](https://github.com/chrisjbryant/errant)

  It is often used to evaluate BEA-2019.

* GoToScorer [[paper]](https://www.aclweb.org/anthology/2020.coling-main.188) [[code]](https://github.com/gotutiyan/GTS)

  It can be evaluated systems considering error correction difficulty.

#### Reference-less

* SOME [[paper]](https://aclanthology.org/2020.coling-main.573.pdf) [[code]](https://github.com/kokeman/SOME)

## Tools

* Lang8-NAIST-extractor [[code]](https://github.com/tomo-wb/Lang8-NAIST-extractor)

  The scripts for extracting error-correct pairs from the Lang-8 Corpus.

* cLang8 (Cleaned Lang-8)  [[paper]](https://arxiv.org/abs/2106.03830) [[code]](https://github.com/google-research-datasets/clang8)

* M2Converter [[code]](https://github.com/Jason3900/M2Convertor)

  The scripts for converting m2 file into source file and target file.

## Survey

* "A Comprehensive Survey of Grammar Error Correction" [Wang+ 2020] [[paper]](https://arxiv.org/abs/2005.06600)

* 私のブックマーク 「自然言語処理による文法誤り訂正」[[website]](https://www.ai-gakkai.or.jp/resource/my-bookmark/my-bookmark_vol33-no6/) [[pdf]](https://www.jstage.jst.go.jp/article/jjsai/33/6/33_893/_pdf/-char/ja)

  Written in Japanese. 2018年までの文法誤り訂正の動向を追うのに有用．

## Applications

* GECko++ [[website]](https://gecko-app.azurewebsites.net) [[paper]](https://aclanthology.org/2021.jeptalnrecital-demo.3.pdf) [[code]](https://github.com/psawa/gecko-app)

  An English assiting tool. Correction grammatical error and re-ordering sentences automatically.

## Other materials

* NLP-progress [[website]](http://nlpprogress.com/english/grammatical_error_correction.html)

  The performance ranking on some datasets.

* A Crash Course in Automatic Grammatical Error Correction [[paper]](https://www.aclweb.org/anthology/2020.coling-tutorials.6/) [[materials]](https://github.com/grammatical/coling2020-tutorial)

  The tutorial in COLING2020.