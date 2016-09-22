# メタプログラミングPython

Speaker:

https://tell-k.github.io/pyconjp2016/


# Type

* type は typeのinstance
* class はtypeのinstance
* typeを使えばclassを動的に定義できる

## Ghost method

* Ruby: method_missing
* Python: __getattr__
  * __getattr__ないで関数を定義して，その関数を返す

## 特異メソッド

+ pythonの場合，boundメソッドとinboundメソッドがある
  + boundメソッドの場合，MethodTypesを呼び出して，boundメソッドに変えて上げる必要がある

## Monkey Patch

* 元の関数に戻せるよう保存
* with文を使って制限して上げるのが良い

## Metaclass

* 3.3から__prepare__で差し替えることができる


## DSL

* astモジュールで実現

## OpenClass

* 組み込み型にはメソッドを追加することができない
  * forbiddenfruits を使えばできる
