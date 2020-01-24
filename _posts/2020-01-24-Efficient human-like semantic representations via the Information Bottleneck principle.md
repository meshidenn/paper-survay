---
layout: post
title:  "Efficient human-like semantic representations via the Information Bottleneck principle"
date:   2020-01-24 10:59:21 +0700
categories: NLP
---
# どんな論文？
## 1. どんなもの？
色を信号として入力し、単語のような離散tokenとして出力するencoderとそれを受け取って、色信号を出力するデコーダーをinformation bottleneckを使って定式化し学習させた論文。これによって、人間の自然言語で表されている色の表現は、かなり最適値に近いことを示した。

## 2. 先行研究と比べてどこがすごいの？
- 人間の自然言語が、情報圧縮の点で、最適であることを示した。
- 逆に、このモデルで外界の入力信号をtokenとして離散化することができることを示した

![Figure 1]({{ site.baseurl }}/assets/img/nlp/Efficient_human-like_semantic_representations_via_the_Information_Bottleneck_principle/fig1.png)

## 3. 技術や手法の"キモ"はどこにある？
- information bottle neck

## 4. どうやって有効だと検証した？
- 以下の実験結果

![Figure 2]({{ site.baseurl }}/assets/img/nlp/Efficient_human-like_semantic_representations_via_the_Information_Bottleneck_principle/fig2.png)


## 5. 議論はあるか？

## 6. 次に読むべき論文はあるか？
- Amit M, Shmerler Y, Eisenberg E, Abraham M, Shnerb N (1994) Language and codificatio dependence of long-range correlations in texts.