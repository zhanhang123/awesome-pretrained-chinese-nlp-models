# Awesome Pretrained Chinese NLP Models[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

在自然语言处理领域中，预训练语言模型（Pretrained Language Models）已成为非常重要的基础技术，本仓库主要收集目前网上公开的一些高质量中文预训练模型(感谢分享资源的大佬)，并将持续更新......

**注**: 🤗[huggingface](https://github.com/huggingface/transformers)模型下载地址: 1. [清华大学开源镜像](https://mirror.tuna.tsinghua.edu.cn/hugging-face-models/) 2. [官方地址](https://huggingface.co/models)

# Expand Table of Contents

+ [NLU系列](#NLU系列)
  - [BERT](#BERT)
  - [RoBERTa](#RoBERTa)
  - [ALBERT](#ALBERT)
  - [NEZHA](#NEZHA)
  - [XLNET](#XLNET)
  - [MacBERT](#MacBERT)
  - [WoBERT](#WoBERT)
  - [ELECTRA](#ELECTRA)
  - [ZEN](#ZEN)
  - [ERNIE](#ERNIE)
  - [RoFormer](#RoFormer)
  - [StructBERT](#StructBERT)
  - [Lattice-BERT](#Lattice-BERT)
+ [NLG系列](#NLG系列)
  - [GPT](#GPT)
  - [NEZHA-GEN](#NEZHA-GEN)
  - [CPM-Generate](#CPM-Generate)
  - [T5](#T5)
  - [T5-PEGASUS](#T5-PEGASUS)
  - [盘古α](#PanGu-Alpha)
+ [NLU-NLG系列](#NLU-NLG系列)
  - [UniLM](#UniLM)
  - [Simbert](#Simbert)
  - [RoFormer-sim](#RoFormer-sim)
  - [CPM-2](#CPM-2)
+ [更新日志](#更新)

## NLU系列

### BERT

+ 2018 | BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding | Jacob Devlin, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1810.04805)
+ 2019 | Pre-Training with Whole Word Masking for Chinese BERT | Yiming Cui, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1906.08101)
+ 2021 | ChineseBERT: Chinese Pretraining Enhanced by Glyph and Pinyin Information | Zijun Sun, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/2106.16038.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| BERT-Base | base | [Google Drive](https://storage.googleapis.com/bert_models/2018_11_03/chinese_L-12_H-768_A-12.zip) | | [Google Research](https://github.com/google-research) | [github](https://github.com/google-research/bert)| 通用 |
| BERT-wwm | base | <p>[Google Drive](https://drive.google.com/open?id=1RoTQsXp2hkQ1gSRVylRIJfQxJUgkfJMW)<br>[讯飞云-07Xj](http://pan.iflytek.com/#/link/A2483AD206EF85FD91569B498A3C3879)</p> | [Google Drive](https://drive.google.com/open?id=1AQitrjbvCWc51SYiLN-cJq4e0WiNN4KY) | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| BERT-wwm-ext | base | <p>[Google Drive](https://drive.google.com/open?id=1buMLEjdtrXE2c4G1rpsNGWEx7lUQ0RHi)<br>[讯飞云-4cMG](http://pan.iflytek.com/#/link/653637473FFF242C3869D77026C9BDB5)</p> | [Google Drive](https://drive.google.com/open?id=1iNeYFhCBJWeUsIlnW_2K6SMwXkM4gLb_) | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| bert-base-民事  | base | [阿里云](https://thunlp.oss-cn-qingdao.aliyuncs.com/bert/ms.zip) | | [THUNLP](https://github.com/thunlp) | [github](https://github.com/thunlp/OpenCLaP) | 司法 |
| bert-base-刑事 | base| [阿里云](https://thunlp.oss-cn-qingdao.aliyuncs.com/bert/xs.zip) | | [THUNLP](https://github.com/thunlp) | [github](https://github.com/thunlp/OpenCLaP) | 司法 |
| BAAI-JDAI-BERT |base | [京东云](https://jdai009.s3.cn-north-1.jdcloud-oss.com/jd-aig/open/models/nlp_baai/20190918/JDAI-BERT.tar.gz?AWSAccessKeyId=86FD402DD0CB693D629F6E62DC11E0E6&Expires=1634304356&Signature=dfnLvSzXeerRPSnMsZXSoEwdmkw%3D) | | [JDAI](https://github.com/jd-aig)  | [github](https://github.com/jd-aig/nlp_baai/tree/master/pretrained_models_and_embeddings) | 电商客服对话 |
| FinBERT | base | <p>[Google Drive](https://drive.google.com/file/d/193B4sT63mMeh4zfge0FJbbFY447KiJXp/view?usp=sharing)<br>[百度网盘-1cmp](https://pan.baidu.com/share/init?surl=D-pVJyW6bbJSre5RxotJkA)</p> | <p>[Google Drive](https://drive.google.com/file/d/1qW1YWtw3q9Q28QThrIY-rDU9Gl-SLIKO/view?usp=sharing)<br>[百度网盘-986f](https://pan.baidu.com/share/init?surl=y_O586GBmZZ7g4d2nOF0Vg)</p> | [Value Simplex](https://github.com/valuesimplex) | [github](https://github.com/valuesimplex/FinBERT) | 金融科技领域 |
| EduBERT |base | [好未来AI](https://ai.100tal.com/download/TAL-EduBERT-TF.zip)  | [好未来AI](https://ai.100tal.com/download/TAL-EduBERT.zip) | [tal-tech](https://github.com/tal-tech) | [github](https://github.com/tal-tech/edu-bert) | 教育领域 |
| MC-BERT | base | [Google Drive](https://drive.google.com/open?id=1ccXRvaeox5XCNP_aSk_ttLBY695Erlok) |  | [Alibaba AI Research](https://github.com/alibaba-research)  | [github](https://github.com/alibaba-research/ChineseBLUE) | 医学领域 |
| guwenbert-base  |base | |<p>[百度网盘-4jng](https://pan.baidu.com/s/1dw_08p7CVsz0jVj4jd58lQ)<br>[huggingface](https://huggingface.co/ethanyt/guwenbert-base)</p> | [Ethan](https://github.com/Ethan-yt) | [github](https://github.com/Ethan-yt/guwenbert)  | 古文领域 |
| guwenbert-large |large | | <p>[百度网盘-m5sz](https://pan.baidu.com/s/1TL9mBIlIv2rSvp61xCkeJQ)<br>[huggingface](https://huggingface.co/ethanyt/guwenbert-large)</p> | [Ethan](https://github.com/Ethan-yt) | [github](https://github.com/Ethan-yt/guwenbert) | 古文领域  |
| ChineseBERT |base | | [huggingface](https://huggingface.co/ShannonAI/ChineseBERT-base) | [ShannonAI](https://github.com/ShannonAI) | [github](https://github.com/ShannonAI/ChineseBert) | 通用  |
|ChineseBERT |large | | [huggingface](https://huggingface.co/ShannonAI/ChineseBERT-large) | [ShannonAI](https://github.com/ShannonAI) | [github](https://github.com/ShannonAI/ChineseBert) | 通用  |
| BERT-CCPoem | small | | [thunlp](https://thunlp.oss-cn-qingdao.aliyuncs.com/BERT_CCPoem_v1.zip) | [THUNLP-AIPoet](https://github.com/THUNLP-AIPoet) | [github](https://github.com/THUNLP-AIPoet/BERT-CCPoem) | 古典诗歌  |

备注: 

> wwm全称为**Whole Word Masking **,一个完整的词的部分WordPiece子词被mask，则同属该词的其他部分也会被mask

> ext表示在更多数据集下训练

### RoBERTa

+ 2019 | RoBERTa: A Robustly Optimized BERT Pretraining Approach | Yinhan Liu, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/1907.11692.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| RoBERTa-tiny-clue  | tiny  |[Google Drive](https://storage.googleapis.com/cluebenchmark/pretrained_models/RoBERTa-tiny-clue.zip) | [百度网盘-8qvb](https://pan.baidu.com/share/init?surl=hoR01GbhcmnDhZxVodeO4w) | [CLUE](https://github.com/CLUEbenchmark)    | [github](https://github.com/CLUEbenchmark/CLUEPretrainedModels) | 通用 |
| RoBERTa-tiny-pair | tiny |  [google drive](https://storage.googleapis.com/cluebenchmark/pretrained_models/RoBERTa-tiny-pair.zip) | [百度网盘-8qvb](https://pan.baidu.com/share/init?surl=hoR01GbhcmnDhZxVodeO4w) | [CLUE](https://github.com/CLUEbenchmark)  | [github](https://github.com/CLUEbenchmark/CLUEPretrainedModels) | 通用 |
| RoBERTa-tiny3L768-clue | tiny  |  [Google Drive](https://storage.googleapis.com/cluebenchmark/pretrained_models/RoBERTa-tiny3L768-clue.zip) |  | [CLUE](https://github.com/CLUEbenchmark) | [github](https://github.com/CLUEbenchmark/CLUEPretrainedModels) | 通用 |
| RoBERTa-tiny3L312-clue | tiny  |  [google drive](https://storage.googleapis.com/cluebenchmark/pretrained_models/RoBERTa-tiny3L312-clue.zip) | [百度网盘-8qvb](https://pan.baidu.com/share/init?surl=hoR01GbhcmnDhZxVodeO4w) | [CLUE](https://github.com/CLUEbenchmark) | [github](https://github.com/CLUEbenchmark/CLUEPretrainedModels) | 通用 |
| RoBERTa-large-pair | large |  [Google Drive](https://storage.googleapis.com/cluebenchmark/pretrained_models/RoBERTa-large-pair.zip) | [百度网盘-8qvb](https://pan.baidu.com/share/init?surl=hoR01GbhcmnDhZxVodeO4w) | [CLUE](https://github.com/CLUEbenchmark)    | [github](https://github.com/CLUEbenchmark/CLUEPretrainedModels) | 通用 |
| RoBERTa-large-clue | large  |  [google drive](https://storage.googleapis.com/cluebenchmark/pretrained_models/RoBERTa-large-clue.zip) | [百度网盘-8qvb](https://pan.baidu.com/share/init?surl=hoR01GbhcmnDhZxVodeO4w) | [CLUE](https://github.com/CLUEbenchmark)    | [github](https://github.com/CLUEbenchmark/CLUEPretrainedModels) | 通用 |
| RBT3 | 3层base|  <p>[Google Drive](https://drive.google.com/file/d/1-rvV0nBDvRCASbRz8M9Decc3_8Aw-2yi/view?usp=drive_open)<br>[讯飞云-b9nx](https://pan.iflytek.com/link/275E5B46185C982D4AF5AC295E1651B6)</p> | [Google Drive](https://drive.google.com/file/d/1_LqmIxm8Nz1Abvlqb8QFZaxYo-TInOed/view) | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| RBTL3 | 3层large|  <p>[Google Drive](https://drive.google.com/open?id=1Jzn1hYwmv0kXkfTeIvNT61Rn1IbRc-o8)<br>[讯飞云-vySW](https://pan.iflytek.com/link/0DD18FAC080BAF75DBA28FB5C0047760)</p> | [Google Drive](https://drive.google.com/open?id=1eHM3l4fMo6DsQYGmey7UZGiTmQquHw25) | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| RBTL4 | 4层large | [讯飞云-e8dN](http://pan.iflytek.com/link/7B04C5BF09812DB241BBA973D649824C) |  | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| RBTL6 | 6层large | [讯飞云-XNMA](http://pan.iflytek.com/link/B935B1F701A8FD352CAA74614126C4A2) |  | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| RoBERTa-wwm-ext  |base |  <p>[Google Drive](https://drive.google.com/open?id=1jMAKIJmPn7kADgD3yQZhpsqM-IRM1qZt)<br>[讯飞云-Xe1p](http://pan.iflytek.com/#/link/98D11FAAF0F0DBCB094EE19CCDBC98BF)</p> | [Google Drive](https://drive.google.com/open?id=1eHM3l4fMo6DsQYGmey7UZGiTmQquHw25) | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| RoBERTa-wwm-ext-large  | large | <p>[Google Drive](https://drive.google.com/open?id=1dtad0FFzG11CBsawu8hvwwzU2R0FDI94)<br>[讯飞云-u6gC](http://pan.iflytek.com/#/link/AC056611607108F33A744A0F56D0F6BE)</p> | [Google Drive](https://drive.google.com/open?id=1-2vEZfIFCdM1-vJ3GD6DlSyKT4eVXMKq) | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-BERT-wwm) | 通用 |
| RoBERTa-base | base |  <p>[Google Drive](https://drive.google.com/open?id=1ykENKV7dIFAqRRQbZIh0mSb7Vjc2MeFA)<br>[百度网盘](https://pan.baidu.com/s/1hAs7-VSn5HZWxBHQMHKkrg)</p> | <p>[Google Drive](https://drive.google.com/open?id=1H6f4tYlGXgug1DdhYzQVBuwIGAkAflwB)<br>[百度网盘](https://pan.baidu.com/s/1AGC76N7pZOzWuo8ua1AZfw)</p> | [brightmart](https://github.com/brightmart) | [github](https://github.com/brightmart/roberta_zh) | 通用 |
| RoBERTa-Large | large |  <p>[Google Drive](https://drive.google.com/open?id=1W3WgPJWGVKlU9wpUYsdZuurAIFKvrl_Y)<br>[百度网盘](https://pan.baidu.com/s/1Rk_QWqd7-wBTwycr91bmug)</p> | [Google Drive](https://drive.google.com/open?id=1yK_P8VhWZtdgzaG0gJ3zUGOKWODitKXZ) | [brightmart](https://github.com/brightmart) | [github](https://github.com/brightmart/roberta_zh) | 通用 |
| RoBERTa-tiny | tiny |[huggingface](https://huggingface.co/uer) | [huggingface](https://huggingface.co/uer) | [DBIIR @ RUC](https://github.com/dbiir) | [UER](https://github.com/dbiir/UER-py) | 通用 |
| RoBERTa-mini | mini |[huggingface](https://huggingface.co/uer) | [huggingface](https://huggingface.co/uer) | [DBIIR @ RUC](https://github.com/dbiir) | [UER](https://github.com/dbiir/UER-py) | 通用 |
| RoBERTa-small | small |[huggingface](https://huggingface.co/uer) | [huggingface](https://huggingface.co/uer) | [DBIIR @ RUC](https://github.com/dbiir) | [UER](https://github.com/dbiir/UER-py) | 通用 |
| RoBERTa-medium | medium |[huggingface](https://huggingface.co/uer) | [huggingface](https://huggingface.co/uer) | [DBIIR @ RUC](https://github.com/dbiir) | [UER](https://github.com/dbiir/UER-py) | 通用 |
| RoBERTa-base | base |[huggingface](https://huggingface.co/uer) | [huggingface](https://huggingface.co/uer) | [DBIIR @ RUC](https://github.com/dbiir) | [UER](https://github.com/dbiir/UER-py) | 通用 |

### ALBERT

+ 2019 | ALBERT: A Lite BERT For Self-Supervised Learning Of Language Representations | Zhenzhong Lan, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/1909.11942.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| Albert_tiny  | tiny  |  [Google Drive](https://storage.googleapis.com/albert_zh/albert_tiny_489k.zip) | [Google Drive](https://drive.google.com/open?id=1VBsUJ7R5eWF1VcUBQY6BEn1a9miEvlBr) | [brightmart](https://github.com/brightmart) | [github](https://github.com/brightmart/albert_zh) | 通用  |
| Albert_base_zh  | base  |  [Google Drive](https://storage.googleapis.com/albert_zh/albert_base_zh_additional_36k_steps.zip) | [Google Drive](https://drive.google.com/open?id=1HeijHGubWR-ElFnfxUf8IrRx7Ghm1S_Q) | [brightmart](https://github.com/brightmart) | [github](https://github.com/brightmart/albert_zh) | 通用  |
| Albert_large_zh  | large |  [Google Drive](https://storage.googleapis.com/albert_zh/albert_large_zh.zip) | [Google Drive](https://drive.google.com/open?id=1TAuv7OiFN8qbkT6S_VbfVbhkhg2GUF3q) | [brightmart](https://github.com/brightmart)           | [github](https://github.com/brightmart/albert_zh) | 通用 |
| Albert_xlarge_zh | xlarge |  [Google Drive](https://storage.googleapis.com/albert_zh/albert_xlarge_zh_183k.zip) | [Google Drive](https://drive.google.com/open?id=1kMhogQRX0uGWIGdNhm7-3hsmHlrzY_gp) | [brightmart](https://github.com/brightmart)           | [github](https://github.com/brightmart/albert_zh) | 通用 |
| Albert_base  | base | [Google Drive](https://storage.googleapis.com/albert_models/albert_base_zh.tar.gz) | | [Google Research](https://github.com/google-research) | [github](https://github.com/google-research/ALBERT)  | 通用  |
| Albert_large  | large |  [Google Drive](https://storage.googleapis.com/albert_models/albert_large_zh.tar.gz) | | [Google Research](https://github.com/google-research) | [github](https://github.com/google-research/ALBERT)  | 通用 |
| Albert_xlarge | xlarge  |  [Google Drive](https://storage.googleapis.com/albert_models/albert_xlarge_zh.tar.gz) |  | [Google Research](https://github.com/google-research) | [github](https://github.com/google-research/ALBERT)  | 通用 |
| Albert_xxlarge | xxlarge |  [Google Drive](https://storage.googleapis.com/albert_models/albert_xxlarge_zh.tar.gz) |  | [Google Research](https://github.com/google-research) | [github](https://github.com/google-research/ALBERT)  | 通用  |

### NEZHA

+ 2019 | NEZHA: Neural Contextualized Representation for Chinese Language Understanding | Junqiu Wei, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1909.00204)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| NEZHA-base  | base | <p>[Google Drive](https://drive.google.com/drive/folders/1tFs-wMoXIY8zganI2hQgDBoDPqA8pSmh?usp=sharing)<br>[百度网盘-ntn3](https://pan.baidu.com/s/1UVQjy9v_Sv4cQd1ELdjqww)</p> | [lonePatient](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | [HUAWEI](https://github.com/huawei-noah)  | [github](https://github.com/huawei-noah/Pretrained-Language-Model) | 通用|
| NEZHA-base-wwm  |  base | <p>[Google Drive](https://drive.google.com/drive/folders/1bK6WbqAG-B6BX2d9RPprnh2MPK6zL0t_?usp=sharing)<br>[百度网盘-f68o](https://pan.baidu.com/s/1-YG8e5V2zKCnR3azsGZT1w)</p> | [lonePatient](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | [HUAWEI](https://github.com/huawei-noah) | [github](https://github.com/huawei-noah/Pretrained-Language-Model) | 通用 |
| NEZHA-large  |  large  |<p>[Google Drive](https://drive.google.com/drive/folders/1ZPPM5XtTTOrS_CDRak1t2nCBU-LFZ_zs?usp=sharing)<br>[百度网盘-7thu](https://pan.baidu.com/s/1R1Ew-Lu8oIP6QhWO6nqp5Q)</p> | [lonePatient](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | [HUAWEI](https://github.com/huawei-noah) | [github](https://github.com/huawei-noah/Pretrained-Language-Model) | 通用 |
| NEZHA-large-wwm | large  | <p>[Google Drive](https://drive.google.com/drive/folders/1LOAUc9LXyogC2gmP_q1ojqj41Ez01aga?usp=sharing)<br>[百度网盘-ni4o](https://pan.baidu.com/s/1JK1RLIJd2wpuypku3stt8w)</p> | [lonePatient](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | [HUAWEI](https://github.com/huawei-noah) | [github](https://github.com/huawei-noah/Pretrained-Language-Model) | 通用 |
| <p>WoNEZHA</br>(word-base)</p> | base |[百度网盘-qgkq](https://pan.baidu.com/s/1ABKwUuIiMEEsRXxxlbyKmw) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/WoBERT) | 通用 |

### MacBERT

+ 2020 | Revisiting Pre-Trained Models for Chinese Natural Language Processing | Yiming Cui, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/2004.13922.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| MacBERT-base  | base  | <p>[Google Drive](https://drive.google.com/file/d/1aV69OhYzIwj_hn-kO1RiBa-m8QAusQ5b/view?usp=sharing)<br>[讯飞云-E2cP](http://pan.iflytek.com/#/link/CF2A1F9AEBF859650E8956854A994C1B)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/MacBERT) | 通用 |
| MacBERT-large | large  | <p>[Google Drive](https://drive.google.com/file/d/1lWYxnk1EqTA2Q20_IShxBrCPc5VSDCkT/view?usp=sharing)<br>[讯飞云-3Yg3](http://pan.iflytek.com/#/link/805D743F3826EC4F4EB5C774D34432AE)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/MacBERT) | 通用 |


### WoBERT

+ 2020 | 提速不掉点：基于词颗粒度的中文WoBERT | 苏剑林. | spaces | [`Blog post`](https://kexue.fm/archives/7758)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| WoBERT | base |[百度网盘-kim2](https://pan.baidu.com/s/1BrdFSx9_n1q2uWBiQrpalw) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/WoBERT) | 通用 |
| WoBERT-plus | base |[百度网盘-aedw](https://pan.baidu.com/s/1Ltq3ltQsyBCj56zoOOvI9A) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/WoBERT) | 通用 |

### XLNET

+ 2019 | XLNet: Generalized Autoregressive Pretraining for Language Understanding | Zhilin Yang, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1906.08237)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| XLNet-base    | base |<p>[Google Drive](https://drive.google.com/open?id=1m9t-a4gKimbkP5rqGXXsEAEPhJSZ8tvx)<br>[讯飞云-uCpe](http://pan.iflytek.com/#/link/32619C31BDEFAF2D82CB8C7F66F01D5C)</p> | [Google Drive](https://drive.google.com/open?id=1mPDgcMfpqAf2wk9Nl8OaMj654pYrWXaR) | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-XLNet) | 通用     |
| XLNet-mid  | middle | <p>[Google Drive](https://drive.google.com/open?id=1342uBc7ZmQwV6Hm6eUIN_OnBSz1LcvfA)<br>[讯飞云-68En](http://pan.iflytek.com/#/link/ED7DF7ED04B871AFE8E4D97704B9134D)</p> | [Google Drive](https://drive.google.com/open?id=1u-UmsJGy5wkXgbNK4w9uRnC0RxHLXhxy) | [Yiming Cui](https://github.com/ymcui)      | [github](https://github.com/ymcui/Chinese-XLNet) | 通用 |
| XLNet_zh_Large |  large | [百度网盘](https://pan.baidu.com/s/1dy0Z27DoZdMpSmoz1Q4G5A)  |   | [brightmart](https://github.com/brightmart) | [github](https://github.com/brightmart/xlnet_zh) | 通用  |

### ELECTRA

+ 2020 | ELECTRA: Pre-training Text Encoders as Discriminators Rather Than Generators | Kevin Clark, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2003.10555)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| ELECTRA-180g-large    | large | <p>[Google Drive](https://drive.google.com/file/d/1P9yAuW0-HR7WvZ2r2weTnx3slo6f5u9q/view?usp=sharing)<br>[讯飞云-Yfcy](http://pan.iflytek.com/#/link/7605874F5A11CD693C60EAB79005CCF3)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 通用 |
| ELECTRA-180g-small-ex | small | <p>[Google Drive](https://drive.google.com/file/d/1NYJTKH1dWzrIBi86VSUK-Ml9Dsso_kuf/view?usp=sharing)<br>[讯飞云-GUdp](http://pan.iflytek.com/#/link/3EFCF909FC5CFEA6F0EA7AA774C64CF0)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 通用 |
| ELECTRA-180g-base  |  base | <p>[Google Drive](https://drive.google.com/file/d/1RlmfBgyEwKVBFagafYvJgyCGuj7cTHfh/view?usp=sharing)<br>[讯飞云-Xcvm](http://pan.iflytek.com/#/link/38E14C9BDBE8E93F09DFE2198E308489)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 通用 |
| ELECTRA-180g-small    | small  |  <p>[Google Drive](https://drive.google.com/file/d/177EVNTQpH2BRW-35-0LNLjV86MuDnEmu/view?usp=sharing)<br>[讯飞云-qsHj](http://pan.iflytek.com/#/link/D1B8FE678FA5BC31AA43BD99AD09913E)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 通用 |
| legal-ELECTRA-large   |  large  |  <p>[Google Drive](https://drive.google.com/file/d/1jPyVi_t4QmTkFy7PD-m-hG-lQ8cIETzD/view?usp=sharing)<br>[讯飞云-7f7b](http://pan.iflytek.com/#/link/CC111ED9B1D4AE7E26C69A520A6D8759)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 司法领域 |
| legal-ELECTRA-base    | base   | <p>[Google Drive](https://drive.google.com/file/d/12ZLaoFgpqGJxSi_9KiQV-jdVN4XRGMiD/view?usp=sharing)<br>[讯飞云-7f7b](http://pan.iflytek.com/#/link/CC111ED9B1D4AE7E26C69A520A6D8759)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 司法领域 |
| legal-ELECTRA-small   |  small   |  <p>[Google Drive](https://drive.google.com/file/d/1arQ5qNTNoc1OyMH8wBUKdTMy2QponIFY/view?usp=sharing)<br>[讯飞云-7f7b](http://pan.iflytek.com/#/link/CC111ED9B1D4AE7E26C69A520A6D8759)</p> |         | [Yiming Cui](https://github.com/ymcui) | [github](https://github.com/ymcui/Chinese-ELECTRA) | 司法领域 |
| ELECTRA-tiny  |  tiny   | <p>[Google Drive](https://drive.google.com/file/d/1UP4byt4-kgenwST0KvyMYNbln6FfaSLp/view?usp=sharing)<br>[百度网盘-rs99](https://pan.baidu.com/share/init?surl=4b-IiCkjRg-6XIYPXnezZA)</p> |         | [CLUE](https://github.com/CLUEbenchmark) | [github](https://github.com/CLUEbenchmark/ELECTRA) | 通用 |

### ZEN

+ 2019 | ZEN: Pre-training Chinese Text Encoder Enhanced by N-gram Representations | Shizhe Diao, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/1911.00720.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | 
| ZEN-Base |  base  |  | <p>[Google Drive](https://drive.google.com/open?id=1oxNdYMQOpFe3QlttH98bAqg_FQiiVeMr)<br>[百度网盘](https://pan.baidu.com/s/1E2ylFnzGSkwBc8tY_OqZYg)</p> | [Sinovation Ventures AI Institute](https://github.com/sinovation) | [github](https://github.com/sinovation/ZEN) | 通用 |

### ERNIE

+ 2019 | ERNIE: Enhanced Representation through Knowledge Integration | Yu Sun, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1904.09223)

+ 2020 | SKEP: Sentiment Knowledge Enhanced Pre-training for Sentiment Analysis | Hao Tian, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2005.05635)

+ 2020 | ERNIE-Gram: Pre-Training with Explicitly N-Gram Masked Language Modeling for Natural Language Understanding | Dongling Xiao, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2010.12148)

| 模型 | 版本 | PaddlePaddle | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| ernie-1.0-base  | base   |  [link](https://ernie-github.cdn.bcebos.com/model-ernie1.0.1.tar.gz) |  | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/ERNIE) | 通用  |
| ernie_1.0_skep_large | large | [link](https://senta.bj.bcebos.com/skep/ernie_1.0_skep_large_ch.tar.gz) |    | [Baidu](https://github.com/baidu) | [github](https://github.com/baidu/Senta)  | 情感分析 |
| ernie-gram | base | [link](https://ernie-github.cdn.bcebos.com/model-ernie-gram-zh.1.tar.gz) |    | [Baidu](https://github.com/baidu) | [github](https://github.com/PaddlePaddle/ERNIE/tree/develop/ernie-gram)  | 通用 |

备注: 

> PaddlePaddle转TensorFlow可参考: [tensorflow_ernie](https://github.com/ArthurRizar/tensorflow_ernie)

> PaddlePaddle转PyTorch可参考: [ERNIE-Pytorch](https://github.com/nghuyong/ERNIE-Pytorch)

### RoFormer

+ 2021 | RoFormer: Enhanced Transformer with Rotary Position Embedding | Jianlin Su, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2104.09864)

+ 2021 | Transformer升级之路：2、博采众长的旋转式位置编码 | 苏剑林. | spaces | [`Blog post`](https://kexue.fm/archives/8265)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| roformer  |  base(L12) | [百度网盘-xy9x](https://pan.baidu.com/s/1fiss862YsGCwf2HvU_Jm-g) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer) | 通用  |
| roformer  |  small(L6) | [百度网盘-gy97](https://pan.baidu.com/s/1iIXgZHHCgrYGXVRRSSCVPg) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer) | 通用  |
| roformer-char  |  base(L12) | [百度网盘-bt94](https://pan.baidu.com/s/1Q1pq8F4Fsl6bTipUAkqeDQ) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer) | 通用  |

### StructBERT

+ 2019 | StructBERT: Incorporating Language Structures into Pre-training for Deep Language Understanding | Wei Wang, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1908.04577)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| StructBERT  |  large(L24) | | [阿里云](https://alice-open.oss-cn-zhangjiakou.aliyuncs.com/StructBERT/ch_model) | [Alibaba](https://github.com/alibaba) | [github](https://github.com/alibaba/AliceMind/tree/main/StructBERT) | 通用  |

### Lattice-BERT

+ 2021 | Lattice-BERT: Leveraging Multi-Granularity Representations in Chinese Pre-trained Language Models | Yuxuan Lai, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/2104.07204.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| LatticeBERT  |  tiny(L4) | | [阿里云](https://alice-open.oss-cn-zhangjiakou.aliyuncs.com/LatticeBERT/chinese_labert-tiny-std-512.tar.gz) | [Alibaba](https://github.com/alibaba) | [github](https://github.com/alibaba/AliceMind/tree/main/LatticeBERT) | 通用  |
| LatticeBERT  |  small(L6) | | [阿里云](https://alice-open.oss-cn-zhangjiakou.aliyuncs.com/LatticeBERT/chinese_labert-lite-std-512.tar.gz) | [Alibaba](https://github.com/alibaba) | [github](https://github.com/alibaba/AliceMind/tree/main/LatticeBERT) | 通用  |
| LatticeBERT  |  base(L12) | | [阿里云](https://alice-open.oss-cn-zhangjiakou.aliyuncs.com/LatticeBERT/chinese_labert-base-std-512.tar.gz) | [Alibaba](https://github.com/alibaba) | [github](https://github.com/alibaba/AliceMind/tree/main/LatticeBERT) | 通用  |


## NLG系列

### GPT

+ 2019 | Improving Language Understandingby Generative Pre-Training | Alec Radford, et al. | arXiv | [`PDF`](https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf)

+ 2019 | Language Models are Unsupervised Multitask Learners | Alec Radford, et al. | arXiv | [`PDF`](https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| GPT2  | 30亿语料  |  | <p>[Google Drive](https://drive.google.com/file/d/1mT_qCQg4AWnAXTwKfsyyRWCRpgPrBJS3)<br>[百度网盘-ffz6](https://pan.baidu.com/s/1yiuTHXUr2DpyBqmFYLJH6A)</p> | [Caspar ZHANG](https://github.com/imcaspar) | [gpt2-ml](https://github.com/imcaspar/gpt2-ml) | 通用 |
| GPT2 | 15亿语料  |  | <p>[Google Drive](https://drive.google.com/file/d/1IzWpQ6I2IgfV7CldZvFJnZ9byNDZdO4n)<br>[百度网盘-q9vr](https://pan.baidu.com/s/1TA_3e-u2bXg_hcx_NwVbGw)</p> | [Caspar ZHANG](https://github.com/imcaspar)  | [gpt2-ml](https://github.com/imcaspar/gpt2-ml)  |  通用 |
| CDial-GPTLCCC-base  | base |  | [huggingface](https://huggingface.co/thu-coai/CDial-GPT_LCCC-base) | [thu-coai](https://github.com/thu-coai)         | [CDial-GPT](https://github.com/thu-coai/CDial-GPT)       |  中文对话  |
| CDial-GPT2LCCC-base | base |  | [huggingface](https://huggingface.co/thu-coai/CDial-GPT2_LCCC-base) | [thu-coai](https://github.com/thu-coai)| [CDial-GPT](https://github.com/thu-coai/CDial-GPT)           |  中文对话 |
| CDial-GPTLCCC-large | large |  | [huggingface](https://huggingface.co/thu-coai/CDial-GPT_LCCC-large) | [thu-coai](https://github.com/thu-coai)         | [CDial-GPT](https://github.com/thu-coai/CDial-GPT)           | 中文对话 |
| GPT2-dialogue       |  base    |  | <p>[Google Drive](https://drive.google.com/drive/folders/1Ogz3eapvtvdY4VUcY9AEwMbNRivLKhri?usp=sharing)</br>[百度网盘-osi6](https://pan.baidu.com/s/1qDZ24VKLBU9GKARX9Ev65g)</p> | [yangjianxin1](https://github.com/yangjianxin1) | [GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat) |  闲聊对话 |
| GPT2-mmi  | base  |   | <p>[Google Drive](https://drive.google.com/drive/folders/1oWgKXP6VG_sT_2VMrm0xL4uOqfYwzgUP?usp=sharing)</br>[百度网盘-1j88](https://pan.baidu.com/s/1ubXGuEvY8KmwEjIVTJVLww)</p> | [yangjianxin1](https://github.com/yangjianxin1) | [GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat) |  闲聊对话 |
| GPT2-散文模型   | base |   | <p>[Google Drive](https://drive.google.com/drive/folders/1rJC4niJKMVwixUQkuL9k5teLRnEYTmUf?usp=sharing)</br>[百度网盘-fpyu](https://pan.baidu.com/s/1nbrW5iw34GRhoTin8uU2tQ)</p> | [Zeyao Du](https://github.com/Morizeyao)        | [GPT2-Chinese](https://github.com/Morizeyao/GPT2-Chinese)    |   散文 |
| GPT2-诗词模型 |  base  |    | <p>[Google Drive](https://drive.google.com/drive/folders/1Z6nF1nrgTkrZcRLHedQHXb4_M9I7yQPN?usp=sharing)</br>[百度网盘-7fev](https://pan.baidu.com/s/1Hy0OQ5xZcTLer9MQZW8o3g)</p> | [Zeyao Du](https://github.com/Morizeyao) | [GPT2-Chinese](https://github.com/Morizeyao/GPT2-Chinese)    |  诗词  |
| GPT2-对联模型  |  base   |  | <p>[Google Drive](https://drive.google.com/drive/folders/1ZnsvS7oHRVueNKj_SeEhiQt86aze3ojj?usp=sharing)</br>[百度网盘-i5n0](https://pan.baidu.com/s/1j9yVQwjlXZq58wOyXK4lcg)</p> | [Zeyao Du](https://github.com/Morizeyao)        | [GPT2-Chinese](https://github.com/Morizeyao/GPT2-Chinese)    | 对联 |
| roformer-gpt  |  base(L12) | [百度网盘-2nnn](https://pan.baidu.com/s/11YTnWLX0ThQr2P2yW0P7GA) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer) | 通用  |

### NEZHA-Gen

+ 2019 | NEZHA: Neural Contextualized Representation for Chinese Language Understanding | Junqiu Wei, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1909.00204)

+ 2019 | Improving Language Understandingby Generative Pre-Training | Alec Radford, et al. | arXiv | [`PDF`](https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| NEZHA-Gen  | base | <p>[Google Drive](https://drive.google.com/drive/folders/1i4f_8LhaVDNjnGlLXNJ0rNgBP0E4L6V0?usp=sharing)<br>[百度网盘-rb5m](https://pan.baidu.com/s/1Bgle8TpcxHyuUz_jAXOBWw)</p> |  | [HUAWEI](https://github.com/huawei-noah)     | [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-Gen-TensorFlow) | 通用  |
| NEZHA-Gen  | base  | <p>[Google Drive](https://drive.google.com/drive/folders/1B5-jxUlzhoKwFVMQ-nkqqbmJQgr1lRAp?usp=sharing)<br>[百度网盘-ytim](https://pan.baidu.com/s/1me6_BGYHbWFdTi80vRQ2Lg)</p> |  | [HUAWEI](https://github.com/huawei-noah)     | [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-Gen-TensorFlow) | 诗歌 |

### CPM-Generate

+ 2020 | CPM: A Large-scale Generative Chinese Pre-trained Language Model | Zhengyan Zhang, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2012.00413)

| 模型 | 版本 | 资源 | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| CPM |  26亿参数 | [项目首页](https://cpm.baai.ac.cn/) | [模型下载](https://cpm.baai.ac.cn/download.html) | [Tsinghua AI](https://github.com/TsinghuaAI) | [github](https://github.com/TsinghuaAI/CPM-Generate) | 通用  |

备注: 

> PyTorch转TensorFlow可参考: [CPM-LM-TF2](https://github.com/qhduan/CPM-LM-TF2)

> PyTorch转PaddlePaddle可参考: [CPM-Generate-Paddle](https://github.com/jm12138/CPM-Generate-Paddle)

### T5

+ 2019 | Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer | Colin Raffel, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1910.10683)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| T5 | small |[huggingface](https://huggingface.co/uer/t5-small-chinese-cluecorpussmall) | [huggingface](https://huggingface.co/uer/t5-small-chinese-cluecorpussmall) | [DBIIR @ RUC](https://github.com/dbiir) | [UER](https://github.com/dbiir/UER-py) | 通用 |


### T5-PEGASUS

+ 2019 | Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer | Colin Raffel, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1910.10683)

+ 2019 | PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization | Jingqing Zhang, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/1912.08777.pdf)

+ 2021 | T5 PEGASUS：开源一个中文生成式预训练模型 | 苏剑林. | spaces | [`Blog post`](https://spaces.ac.cn/archives/8209)

| 模型 | 版本 | Keras | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| T5 PEGASUS | base |[百度网盘-3sfn](https://pan.baidu.com/s/1lQ9Dt9wZDO3IgiCL9tP-Ug) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/t5-pegasus) | 通用 |
| T5 PEGASUS | small |[百度网盘-qguk](https://pan.baidu.com/s/1bXRVWnDyAck9VfSO9_1oJQ) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/t5-pegasus) | 通用 |

>  Keras转PyTorch可参考: [t5-pegasus-pytorch](https://github.com/renmada/t5-pegasus-pytorch)

### PanGu-Alpha

+ 2021 | PanGu-α: Large-scale Autoregressive Pretrained Chinese Language Models with Auto-parallel Computation | Wei Zeng, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2104.12369)

| 模型 | 版本 | 资源 | 下载地址 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| 盘古α-2.6B |  2.6G | [项目首页](https://git.openi.org.cn/PCL-Platform.Intelligence/PanGu-Alpha/src/branch/master) | [模型下载](https://git.openi.org.cn/PCL-Platform.Intelligence/PanGu-Alpha/src/branch/master) | [PCL-Platform.Intelligence](https://git.openi.org.cn/PCL-Platform.Intelligence) | [github](https://git.openi.org.cn/PCL-Platform.Intelligence/PanGu-Alpha) | 通用  |
| 盘古α-13B |  12G | [项目首页](https://git.openi.org.cn/PCL-Platform.Intelligence/PanGu-Alpha/src/branch/master) | [模型下载](https://git.openi.org.cn/PCL-Platform.Intelligence/PanGu-Alpha/src/branch/master) | [PCL-Platform.Intelligence](https://git.openi.org.cn/PCL-Platform.Intelligence) | [github](https://git.openi.org.cn/PCL-Platform.Intelligence/PanGu-Alpha) | 通用  |

## NLU-NLG系列

### UniLM

+ 2019 | Unified Language Model Pre-training for Natural Language Understanding and Generation | Li Dong, et al. | arXiv | [`PDF`](https://arxiv.org/abs/1905.03197)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| Unilm  |  base | [百度网盘-tblr](https://pan.baidu.com/s/1HgxIkBl5Yfwrzs1K1B6NFA) | [百度网盘-etwf](https://pan.baidu.com/s/1DHJGOFJ5cce5N5g4aBDiMQ) | [YunwenTechnology](https://github.com/YunwenTechnology) | [github](https://github.com/YunwenTechnology/Unilm) | 通用  |

### Simbert 

+ 2020 | 鱼与熊掌兼得：融合检索和生成的SimBERT模型 | 苏剑林. | spaces | [`Blog post`](https://kexue.fm/archives/7427)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| SimBERT Tiny  |  tiny | [百度网盘-1tp7](https://pan.baidu.com/s/1z_agqTuBTuyHANwrS-gPcg) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/pretrained-models) | 通用  |
| SimBERT Small  |  small | [百度网盘-nu67](https://pan.baidu.com/s/1kq_EQDI0gpiZBLFd_AxwrA) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/pretrained-models) | 通用  |
| SimBERT Base  |  base | [百度网盘-6xhq](https://pan.baidu.com/s/1uGfQmX1Kxcv_cXTVsvxTsQ) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/pretrained-models) | 通用  |

### RoFormer-sim

+ 2021 | SimBERTv2来了！融合检索和生成的RoFormer-Sim模型 | 苏剑林. | spaces | [`Blog post`](https://kexue.fm/archives/8454)

| 模型 | 版本 | TensorFlow | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| roformer-sim  |  base(L12) | [百度网盘-2cgz](https://pan.baidu.com/s/1f1FB288nv1a6jYjsNCordg) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer-sim) | 通用  |
| roformer-sim  |  small(L6) | [百度网盘-h68q](https://pan.baidu.com/s/1r0eJ7shGwQ0RzV9BTFFW4g) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer-sim) | 通用  |
| roformer-sim-v2  |  base(L12) | [百度网盘-w15n](https://pan.baidu.com/s/1Igh3tSvSu_ahDZmGaOlVoA) | | [ZhuiyiTechnology](https://github.com/ZhuiyiTechnology) | [github](https://github.com/ZhuiyiTechnology/roformer-sim) | 通用  |

### CPM-2

+ 2021 | CPM-2: Large-scale Cost-effective Pre-trained Language Models | Zhengyan Zhang, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2106.10715)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 | 备注 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |---- |
| CPM-2 |  110亿参数 | [项目首页](https://wudaoai.cn/home) | [模型下载](https://resource.wudaoai.cn/home?ind=2&name=WuDao%20WenYuan&id=1394901846484627456) | [BAAI-WuDao](https://github.com/BAAI-WuDao) | [github](https://github.com/BAAI-WuDao/Model) | 通用  | 需要申请才能下载 |
| CPM-2 |  100亿参数 | [项目首页](https://wudaoai.cn/home) | [模型下载](https://resource.wudaoai.cn/home?ind=2&name=WuDao%20WenYuan&id=1394901846484627456) | [BAAI-WuDao](https://github.com/BAAI-WuDao) | [github](https://github.com/BAAI-WuDao/Model) | 中英  | 需要申请才能下载 |
| CPM-2 |  1980亿参数 | [项目首页](https://wudaoai.cn/home) | [模型下载](https://resource.wudaoai.cn/home?ind=2&name=WuDao%20WenYuan&id=1394901846484627456) | [BAAI-WuDao](https://github.com/BAAI-WuDao) | [github](https://github.com/BAAI-WuDao/Model) | 中英  | 需要申请才能下载 |

## 更新

* 2021.08.16 增加CPM-2: Large-scale Cost-effective Pre-trained Language Models
* 2021.08.16 增加Lattice-BERT: Leveraging Multi-Granularity Representations in Chinese Pre-trained Language Models
* 2021.07.19 增加roformer-sim-v2：利用标注数据增强版本
* 2021.07.15 增加BERT-CCPoem：古典诗歌语料训练的BERT
* 2021.07.06 增加ChineseBERT：Chinese Pretraining Enhanced by Glyph and Pinyin Information
* 2021.06.22 增加StructBERT
* 2021.06.14 增加RoFormer：Enhanced Transformer with Rotary Position Embedding
* 2021.05.25 增加ERNIE-Gram
* 2021.04.28 增加PanGu-Alpha
* 2021.03.16 增加T5-PEGASUS
* 2021.03.09 增加UER系列模型
* 2021.03.04 增加WoBERT
