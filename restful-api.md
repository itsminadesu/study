REST / RESTful APIさらっとまとめ

# 目次
1. そもそもRESTとは
2. そもそもAPIとは
3. RESTful APIとは
4. RESTful APIのメリット
5. 参考文献
6. おわりに

# 1. そもそもRESTとは
> Representational State Transfer (REST) は、ウェブのような分散ハイパーメディアシステムのためのソフトウェアアーキテクチャのスタイルのひとつである。

(Wikipediaより)<br>

REST(**RE**presentational **S**tate **T**ransfer)はWebサービスの設計モデルのこと。RESTなWebサービスは、そのサービスのURIにHTTPメソッドでアクセスすることでデータの送受信を行う。<br>
RESTは4つの設計原則があり、
```
1. ステートレス性(Stateless)
セッションなどの状態管理を行わない。(やり取りされる情報はそれ自体で完結して解釈することができる)

2. 統一インターフェース(Uniform Interface)
情報を操作する命令の体系が予め定義・共有されている。（HTTPのGETやPOSTメソッドなど）

3. アドレス可能性(Addressability)
すべての情報は汎用的な構文で一意に識別される。（URLやURIなど）

4. 接続性(Connectability)
情報の内部に、別の情報や(その情報の別の)状態へのリンクを含めることができる。
```
この原則に従ったWebサービスをRESTfulなサービスという

# 2. そもそもAPIとは
API(Application Programming Interface)とは、何かしらのサービス提供者が、そのサービスを利用するために提供するインタフェースのこと

# 3. RESTful APIとは
> RESTful APIとは、Webシステムを外部から利用するためのプログラムの呼び出し規約（API）の種類の一つで、RESTと呼ばれる設計原則に従って策定されたもの。RESTそのものは適用範囲の広い抽象的なモデルだが、一般的にはRESTの考え方をWeb APIに適用したものをRESTful APIと呼んでいる。

(e-Wordsより)

要はRESTの原則に則って構築されたWebシステムのHTTPでの呼び出しインターフェースのこと

# 4. RESTful APIのメリット
- URIに規則が生まれることで、利用する開発者が把握しやすく実装しやすい
- ブラウザへURIを入力するだけでリソースの参照ができる
- ステートレスであり、サーバ・クライアント間で何も共有しないため、負荷に応じたスケーラビリティを向上することができる
- HTTP標準のメソッドを使うことで、シンプルかつ一貫性のあるリクエストを円滑に行うことができる
- RESTfulAPIを公開することで、標準的なデータフォーマットを使い多様なアプリケーションを提供することができる

# 5. 参考文献
https://ja.wikipedia.org/wiki/Representational_State_Transfer<br>
https://qiita.com/TakahiRoyte/items/949f4e88caecb02119aa<br>
http://e-words.jp/w/RESTful_API.html<br>
http://wp.tech-style.info/archives/683<br>
https://qiita.com/masato44gm/items/dffb8281536ad321fb08<br>
https://qiita.com/kamihork/items/f9d31c03505028d8a9e9

# 6. おわりに
慣れるには手を動かすのみだけど、読みものとしてここら辺読んだら面白かった

[翻訳: WebAPI 設計のベストプラクティス](https://qiita.com/mserizawa/items/b833e407d89abd21ee72)<br>
[GoogleのWebAPI設計とWebAPI設計のベストプラクティスを比較してみる](https://qiita.com/howdy39/items/3b2b14ce73ec44c54f7b)<br>
[RESTful API設計におけるHTTPステータスコードの指針](https://qiita.com/uenosy/items/ba9dbc70781bddc4a491)
