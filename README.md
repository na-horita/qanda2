
# Ruby on Rails で作るQ&Aサイトを作成する。
Q＆Aサイトの作成
## 設定
#### Ruby・Railsの基本的なコマンド
```:コマンドプロンプト
ruby -v
rails -v
//全てのルートパスの確認
rails routes
rails db
```
### 環境構築
```:コマンドプロンプト
rails new qanda2 _7.0.4_
bundle install
```
```:コマンドプロンプト
//目的とするファイルに移動
cd qanda2
//サーバー立ち上げ
rails s
```

### 『Question(質問)のコントローラー・モデル作成』
```:コマンドプロンプト
//コントローラー作成時は　複数形で記述
rails g controller questions

//モデル作成時は　単数形でイニシャルは大文字で記述
rails g model Question name:string title:string content:text

//モデルの情報をDBに反映します。
rails db:migrate
```
