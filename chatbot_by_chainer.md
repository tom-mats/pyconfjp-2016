# ニューラルネットワークのフレームワークであるChainerで始める対話Botの作成

Speaker: Masaya Ogushi

http://www.slideshare.net/Gushi/chainer-bot-slide-share-64321155
http://www.slideshare.net/Gushi/chat-bot-madebythechainer

*　New character の実装の方がデータが少なくとも実装できるので，最初にやるのがいい
* 見た目は重要
  * 話しやすい
  * 賢くなさそう

* NeuralStory Teller
  * メッセージにキャラクター付けを行う．
    * 必要なのキャラクターの情報だけ与えれば良い

* つぶやきには内容をカテゴライズして回答
  * NNで実装
* 質問応答はelastic searchで対応

* Wikipedia entitiy vector
* コンセプトの数が多すぎるので，コサイン類似度でグルーピングを繰り返して減らしていった

* 連続性
  * Recurrent NN
* 重度
  * Attention model(NN)
