受託でWebpack使ったので備忘録込みのさらっとまとめ

# 目次
1. Webpackとは
2. Webpackのメリット
3. Webpackの基本的な役割
4. 参考文献
5. おわりに

# 1. Webpackとは
[Webpack](https://webpack.js.org/)とはウェブコンテンツを構成するファイル(jsとかsassとか)をまとめてしまうツールのこと。Webpackを使うことで、複数のjsファイルをひとつのjsファイルにまとめたり、複数のsassファイルをひとつのsassファイルにしたりできる

![alt](https://i1.wp.com/goworkship.com/magazine/wp-content/uploads/2018/09/32af52ff9594b121517ecdd932644da4.png?resize=640%2C351&ssl=1)

# 2. Webpackのメリット
## ファイル取得時間の短縮
複数のJS、CSS、画像ファイルなどを１つにまとめることによって通信の際にファイル取得時間を短縮できる

## プラグインの豊富さ
Webpackには豊富なプラグインが用意されており、出力ファイルの圧縮やファイルでのエラーのスキップなど様々な期待される用途によって出力を分けることができる。

## 環境ごとに実行ファイルを分けれる
同じソースコードからwebブラウザで動く用のjsファイルとnodeサーバーで動く用のjsファイルなど、使用する環境に応じて異なった出力をすることができる。
これにより一つのサービスを複数の環境で提供することを容易になる。

## その他
コードが読みやすくなる、保守性が高くなるなど...

# 3. Webpackの基本的な役割
Webpackは自分で書いたJSとライブラリとして読み込んでいるJSを一つのJSファイルにまとめてくれ、またJSライブラリで読み込む必要があるCSSファイルたちもJSにまとめてくれる。かつそれらのCSSで読み込む画像ファイルもJSファイルにまとめてくれるので、JS/CSS/画像ファイルを一つのJSファイルにまとめてくれる。すごい

![alt](https://camo.qiitausercontent.com/3dacc1d70f3e3223763853934e8a6292fafde7a4/68747470733a2f2f71696974612d696d6167652d73746f72652e73332e616d617a6f6e6177732e636f6d2f302f37333434362f34316565366532342d383832352d353466372d646134362d3262613861623731396531332e6a706567)

# 4. 参考文献
https://webpack.js.org/
https://github.com/webpack/webpack/
https://goworkship.com/magazine/how-to-webpack/
https://qiita.com/Shagamii/items/698a67bab0cd5eefcb4f
https://qiita.com/kamykn/items/45fb4690ace32216ca25

# 5. おわりに
実際の現場だとセットアップ全部済んだ状態で使うこと多いから、個人開発で取り入れるのあり
