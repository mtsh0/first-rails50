いままでrailsは4.2系ばかり使っていたので5.0系との違いを把握するためのリポジトリです:bangbang:

* Ruby version: 2.4.4

* System dependencies: 5.0.7

* Database creation: MySQL

### Rails4.2系と5.0系の大まかな違い

||Rails4.2系|Rails5.0系|備考|
|:--|:--:|:--:|:--|
|対象の<br>Rubyバージョン<br>(必須)|2.0以上<br>(1.9.3)|2.2.2以上|4.2系は1.9.3でも動作するが2.0以上が推奨されている|
|双方向通信|WebSocket|Action Cable| ActionCableとはWebSocketsを利用したリアルタイムコミニュケーションのフレームワークのこと。<br>通常のRailsアプリケーションと同じスタイル・方法でリアルタイム機能をRubyで記述できる。<br>Active RecordなどのORMで書かれたすべてのドメインモデルにアクセスできる|
|WEBサーバ|Unicorn|Puma|ActionCableをサポートするためPumaに変更|
|APIモード|Gemを利用(Grape)|--apiオプションをつけるだけ|Rails5からは`apiオプション`を使うことで、APIとして最低限必要な機能が有効化される。<br>また、ApplicationControllerの継承元がActionController::Baseではなく、ActionController::APIとなる。||
|モデル(継承元)|ActiveRecord::Base|ApplicationRecord|-||
|SQL<br>(or<br>left_outer_joins<br>left_joins<br>メソッド)|該当なし|or<br>left outer join<br>に該当するアクセスコードが追加|SQL文のor、 left outer join にに該当するアクセスコードを `Rails 5`で追加された|
|Turbolinks|ver.4|ver.5|data-turbolinks-permanent<br>data-turbolinks-temporary<br>が追加されたことにより高速化が期待できる|
|gコマンド|`rake`<br>`rails`<br>が混在|`rails`に統一<br>(`rake`コマンドも今までどおり使える)|-|
|対応Rubyバージョン<br>(必須)|1.9.3|2.2.2||

<br>

### Rails5.0(全く知らなかったこと)
- binディレクトリ
  - rails newコマンドでRailsプロジェクトを作成すると、プロジェクト内にbinディレクトリが自動生成される
  - 通常railsコマンドをプロジェクトローカルに実行するにはbundle execを接頭辞のように付与する必要がある
  - bin/railsコマンドを利用することでbundle execを省略することが可能
