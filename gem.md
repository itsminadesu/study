gemってなんだ！ bundleってなんだ！

# 目次
1. そもそもライブラリってなんだ
2. gemってなんだ
3. RubyGemsってなんだ
4. Bundlerってなんだ<br>
  4.1 Gemfile/Gemfile.lockとは<br>
  4.2 bundle install/bundle updateの違い
5. 参考文献
6. おわりに

# 1. そもそもライブラリってなんだ
> ITの分野では、ある特定の機能を持ったコンピュータプログラムを他のプログラムから呼び出して利用できるように部品化し、そのようなプログラム部品を複数集めて一つのファイルに収納したものをライブラリという。

(IT用語辞典より)

要は汎用性の高いプログラムを再利用できる形でまとめたもののことで、ライブラリを使うことで自分で1からプログラムを記述する必要がなくなる

# 2. gemってなんだ
Ruby用のライブラリのことをgemという。

gemの例
```
Ruby on Rails(Webフレームワーク) ← 実はRailsもgem
omniauth(認証)
RSpec(テスト)
```

# 3. RubyGemsってなんだ
> RubyGemsは、Ruby言語用のパッケージ管理システムであり、Rubyのプログラムと（"gem" と呼ばれる）ライブラリの配布用標準フォーマットを提供している。gemを容易に管理でき、gemを配布するサーバの機能も持つ。Rubyバージョン1.9以降では標準ライブラリの一部となっている。

(Wikipediaより)

要はgem専用のパッケージ管理システムのこと。
[rubygems.org](https://rubygems.org/)でgemの情報公開、提供を行なっている。

# 4. Bundlerってなんだ
Bundlerは`Gemfile`と`Gemfile.lock`に従ってgemを管理するライブラリのこと。gemは`gem install 'omniauth'`のように個別インストールも可能だが、様々なgemを組み合わせて使っていると、
```
gemAのver1とgemBのVer2はうまく動くけど、最新バージョン同士だとうまく動かない
複数人、複数環境で開発を行う場合、各環境で使うライブラリの名前、バージョンを合わなければならない
```
のようなことが起こりうる。そのような時にgem同士の互換性を保ちながら各gemの導入、管理を行ってくれるのがBundler

## 4.1 Gemfile/Gemfile.lockとは
Gemfileとは、gemをインストールするための`設計図`のようなもの。開発に必要なgemをこのGemfileに記載する。<br>
Gemfile.lockとは、実際にgemをインストールした後の結果を記載したもの。gem同士は関連し合っていることが多く、Gemfileに書いてあるgemの他にも必要なgemがあることがあり、Bundlerはそれらを自動でインストールし、Gemfile.lockに記述する。
## 4.2 bundle install/bundle updateの違い
bundle installすると、`Gemfile.lock`を元にgemのインストールを行う。もしGemfileに更新があれば、そのgemとそのgemに関連するgemをインストールした後にGemfile.lockを更新する。<br>
bundle updateをすると、`Gemfile`を元にgemのインストールをし、Gemfile.lockを更新する。

# 5. 参考文献
http://e-words.jp/w/%E3%83%A9%E3%82%A4%E3%83%96%E3%83%A9%E3%83%AA.html<br>
https://tech-camp.in/note/technology/55305/<br>
https://ja.wikipedia.org/wiki/RubyGems<br>
https://qiita.com/mochikichi321/items/ee0b7133524816f73e60<br>
https://qiita.com/oshou/items/6283c2315dc7dd244aef<br>
https://qiita.com/3no3_tw/items/8c1e3e95c75edae1036d<br>
https://qiita.com/lasershow/items/1a048d03ddaaba98171e<br>
https://qiita.com/YusukeHigaki/items/0314e2ec1d13cc5d4c99<br>

# 6. おわりに
雰囲気でやってたので地味に理解が深まった
