# STS_TF-IDF
このソースコードは,SemEval-2014のSemanticTextualSimilarityというタスクを想定して作成した物である。

## データセット
TfidfVectorizerの訓練データは、STS.input.OnWN.txt、STS.input.deft-forum.txt、STS.input.deft-news.txt、STS.input.headlines.txtの4つである。

## 特徴
- 文章の前処理として、SnowballStemmerを用いてステミングを実施
- sklearnのTfidfVectorizerを用いて計算したTf-IDFを素性として文ベクトルを生成
- 類似度の求め方はcos類似度で計算

## 精度
テストデータSTS.input.images.txtに対して0.71である。
