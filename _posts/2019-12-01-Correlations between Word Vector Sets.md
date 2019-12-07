---
layout: post
title:  "Correlations between Word Vector Sets"
date:   2019-12-01 10:59:21 +0700
categories: NLP
---
# どんな論文？
文表現の変数を潜在空間の次元１つ１つに対してトークン数次元を持つデータのサンプリングとして捉えることで、計量に相関係数を導入した論文。poolingして文の表現を作成するアプローチとカーネルによる直接計算を行っている。

# 新規性
2pairのd次元統計と考え、poolingと計量の方法を比べた点とカーネルを使用しそのまま文を比較する方法を提案したこと。


# 結果
max-poolingとロバストな相関係数を使用することで、STSタスクの多くにおいてでのピアソン相関が向上。さらに、カーネルを使用する方法は、STSタスクの年代によっては、ピアソン相関が向上。

![Figure 1]({{ site.baseurl }}/assets/img/nlp/Correlations_between_Word_Vector_Sets/fig1.png)

![Figure 2]({{ site.baseurl }}/assets/img/nlp/Correlations_between_Word_Vector_Sets/fig2.png)



# 次に読むべき論文
- Arthur Gretton, Olivier Bousquet, Alex Smola, and Bernhard Sch¨olkopf. 2005a. Measuring statistical dependence with hilbert-schmidt norms. In Inter- national conference on algorithmic learning theory, pages 63–77. Springer.
- Arthur Gretton, Ralf Herbrich, Alexander Smola, Olivier Bousquet, and Bernhard Sch¨olkopf. 2005b. Kernel methods for measuring independence. Jour- nal of Machine Learning Research, 6(Dec):2075– 2129.