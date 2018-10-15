# SUP(Shimane University Pedia)

## 前提
* [Codeanywhere](https://codeanywhere.com/) 上で、 Ruby(CentOS7.2) のコンテナを用いる

## 環境構築手順
* Codeanywhere で Ruby(CentOS7.2) のコンテナを適当な名前で作成する

* SSH Terminal (黒い画面) を開く

* このリポジトリを clone する (以下のコマンドを実行する)
```
$ git clone https://github.com/SystemCreation2018/SUP.git
```

* このディレクトリに移動する
```
$ cd SUP
```

* このアプリケーションで用いるライブラリ群をインストールする
```
$ bundle install --path vendor/bundle
```

* データベース及びテーブルを作成する
```
$ rails db:create
$ rails db:migrate
```

* ローカルサーバーを立ち上げる
```
$ rails server
```

## 注意事項
* Codeanywhere は無料枠だとコンテナを一つしか作れない上、 2 ~ 3 週間ログアウトしているとコンテナが抹消されます。 この github でソースコード管理をすることを徹底し、定期的に Codeanywhere のログインをしましょう。
