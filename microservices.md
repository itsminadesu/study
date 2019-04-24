マイクロサービスさらっとまとめ

# 目次
1. マイクロサービスとは
2. マイクロサービスのメリット
3. マイクロサービスのデメリット
4. マイクロサービスフレームワーク
5. マイクロサービスの事例
6. 参考文献
7. おわりに

# 1. マイクロサービスとは
> マイクロサービス（英語：microservices）とは、ソフトウェア開発の技法の1つであり、1つのアプリケーションを、ビジネス機能に沿った複数の小さいサービスの疎に結合された集合体として構成するサービス指向アーキテクチャ（service-oriented architecture; SOA）の1種である。

(wikipediaより)

マイクロサービスは、個々に開発された複数の小さな（マイクロ）サービスを連携させて管理、運営をおこなっていくソフトウェアのアーキテクチャのこと。

![alt](https://cz-cdn.shoeisha.jp/static/images/article/11055/11055_003.png)

例えばオンラインショッピング全体が一つの大きなサービスとした時、
```
認証サービス   IDやパスワード
ロジック      データのフィルタリングサービス（サイズや色）
ロジック      レコメンデーションサービス（おすすめ商品の通知）
アクセス許可   在庫管理システム連携サービス
データ        販売実績の追加、配送ステータス管理サービス
```
マイクロサービスではこのように小さいサービスを開発してWebAPIを通じて各サービスを呼び出して連携させる。

# 2. マイクロサービスのメリット
マイクロサービスのメリットとして、
- 開発チームがサービスごとに分かれて得意な言語を利用して各サービスの開発を進めることができる
- 変更をかけたいときはシステム全体ではなく、その小さなサービスごとに変更をかけられる
- 小さなサービスで開発単位を進めるため、ビルドやテストの期間が短くなり開発効率が上がる
- モノリシックなシステムだと何か障害が起きたときにどこがおかしいのかルート構造をたどるのに時間がかかるが、原因の突き止めが比較的容易

などがあり、変化に強くて柔軟性の高いアプリケーション開発を行うことができる

# 3. マイクロサービスのデメリット
マイクロサービスのデメリットとして、
- 既にモノリシックなアーキテクチャでシステムを開発させているため、今更システムを分割させるのが難しい
- 一貫性に欠けるため、運用業務の負担が増加する

などがある。

# 4. マイクロサービスフレームワーク
マイクロサービスの開発に使うことができるフレームワーク

## Slim
PHPのマイクロサービスフレームワーク<br>
![alt](https://ec-orange.jp/ec-media/wp-content/uploads/2018/11/microservice_20181112_05.jpg)<br>
[公式](https://www.slimframework.com/)

## Lagom
Javaのマイクロサービスフレームワーク<br>
![alt](https://image.itmedia.co.jp/ait/articles/1806/05/news013_0.jpg)<br>
[公式](https://www.lightbend.com/lagom-framework)

## Bottle
Pythonのマイクロサービスフレームワーク<br>
![alt](https://ec-orange.jp/ec-media/wp-content/uploads/2018/11/microservice_20181112_07.jpg)<br>
[公式](http://bottlepy.org/docs/dev/index.html)

などなど

# 5. マイクロサービスの事例
有名どころだとクックパッド、Amazon、Gunosy、LINE、Netflixなどが挙げられる。最近だとFiNCのスライドがバズってたイメージ

FiNCシリーズ<br>
https://speakerdeck.com/shinofumijp/microservices-at-finc<br>
https://www.slideshare.net/fumiyashinozuka/finc-52564251<br>
http://slides.com/qsona/deck-3#/


# 6. 参考文献
https://ja.wikipedia.org/wiki/%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%B5%E3%83%BC%E3%83%93%E3%82%B9<br>
https://www.salesforce.com/jp/blog/2016/03/microservices.html<br>
https://codezine.jp/article/detail/11055<br>
https://ec-orange.jp/ec-media/?p=23458

# 7. おわりに
インターンでごりっとマイクロサービス化のところ触れられそうなので楽しみ
