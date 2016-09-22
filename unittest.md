# Pausable Unittest on EFI Stackless Python

Speaker : Masamitsu Murase

https://masamitsu-murase.blogspot.jp/2016/09/pausable-unittest-on-efi-stackless.html
https://github.com/masamitsu-murase/pausable_unittest

## 概要

* 再起動とかのテストなどを行いたい
  * 変数を戻したい
    * localsでpickel->unpickel
  * メソッドの途中から実行できる
  * 再起動後，勝手に起動するようにしたい．

## Stackless Python

* Cpythonの亜種
* Cのスタックをあまり使わない
* taskletという軽量スレッドを実装

## tasklet

+ 明示的に実行を切り替えられる
+ pickle可能
  + taskletの状態を保存できる

＃EFI

* BIOSの新規格
* EFI ShellというDOSライクなシェルが開く
  * Pythonは移植されている

## FAQ

* Rubyだとできないらしい
