# eloquent-app-practice

## 概要
COACHTECH 教材 Tutorial 9-4「Eloquent ORM ハンズオン演習」で作成した成果物です。
Eloquent モデルを使って、「ブログシステム」の投稿一覧機能（投稿を作成、編集、削除機能あり）を作成

## 使用技術
- PHP 8.5.10
- Laravel 10.50.3
- Eloquent ORM
- MySQL

## 学んだこと
- Eloquent モデルを使った、データの取得、作成、更新、削除からなる CRUD操作
- $fillable を使い、マスアサインメントのセキュリティリスクを塞ぐ必要性があること
- コントローラーに入力した index,create,store,edit,update,delete の役割
- 一度目の動作確認で、投稿を新規作成しようとしたら、エラー出て作成できなかったので、見直したところ、データ操作のメソッドに対して、ルーティング設定での store,update,delete のルートを書いていなかった。書き足し後動作確認をしたらきちんと作成、編集、削除ができた

## 動作確認
- http://localhost/posts
にアクセスし、完成イメージと同じ画面になるか確認した。
- 実際に表示された画面から、投稿の新規作成、編集、削除ができることを確認した。