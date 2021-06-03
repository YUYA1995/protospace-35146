# README

# テーブル設計

## users テーブル
| Column     | Type    |  Option     |
| ---------- | ------- | ----------- |
| email      | string  |  NOT NULL   |
| password   | string  |  NOT NULL   |
| name       | string  |  NOT NULL   |
| profile    | text    |  NOT NULL   |
| occupation | text    |  NOT NULL   |
| position   | text    |  NOY NULL   |

## prototype テーブル
| Column     | Type       |  Option   |
| ---------- | ---------- | --------  |
| title      | string     | NOT NULL  | 
| catch_copy | text       | NOT NULL  |
| concept    | text       | NOY NULL  | 
| user       | references |           |

## comments テーブル
| Column     | Type       |  Option  |
| ---------- | ---------- | -------- |
| text       | text       | NOT NULL |
| user       | references |          |
| prototype  | references |          |


