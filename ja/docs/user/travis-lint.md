---
title: .travis.ymlの検証
layout: ja
permalink: travis-lint/
---

### このガイドについて

ここでは、[travis-lint](https://github.com/travis-ci/travis-lint)という、`.travis.yml`ファイルを検証してよくある問題を見つけるのをたすけてくれる小さなツールについて解説していきます。
travis-ci.orgを使い始めるための情報を探しているなら、[はじめに](/ja/docs/user/getting-started/)から見てみてください。

## lint.travis-ci.orgを使う

[.travis.yml validation Web app](http://lint.travis-ci.org)で簡単に`.travis.yml`の検証が行えます。

## travis-lintコマンドラインツールを使う

もしRuby 1.8.7+とRubyGemsがインストール済みなら、[travis-lint](http://github.com/travis-ci/travis-lint)で`.travis.yml`ファイルを検証できます。
次のように導入します。

    gem install travis-lint

そしてあなたの`.travis.yml`に対して実行します。:

    # .travis.ymlのあるリポジトリ内
    travis-lint

    # その他のディレクトリから
    travis-lint [path to your .travis.yml]

`travis-lint`はできたばかりですが、travis-ci.orgユーザーから学んだよくある問題のためのより多くのチェックを元に日々改善されています。
