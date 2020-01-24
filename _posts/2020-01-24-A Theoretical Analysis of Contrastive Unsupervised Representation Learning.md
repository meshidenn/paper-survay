---
layout: post
title:  "A Theoretical Analysis of Contrastive Unsupervised Representation Learning"
date:   2020-01-24 10:59:21 +0700
categories: Theory
---
# どんな論文？
## 1. どんなもの？
同じグループの表現を近づけて、negative samplingにより異なるグループ表現を遠ざける教師なし学習が、教師あり学習の上界になっていることを示した論文。
さらに、この理論解析から、CURL(Contrastive Unsupervised Representation Learning)という、同じグループの平均を使う方法を提案し、精度が向上することを示した。

## 2. 先行研究と比べてどこがすごいの？
- 教師なしの表現学習が、分類タスクで精度を向上させてきた実験結果の理論保証になる


## 3. 技術や手法の"キモ"はどこにある？
- 理論保証
  - グループ一致時とグループ不一致時で功を分ける
     - グループ一致時が分散として取り出される

![(1)]({{ site.baseurl }}/assets/img/theory/A_Theoretical_Analysis_of_Contrastive_Unsupervised_Representation_Learning/formulation1.png)


- 同じグループと想定されるデータの表現をpositive samplingで平均化すること

## 4. どうやって有効だと検証した？
- 以下の実験結果

![tables]({{ site.baseurl }}/assets/img/theory/A_Theoretical_Analysis_of_Contrastive_Unsupervised_Representation_Learning/tables.png)
