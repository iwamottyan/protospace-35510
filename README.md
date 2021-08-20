## usersテーブル

| Column   | Options             |
| ------   | ------------------- |
| email    | (string型,NOT NULL) |
| password | (string型,NOT NULL) | 
| name     | (string型,NOT NULL) |
| profile  | (text型, NOT NULL)  |

## prototypesテーブル

| Column   | Options                |
| ------   | ---------------------- |
| title    | (string型,NOT NULL)    |
| catch_copy | (text型, NOT NULL)   |
| concept    | (text型, NOT NULL)   |
| image      | (ActiveStorageで実装) |
| user       | (references型)       |

## commentsテーブル

| Column    | Options            |
| ------    | ------------------ |
| text      | (text型, NOT NULL) |
| user      | (references型)     |
| prototype | (references型)     |