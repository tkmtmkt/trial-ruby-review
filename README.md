trial-ruby
==========

準備
----

オンライン環境でgemをインストールする。

```sh
$ bundle install --path vendor/bundle
```

インストールしたgemをローカル用に保存する。

```sh
$ bundle package
```

cacheに保存したgemからgemをインストールする。

```sh
$ bundle install --path vendor/bundle --local
```

bundleで管理しているgemのコマンドスタブ作成

```sh
$ bundle binstubs rake pry review
```

実行
----

```sh
$ bin/review-init my-book
$ mv my-book/* .
$ rmdir my-book
```

```sh
$ bin/rake epub
$ bin/rake pdf
```
