# HomeHack
家CON2015に提出した作品「4Dコントローラー」の使い方です。
HEMS標準APIおよび住宅APIが搭載されているスマートハウスでの利用を前提としています。

# 環境
* Android(4.0以降)
* Raspberry Pi 2 TypeB
 * 上記端末以外でも動作する可能性はありますが動作確認はしていません。
* AndroidとRaspberry Piが同一ネットワークに存在できる環境

# 4Dコントローラーとは
「4D、つまりデジタル以外の新たな要素を使い新たな感覚や感動」を人に与えることができるコントローラーです。
現状は以下ができます。
* 映像にあわして空調/照明のコントロール
* Android操作で状況に合わした照明コントロール


# 使い方
## Androidアプリをダウンロード
* 以下からAndroid端末にダウンロードをする
[4Dコントローラー](https://play.google.com/store/apps/details?id=com.syatyo.HomeHack)

## Raspberry Piをセットアップ(1)
* 以下からRaspberry PiのイメージをダウンロードしRaspberry Piに反映。
[4Dコントローラーサーバー](http://maron-kun.com/iecon/iecon-rspi-v0100.img)


## Raspberry Piをセットアップ(2)

1. Raspberry Piをネットワークに接続
2. Raspberry PiのPRIVATE IPを取得

## Androidアプリ「4Dコントローラー」(Android上では「4Dコン」)を起動

1. 取得したRaspberry PiのIPを「アクセス先」に入力し「Access」ボタン押下
2. HEMS標準APIおよび住宅APIが待ってるIPを入力（PORT指定が必要な場合、IP:PORTの順で書くこと）
	* 例) IP「192.168.0.1」ポート「1234」の場合、「192.168.0.1:1234」
3. 起動完了

## License
Read LICENSE File. 