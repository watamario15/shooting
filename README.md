# シューティング

[弾避け](/../dodge) | **Windows 専用版** | [クロスプラットフォーム版](/../main)

飛んでくる敵をひたすら撃ち落とし続けるシンプルなシューティングゲームです。上下キーで移動し、右キーで弾を撃ちます。スペースキーを押すと一時停止します。10 秒ごとにレベルが最大 8 まで上がり、奇数レベルでは敵の強さ、偶数レベルでは敵の数が変化します。また、レベル 4 から敵も弾を撃ってきます。得点は時間 1 点、撃破数 5 点です。実行ファイルと同じ場所に作成される `save.bin` ファイルを消すと、最高記録のデータを消去できます。

本作は当初 Windows 専用の通常版 HSP3 で開発していましたが、途中から HSP3Dish を用いた Android 端末を主対象とするクロスプラットフォーム開発に切り替えました。本 branch はクロスプラットフォーム移行前のコードベースを保管するもので、移行後の大量の新要素は含まれません。

## 対応環境

Windows XP 以降の日本語版で動作します。開発環境の制約上、日本語ロケールでしか正しく動作しないのでご注意ください。性能は大して要求しません。こちらは 640x480 なので、画面の小さな PC でもプレイ可能です。

[Releases](../../releases) から適切なものをダウンロードすればインストール不要で遊べます。

## ソースコード

ソースコードは [`shooting.hsp`](shooting.hsp) で、[Hot Soup Processor 3](https://hsp.tv) のスクリプトエディタで開けます。一般のテキストエディタを使う場合は Shift_JIS (CP932) で開いてください。

## 素材

本作品は元は高校時代に個人用に練習で作ったものですが、著作権上マズい素材をふんだんに使っていたので、公開にあたり全て置き換えています。各素材は適宜加工して使用しています。

以下の音声素材は [OtoLogic](https://otologic.jp/) ([CC-BY-4.0](https://otologic.jp/free/license.html)) を使用しています。

- [GB　STG　A01](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`title.mp3`)
- [GB　STG　A02](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`options.mp3`)
- [GB　STG　A03](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`ending_bad.mp3`)
- [GB　STG　A04](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`ending_good,mp3`)
- [GB　STG　A05](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`bgm.wav`)
- [GB　STG　A08](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`gameover.wav`)
- [カウントダウン 01](https://otologic.jp/free/se/countdown01.html) (`countdown.wav`, `go.wav`)
- [SNES　シューティング 01](https://otologic.jp/free/se/game-shooter01.html) (`hit.wav`, `powerdown.wav`)
- [SNES　シューティング 02](https://otologic.jp/free/se/game-shooter01.html) (`pause.wav`)

以下の音声素材は [Kenney](https://www.kenney.nl/) ([CC0-1.0](https://www.kenney.nl/support)) を使用しています。

- [Voiceover Pack](https://www.kenney.nl/assets/voiceover-pack) (`kill.wav`, `shoot.wav`)

以下の画像素材は [Kenney](https://www.kenney.nl/) ([CC0-1.0](https://www.kenney.nl/support)) を使用しています。これ以外は自作ですが、同様に CC0-1.0 とします。

- [Space Shooter Extension](https://www.kenney.nl/assets/space-shooter-extension) (`player.bmp`)
- [Pixel Shmup](https://www.kenney.nl/assets/pixel-shmup) (`fire.bmp`)
- [Tiny Dungeon](https://www.kenney.nl/assets/tiny-dungeon) (`enemy.bmp`)

## 著作権

ソースコードは著作権を放棄し Public Domain ([CC0-1.0](LICENSE)) で配布します。画像素材・音声素材は前節の通りです。
