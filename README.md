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
以下のようにしてLEDが光ることを確認してください。
```bash
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
$ echo 1 > /dev/myled0 (左から1番目が点灯)
$ echo 2 > /dev/myled0 (左から2番目までが点灯)
$ echo 3 > /dev/myled0 (左から3番目までが点灯)
$ echo 4 > /dev/myled0 (左から4番目だけが点灯)
```
# 動作の様子
https://youtu.be/9dhs1au0ZRE


