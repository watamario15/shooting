# シューティング

[弾避け](/../dodge) | [Windows 専用版](/../legacy) | **クロスプラットフォーム版**

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

本作品は元は高校時代に練習で作ったものですが、著作権上マズい素材をふんだんに使っていたので、公開にあたり全て置き換えています。

音声素材は以下の通りです。

- カウントダウン効果音（`countdown.wav`, `go.wav`）：[カウントダウン 01](https://otologic.jp/free/se/countdown01.html)

画像素材は以下の通りです。

- 設定（`option.png`）： [Phosphor Icons](https://phosphoricons.com/) にて [MIT License](https://github.com/phosphor-icons/homepage/blob/master/LICENSE) で配布されている gear です
- 戻る（`back.png`）： [Phosphor Icons](https://phosphoricons.com/) にて [MIT License](https://github.com/phosphor-icons/homepage/blob/master/LICENSE) で配布されている arrow-u-down-right です
- ゴミ箱（`reset.png`）：[SVG Repo](https://www.svgrepo.com/) で CC0-1.0 で配布されている [Delete SVG Vector](https://www.svgrepo.com/svg/171102/delete) です
- その他ボタン類：ペイントで適当に作ったものですが、文字は [OFL-1.1](https://openfontlicense.org/) で提供される [BIZ UDPGothic](https://github.com/googlefonts/morisawa-biz-ud-gothic) を使用しています（私の作業分については著作権を主張しません）

## 著作権

ソースコードは [MIT License](LICENSE) で配布します。画像素材・音声素材は前節の通りです。

プログラムの最終更新: 2020年09月27日(日)
