# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


# ChronoEditor
with this application you can create a personal chronology.

## Description
with this application you can create a personal chronology.

## Demo
image/gif URL

## Usage
hoge

## Requirement
hoge

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

## Licence
hoge

## Author
[Shuichiro Saeki](https://github.com/SSaeki-jp)