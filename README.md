# README
# ChronoEditor

## アプリの説明
ChronoEditorを使えば簡単に自分史を作ることができます。
自身の生い立ちを振り返ってみたり、故郷の思い出を綴ってみましょう。

## URL
https://chrono-editor.herokuapp.com/

## テストアカウント
現在はなし

## 利用方法
### 起動方法
上記のURLからアクセスできます。
### ログイン／新規登録方法
ヘッダーからログイン／新規登録ができます。

## 目指した課題解決
「20~35歳くらいの年齢層」の、自分らしさの土台となる「自分はどんな人間か、自己の再確認」に寄り添うことを目的としています。

## 開発環境
Ruby 2.6.5 / Ruby on Rails 6.0.0 / MySQL / Heroku / GitHub / Visual Studio Code / Trello

## ローカルでの動作方法
クローンを作成したいディレクトリ上で以下のコマンドを実行する
% git clone https://github.com/SSaeki-jp/chrono-editor.git
% cd chrono-editor
% bundle install
% yarn install
% rails db:create
% rails db:migrate
% rails s

## 要件定義
## Tables
#### users
| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| nickname | string | null: false |
| email    | string | null: false |
| password | string | null: false |
##### Association
- has_one :chronology

#### chronologies
| Column  | Type       | Options           |
| ------- | ---------- | ----------------- |
| user_id | references | foreign_key: true |
| date    | datetime   | null: false       |
| text    | text       | null: false       |
##### Association
- belongs_to :user

## Author
[Shuichiro Saeki](https://github.com/SSaeki-jp)


### 後日記載予定

## 投稿機能の概要

## デモ
image/gif

## Licence
hoge
