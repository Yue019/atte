# アプリケーション名　Atte
概要：ある企業の勤怠管理システム
![Image](img/atte-top.png)

## 作成した目的
人事評価のため

## アプリケーションURL

## 機能一覧
* 会員登録、ログイン、ログアウト（Laravel認証機能を使用）
* 勤務開始、勤務終了（日を跨いだ時点で出勤を切り替える）
* 休憩開始、休憩終了（1日に何度でも休憩を取得できる）
* 日付別勤怠一覧表
* ページネーション（5件づつ取得）

## 使用技術
* Laravel 8.75
* PHP 8.3.6
* nginx 1.27.1
* mysql 8.0.26

## テーブル設計
![Image](img/atte-table.png)

## ER図
![Image](img/relation.png)

## 環境構築
☆bladeビュー
* ログイン画面（logion.blade.php）
* 会員登録画面（register.blade.php）
* 勤務、休憩打刻画面（index.blade.php）
* 日付別勤怠一覧表（attendance_date.blade.php）

☆モデル
* User.php（ユーザーモデル）
* Work.php（出勤、退勤モデル）
* Rest.php（休憩モデル）

☆コントローラー
* AuthController
* WorkController
* RestController

## その他
テストユーザーアカウント

* 名前:Lazvell
* メールアドレス:zeta@gmail.com
* パスワード:12345678
※ログインにはメールアドレスとパスワードを使用します。


