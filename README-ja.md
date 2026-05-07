# シューティング

[English](README.md) | **日本語**

[弾避け](/../dodge) | [Windows 専用版](/../legacy) | **クロスプラットフォーム版**

![](title.png)
![](play.png)
![](boss.png)
![](result.png)

飛んでくる敵をひたすら撃ち落とし続けるシンプルなシューティングゲームです。上下キーやタップで移動し、右キーや SHOOT ボタンで弾を撃ちます。スペースキーや PAUSE ボタンで一時停止します。10 秒ごとにレベルが最大 8 まで上がり、奇数レベルでは敵の強さ、偶数レベルでは敵の数が変化します。また、レベル 4 から敵も弾を撃ってきます。アイテムを取ると、少し良いことが起こります。点は耐久時間、撃破数、アイテムの取得数で算出します。

適当なランダムなので回避不能パターンも普通にありますが、その代わりライフが 8 ある上に攻撃／回復アイテムも大盤振る舞いなので、上手くなってくると着実にアイテムを回収していれば割と無限に続きます。

## 対応環境

Linux 環境では、スクリプトの文字コードを UTF-8 に変換すれば [Linux 版ランタイム](https://hsp.tv/make/hsp3linux_pi.html)で動作しますが、導入手順が煩雑なため Wine で exe ファイルを実行するか Web 版を使う方が手軽です（macOS も同様）。開発環境上は iOS/iPadOS にも対応していますが、私がビルド環境もテスト環境も持ち合わせないため作成していません（そもそも野良配布できないし...）。

- Windows XP 以降
  - 実質画面サイズが 1280x720 以上必要です（不足する場合は Web 版や [Windows 専用版](/../legacy)をご利用ください）
  - 高繊細モニタを搭載する機種では実行ファイルを右クリックして「プロパティ>互換性>高 DPI 設定の変更」で、「高い DPI スケールの動作を上書きします。」にチェックを入れて「システム（拡張）」を選択して OK した状態で起動すると、画面に収まる場合があります
- Android 5 以降
  - Play Store 等では公開していないので、提供元不明アプリのインストールを有効化した上で、直接 APK をインストールしてください（ADB からのインストールも可能です）
  - 新しめの OS や可変フレームレートの端末など、環境によってはフレームレートが安定しない場合があります
- 新しめの Web ブラウザ [Experimental]
  - Web 版は「とりあえずビルドしてみた」程度で、環境によってはうまく動かない場合があります
  - 画面をはみ出す環境では全画面モードがおすすめです（縦方向に画面が余ると文字表示が壊れるので、横長状態で全画面化してください）

[Releases](../../releases) から適切なものをダウンロードしてください。Web 版は <https://watamario15.github.io/shooting/> で遊べます（ロードにそこそこ時間が掛かります）。

## ソースコード

ソースコードは [`shooting.hsp`](shooting.hsp) で、[Hot Soup Processor 3](https://hsp.tv) のスクリプトエディタで開けます（ビルドはβ版含む最新版を推奨）。一般のテキストエディタを使う場合は Shift_JIS (CP932) で開いてください。

## 素材

本作品は元は高校時代に個人用に練習で作ったものですが、著作権上マズい素材をふんだんに使っていたので、公開にあたり全て置き換えています（ファイル名やソースコードからお察しください）。各素材は適宜加工して使用しています。

音声素材は [OtoLogic](https://otologic.jp/) ([CC-BY-4.0](https://otologic.jp/free/license.html)) を使用しています。

- [GB　STG　A01](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`title.mp3`)
- [GB　STG　A02](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`options.mp3`)
- [GB　STG　A03](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`ending_bad.mp3`)
- [GB　STG　A04](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`ending_good,mp3`)
- [GB　STG　A05](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`bgm.mp3`)
- [GB　STG　A06](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`bossbgm.mp3`)
- [GB　STG　A08](https://otologic.jp/free/bgm/game-shooter-gb01.html) (`bossclear.wav`, `gameover.wav`)
- [GB　アクションC02](https://otologic.jp/free/bgm/game-action-gb02.html) (`special.mp3`)
- [GB　アクションC08](https://otologic.jp/free/bgm/game-action-gb02.html) (`invincible.mp3`)
- [カウントダウン 01](https://otologic.jp/free/se/countdown01.html) (`countdown.wav`, `go.wav`)
- [SNES　シューティング 01](https://otologic.jp/free/se/game-shooter01.html) (`hit.wav`, `powerdown.wav`, `powerup.wav`)
- [SNES　シューティング 02](https://otologic.jp/free/se/game-shooter01.html) (`btnclick.wav`, `pause.wav`)

以下の画像素材は [Kenney](https://www.kenney.nl/) ([CC0-1.0](https://www.kenney.nl/support)) を使用しています。これ以外は自作ですが、同様に CC0-1.0 とします。

- [Space Shooter Extension](https://www.kenney.nl/assets/space-shooter-extension) (`cloud1.png`, `cloud2.png`, `player.png`)
- [Pixel Shmup](https://www.kenney.nl/assets/pixel-shmup) (`fire.png`, `invincible.png`, `lifeup.png`, `special.png`)
- [Tiny Dungeon](https://www.kenney.nl/assets/tiny-dungeon) (`enemy1.png`, `enemy2.png`)
- [Toon Characters](https://www.kenney.nl/assets/toon-characters) (`jr.png`, `kingbomb.png`, `sledgebro.png`)
- [Platformer Characters](https://www.kenney.nl/assets/platformer-characters) (`bowser2.png`, `bowser3.png`)
- [Roguelike Characters](https://www.kenney.nl/assets/roguelike-characters) (`bowser1.png`)
- [Game Icons](https://www.kenney.nl/assets/game-icons) (`back.png`, `option.png`, `reset.png`)

## 著作権

ソースコードは著作権を放棄し Public Domain ([CC0-1.0](LICENSE)) で配布します。画像素材・音声素材は前節の通りです。
