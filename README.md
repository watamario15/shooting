# 敵避けゲーム

**弾避け** | [Windows 専用版](/../legacy) | [クロスプラットフォーム版](/../main)

マウスを動かして上からランダムに降ってくる敵をひたすら避け続けるシンプルなゲームです。10 回ごとにレベルが最大 5 まで上がり、1 度に出る敵の数も増えます。スペースキーを押すと一時停止します。実行ファイルと同じ場所に作成される `save.bin` ファイルを消すと、最高記録のデータを消去できます。

次作のシューティングゲームの原型となった作品です。

## 対応環境

Windows XP 以降の日本語版で動作します。開発環境の制約上、日本語ロケールでしか正しく動作しないのでご注意ください。性能は大して要求しません。

[Releases](../../releases) から適切なものをダウンロードすればインストール不要で遊べます。

## ソースコード

ソースコードは [`dodge.hsp`](dodge.hsp) で、[Hot Soup Processor 3](https://hsp.tv) のスクリプトエディタで開けます。一般のテキストエディタを使う場合は Shift_JIS (CP932) で開いてください。

## 素材

本作品は元は高校時代に個人用に練習で作ったものですが、著作権上マズい素材をふんだんに使っていたので、公開にあたり全て置き換えています。各素材は適宜加工して使用しています。

音声素材は [OtoLogic](https://otologic.jp/) ([CC-BY-4.0](https://otologic.jp/free/license.html)) を使用しています。

- [GB　レース　A01](https://otologic.jp/free/bgm/game-sports-gb01.html) (`title.mp3`)
- [GB　レース　A03](https://otologic.jp/free/bgm/game-sports-gb01.html) (`bgm.mp3`)
- [GB　レース　A06](https://otologic.jp/free/bgm/game-sports-gb02.html) (`result.mp3`)
- [GB　レース　A09](https://otologic.jp/free/bgm/game-sports-gb02.html) (`gameover.wav`)
- [カウントダウン 01](https://otologic.jp/free/se/countdown01.html) (`countdown.wav`, `go.wav`)
- [SNES　シューティング 02](https://otologic.jp/free/se/game-shooter01.html) (`pause.wav`)

以下の画像素材は [Kenney](https://www.kenney.nl/) ([CC0-1.0](https://www.kenney.nl/support)) を使用しています。これ以外は自作ですが、同様に CC0-1.0 とします。

- [Pixel Platformer](https://www.kenney.nl/assets/pixel-platformer) (`enemy.bmp`, `player.bmp`)

## 著作権

ソースコードは著作権を放棄し Public Domain ([CC0-1.0](LICENSE)) で配布します。画像素材・音声素材は前節の通りです。
