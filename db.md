DBさらっとまとめ

# 目次
1. DBとは
2. 代表的なDB
3. リレーショナルデータベース(RDB)とは
4. データベース管理システム（DBS）とは
5. おわりに

# 1. DBとは
> データベース（英: database, DB）とは、検索や蓄積が容易にできるよう整理された情報の集まり。 通常はコンピュータによって実現されたものを指すが、紙の住所録などをデータベースと呼ぶ場合もある。 狭義には、データベース管理システム (Database Management System, DBMS) またはそれが扱う対象のことをいう。

つまり、**一定の形式で「複数で共有・利用すること」と「検索・加工すること」を目的に整理されたデータの集まり**のこと。

# 2. 代表的なDB
## Oracle Database
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/wpid-wp-1420713408925-640x217.jpeg)
- 機能や動作速度、堅牢性に定評があり、たくさんの企業で使われているデータベース
- 高機能だが高額なため、**大規模なデータ管理**に使われることが多い

[公式](https://www.oracle.com/jp/database/index.html)

## MySQL
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/mysql-logo-640x267.jpg)
- 世界で最も有名な**オープンソースデータベース**で、基本的に無料で使用することができる
- 多くのレンタルサーバで利用することができるため、市場シェアが高いデータベース
- XAMPPで標準インストールされ、PHPとの相性も非常に良い

[公式](https://www.mysql.com/jp/)

## PostgreSQL
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/slonik_with_black_text_and_tagline-640x234.gif)
- MySQLと同じ**オープンソースデータベース**
- 大規模商用データベースが持つような機能をもっており、MySQLと並んで人気がある
- MySQLに比べて、**関数や機能等が豊富**なのも特徴としてあげられます。

[公式](https://www.postgresql.jp/)

## SQLite
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/sqlite-183454_640.png)
- データ保存に**単一ファイルのみ**を使用する軽量データベース
- **中小規模**のデータ管理に適しており、今モバイル環境での利用がとても増えている
- アプリケーションに組み込んで利用されることを想定していて、Android端末の標準ライブラリとして採用されている

[公式](https://www.sqlite.org/index.html)

## Microsoft SQL Server
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/sqlserver-640x163.png)
- MicrosoftがOracleの対抗製品として開発しているデータベース
- 高機能な分高額
- **Windows ServerやMicrosoftの開発言語との相性が抜群に良い**

[公式](https://azure.microsoft.com/ja-jp/?ocid=cloudplat_hp)

## Microsoft Access
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/Microsoft-Access-Course.jpg)
- Microsoft office製品の一つで、他のoffice製品同様の操作感でデータベースの構築・管理を行うことができる
- **Windows ServerやMicrosoft office製品との親和性がとても高く、使いやすい**

[公式](https://products.office.com/ja-jp/access)

## FileMaker
![alt](https://www.sejuku.net/blog/wp-content/uploads/2016/07/filemaker_logo-640x147.png)
- MacOS、Windowsで使用できるデータベース
- **グラフ作成機能が充実**していて、レポート作成や分析資料作成をしやすいことで人気
- iPhoneやiPadとの親和性も高く、好んで利用している人も多くいる

[公式](https://www.filemaker.com/jp/)

# 3. リレーショナルデータベース(RDB)とは
> リレーショナルデータベース（RDB）とは、「テーブル」といわれる表形式の構造でデータを管理する関係モデルを使ったデータベース

1つのテーブルごとに、「商品」「スタッフ」「売り上げ」のように**関連性のある一連のデータ**がそれぞれ格納される。
行はレコード、列はフィールドと呼ばれ、1行に1件のデータが格納されて1レコードとなる。この時、各レコードのデータは必ず**一意**にならないといけない。

RDBが使われる理由は大きく分けて
- データの重複を避けられる<br>
- 検索能力が高い<br>

の二つがあり、1つ見つかればそこで検索作業を終了できるため、データを検索するスピードを上げることができる

# 4. データベース管理システム（DBS）とは
**データベースを効率よく管理、運用するソフトウェア**のこと
(図書館の司書さん的な)

特に、リレーショナルデータベース(RDB)を管理、運用するデータベース管理システムのことをリレーショナルデータベース管理システム(RDBS)という

データベースは自動でデータを追加、更新、削除などの操作は行わないため、コンピュータのシステムに管理してもらおう！ということで、DBSは必要

# 5. おわりに
さらっとまとめたけど、DBへの理解が深まった
