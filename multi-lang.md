# 複数の言語からなるプロジェクトを作るということ

Speaker: Kosuke Kusano

https://github.com/cocuh/pyconjp2016-chimera

## 概要

* マルチ言語でのテスト方法について話す予定

### なぜ分けるか

* 実行/開発環境は意外に重要
* パッケージ管理とか


### numpy

* c+python
* UIFとしてPythonは向いているが遅い
* Cは速い
* python-(bind)->C

## 言語を組み合わせる

* 手続き呼び出し(procedure call)に還元される

### Ctypes

* Structureを触るのは向いていない
* Build/Pathの管理はしてくれない

### Cython

* 内部的にはC extensionでコードを生成するので，デバッグする際は注意
* C++もサポートできるがドキュメントが不足している
+ Interface定義を行う程度にとどめておいた方が良い

## Rust+Python

* モダンな型

## まとめ

* 結合度は下げる
* 依存ライブラリの扱いがたいへん
* Cとの連携には向いているが多言語化には向いていない
