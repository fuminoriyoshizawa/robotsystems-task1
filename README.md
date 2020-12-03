# robotsystems-task1
ロボットシステム学課題1

# デバイスドライバの概要
講義内で作成したデバイスドライバに改良を行い、LEDをレース場にあるシグナル
風に光らせました。

# 今回使用したもの
* Raspberry Pi4 ModelB 4GB
* 5mmLED(赤2個、青1個)
* ブレッドボード
* 100Ω抵抗　×4
* F-M 20Pジャンパー戦　×8

# 回路概要
LEDはアノード側をGPIO7,8,21,25に接続しています。GNDは各LEDごとに適当な位置に接続しています。

# プログラムのインストール
以下のようにしてインストールを行ってください。
```bash
$ git clone https://github.com/fuminoriyoshizawa/robotsystems-task1.git
$ cd robotsystems-task1/myled
```
# 動作確認



