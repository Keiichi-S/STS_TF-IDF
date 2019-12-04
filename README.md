# STS_TF-IDF

このソースコードは,SemEval-2014のSemanticTextualSimilarityというタスクを想定して作成した物である。

文章の前処理としては、SnowballStemmerを施している。
文ベクトルは、sklearnのTfidfVectorizerを使用してTf-IDFを素性として作っている。
TfidfVectorizerの訓練データは、STS.input.OnWN.txt、STS.input.deft-forum.txt、STS.input.deft-news.txt、STS.input.headlines.txtの4つである。

類似度の求め方はcos類似度で求めている。

精度は、テストデータSTS.input.images.txtに対して0.71である。
