# コマンド

### migrationが実行されてないものの確認
`bundle exec rake db:migrate:status`

### 特定のversionだけmigrateする
`bundle exec rake db:migrate:up VERSION=[version]`

### 特定のテストだけ流す
`describe "#testA", type: :doing do` # testに書く<br>
`bundle exec rspec --tag type:doing [ファイルパス]` # コマンドを打つ

### Docker時のpryの立ち上げ
`docker-compose start rails`<br>
`docker ps` # プロセスの確認<br>
`docker attach [THE_RAILS_PROCESS]`

### 行数確認
`bundle exec rake stats`<br>
`find ./app/views -name "*.slim" | xargs wc -l`

### slim導入
`gem 'slim-rails'` # Gemfileに追記<br>
`gem ‘html2slim'` # Gemfileに追記<br>
`for i in app/views/**/*.erb; do erb2slim $i ${i%erb}slim && rm $i; done`

### Heroku本番コンソール
`heroku run console --app [app名]`

### 特定のファイルのversionを戻す
`git checkout [コミット番号] [ファイルパス]`

### 特定のブランチをもってくる
`git pull origin [pullしたいリモートブランチ名]:[ローカルブランチ名]`

### Redis(立ち上げ兼操作)
`docker-compose up`<br>
`redis-server`<br>
`docker exec -it [DOCKER_PROCESS] bash`<br>
`redis-cli` #この中で

# エラー

### Docker立ち上げ時にjsでmodule not foundみたいなエラーが出た時
`docker-compose run rails bundle exec yarn add [module]` #自分のローカルに、エラーが出たモジュールが入っていないために起こる
