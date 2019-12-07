---
layout: default
title: About
permalink: /about/
avatar: true
navigation: true
---

## このページについて
このページは、[meshidenn](https://github.com/meshidenn/)が読んだ論文の簡易なまとめをメモするページです。
まとめのフォーマットは、落合先生フォーマットか、paperchallengeのフォーマットを使用します。

### 落合先生フォーマット
```
---
layout: post
title:  "論文タイトル"
date:   YYYY-MM-DD
categories: NLP Theory Graph Others
---

## 1. どんなもの？

## 2. 先行研究と比べてどこがすごいの？

## 3. 技術や手法の"キモ"はどこにある？

## 4. どうやって有効だと検証した？

## 5. 議論はあるか？

## 6. 次に読むべき論文はあるか？

### 論文情報・リンク

- [著者，"タイトル，" ジャーナル名，voluem，no.，ページ，年](論文リンク)
```

### pallerchallengeフォーマット
```
---
layout: post
title:  "論文タイトル"
date:   YYYY-MM-DD
categories: NLP Theory Graph Others
---

## 概要

## 新規性

## 結果

## 次に読むべき論文

### 論文情報・リンク

- [著者，"タイトル，" ジャーナル名，voluem，no.，ページ，年](論文リンク)
```


## このページの作成について
このページ({% include icon-github.html username="meshidenn" %}[paper-survey](https://github.com/meshidenn/paper-survey))は、[こちらのページ](https://github.com/shunk031/paper-survey)を参考に作成しました。

基本テンプレートは、以下を組み合わせています。
- {% include icon-github.html username="rmsubekti" %}[emping](https://github.com/rmsubekti/emping) 
- {% include icon-github.html username="pages-theme" %}[slate](https://github.com/pages-themes/slate)

基本フレームワークはJekyllです。
{% include icon-github.html username="jekyll" %} /
[jekyll](https://github.com/jekyll/jekyll)

---

### Site Last Generated : {{ site.time | date: "%-d %B %Y"  }}

Built with [Jekyll](http://jekyllrb.com/){:target="_blank"}.

Hosted on [Github Pages](https://pages.github.com/){:target="_blank"}.
