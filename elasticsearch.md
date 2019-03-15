Elasticsearchさらっとまとめ

# 目次
1. Elasticsearchとは
2. 特徴
3. 参考文献
4. おわりに

# 1. Elasticsearchとは
> Elasticsearchは、様々なユースケースを解決する分散型RESTful検索/分析エンジンです。予期した結果や、そうでないものも検索できるようにデータを集めて格納するElastic Stackのコア製品です。

[公式](https://www.elastic.co/jp/products/elasticsearch)より

ElasticsearchはElastic社が開発しているオープンソースの全文検索エンジンで、大量のドキュメントから目的の単語を含むドキュメントを高速に抽出することができる

# 2. 特徴
## RESTfulな検索
RDBではSQLを用いてデータを検索するが、ElasticsearchはRESTfulインターフェースを用いてデータを検索する

## スコアによる検索
Elasticsearchは完全一致による検索だけではなく、関連度の高さ（スコア）による検索も可能

## 高速
とにかく速い！

## マルチテナント
様々なサービスで自由に横断して検索・分析が可能で、一番よく使われるのは[Kibana](https://www.elastic.co/jp/products/kibana)

# 3. 参考文献
https://www.elastic.co/jp/products/elasticsearch
https://qiita.com/nskydiving/items/1c2dc4e0b9c98d164329
https://qiita.com/Mister_K/items/69433cd3c2ccefe48f4b#_reference-72850a29379955f0a9a5
https://qiita.com/r548/items/3622048a622d9c0acc05
https://qiita.com/rjkuro/items/95f71ad522226dc381c8

# 4. おわりに
さらっとまとめたけど、慣れるにはチュートリアルやるのが速い
