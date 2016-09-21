# Pythonで作るWebクローラ入門

Speaker: Ai Makabi

* Scrapy
* https://speakerdeck.com/amacbee/pythondezuo-ruwebkuroraru-men
* https://pycon.jp/2016/ja/schedule/presentation/32/

* クローリングの話がメイン
+ beautifulsoup4(スクレイピング)/javascriptの解釈方法については省略

## 参考例
### 類似映画検索

* キャスト，監督，視聴率から類似度を推定．
  * 売上を予測

### トレンド分析

* 在庫情報からトレンドを分析

## Scrapy

* Robots.txtを自動で解釈してクローリングをしてくれる
* Windows環境ではpython3でテスト仕切れていないので，Linux上で行うのが良い
* pipでインストールできる
  * ubuntu ではapt-getでのインストールを推奨
### Spider

* クローラの設定が書かれている

#### 設定情報

* name: クローラ名
* allowed_domain : クロール対象のドメイン(複数可能)
* start_url : クロール開始のurl(複数可能)
* parse
  * ページからクロール対象の要素を返す
  * 次ページへのURLを返す
  * タグ要素の取得には,XpathやCSSのセレクタを使うことができる
    * Beautifulsoupのセレクタも使用できる

### クローリング共通の設定

settings.py
* 確実に設定してほしい
  * DOWNLOAD_DELAY(秒)
  * ROBOTSTXT_OBEYは標準でtrue

logの情報も自動で取得できる．(通常のログ機能と同等のレベル)

## サンプル

* http://www.python.org/jobs
  * 求人情報が載っている

## Tips

* Google Chrome のデベロッパツールでスクレイピング箇所を特定できる
* scrapyには対話環境があるので，必要に応じて調整できる
* クローリングとスクレイピングの処理は分ける
  * 無駄にクローリングを再実行をしない
* Javascriptが含まれているかどうかを確認する
  * めんどい
