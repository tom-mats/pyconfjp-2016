# 週末サイエンティストの勧め

Speaker: Kashino Yuta(BakFoo, Inc)

## 概要

### なぜ可能か

* 計算リソースが安価
  * Cloud Service (GPU付きのもある)
  * 通信が高速(シームレス)
  * 仮想環境(自分が作った環境を外に渡すのが簡単)
* データがいっぱい
  * arXiv(オープンアクセスジャーナル)
  * オープンデータ
  * カンファレンスデータ(ビデオ)
    * Open AI
    * Google
  * 勉強会
  * 講義ビデオ(MOOC)
* OSS
  * 専門家が仕事や教育のためにライブラリを書き始め, Githubに乗せるようになった
    * NeXTの夢

## 研究リテラシー

* アイディアを思いつく
* 論文を探すこと
* 自習
* 科学的方法論
* Publish

### 論文を探す

+ arXiv
  + GitXiv arXivのまとめサイト
+ カンファレンスをチェック
+ SNS

### 自習

+ 継続的なdeliberate practice
  + 目的は明確
  + 時間は短く
  + Feedback
  + 間違いはfix

## 環境構築

### 整備

+ サーバーを借りる
  * 隙間時間にアクセスしたい
  * 計算を止めたくない
  *  GPUを使うならAWS, さくら
    * sakura : コストパフォーマンスがいい
    * AWS : スケーリングしやすい
+ OSはUbuntu
  + 科学スタックはほとんどUbuntuベースで開発
+ PythonはAnaconda(conda+pip)
  + condaが楽
  + 昔はpipと相性が悪かったが，最近は問題がない
  + バイナリを入れてくれる
  + 2を使う場合は3を考慮したコーディングをしておいたほうが良い
+ 実験環境
  + Dockerが良さそう
+ コード保全はgit
  + testN.pyは禁止

### 科学スタック

+ pyflux
* https://github.com/bakfoo/awesome-pysci

## サンプル

気象データはulmoを使えばデータも入手できる

### 地震波解析

+ odspy
