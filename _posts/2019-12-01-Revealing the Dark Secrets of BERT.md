---
layout: post
title:  "Revealing the Dark Secrets of BERT"
date:   2019-12-01 10:59:21 +0700
categories: NLP
---
# どんな論文？
BERTのself-attentionにたいして、調査を行った論文。attentionにかんして、タスクごとのパターン、言語的な特徴、タスク毎に重視するパターンの調査を行った。

# 新規性
attentionについて細かく見ている点。

# 結果
タスクによって、attentionパターンはちがう。しかし、多くのタスクでSEPが強くattentionされる。
何らかの言語的特徴をattentionは捉えている。
ある層のattentionを平準化したところ精度が上がるものがあるので、BERTはbaseの大きさで、overparametarize。
pre-trainなしだとGLUE精度がでない。