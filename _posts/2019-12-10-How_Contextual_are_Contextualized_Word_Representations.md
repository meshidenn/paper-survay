---
layout: post
title:  "How Contextual are Contextualized Word Representations? Comparing the Geometry of BERT, ELMo, and GPT-2 Embeddings"
date:   2019-12-10 10:59:21 +0700
categories: NLP
---
# どんな論文？
Contextulalized Word Vectorの性質を調べた論文。単語ベクトルが層を経る毎にどの程度移動しているか、文の平均とどの程度ずれているか、ランダムサンプルしたベクトル間のcos類似度がどうなっているか、どの程度一つのベクトルで説明可能かを調査している。

# 新規性
probing taskではなく、潜在空間の性質をそのまま調べている。


# 結果
1. contextualized word vectorの空間は異方性
2. 上の層のベクトルは、下の層のベクトルとあまり似ていない。上の層は、task-specificな特徴になっていると考えられる
3. １文中の各tokenに対するベクトル表現において、ELMOは、どの表現も同じになるようにcontextualizeされるが、BERTはだんだんと異なる表現になっており、GPT-2は、全く似ていない表現になっている。
4. contextulalized word vectorは一つの主成分では5%も説明できないので、有限の語の意味を表しているとはあまり考えられない。

![Figure 1]({{ site.baseurl }}/assets/img/nlp/How_Contextual_are_Contextualized_Word_Representations/fig1.png)

![Figure 2]({{ site.baseurl }}/assets/img/nlp/How_Contextual_are_Contextualized_Word_Representations/fig2.png)

![Figure 3]({{ site.baseurl }}/assets/img/nlp/How_Contextual_are_Contextualized_Word_Representations/fig3.png)

![Figure 4]({{ site.baseurl }}/assets/img/nlp/How_Contextual_are_Contextualized_Word_Representations/fig4.png)



# 次に読むべき論文
- David Mimno and Laure Thompson. 2017. The strange geometry of skip-gram with negative sampling. In Proceedings of the 2017 Conference on Empirical Methods in Natural Language Processing. pages 2873–2878