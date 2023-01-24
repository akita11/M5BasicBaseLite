# M5BasicBaseLite

<img src="https://github.com/akita11/M5BasicBaseLite/blob/main/M5BasicBaseLite1.jpg" width="240px">

<img src="https://github.com/akita11/M5BasicBaseLite/blob/main/M5BasicBaseLite2.jpg" width="240px">

<img src="https://github.com/akita11/M5BasicBaseLite/blob/main/M5BasicBaseLite3.jpg" width="240px">

M5Stackの上部本体(Core Basic)にとりつけて、以下のようなM5GO/Fireの機能やそれ以外の機能を追加できる底板（ベースボード）用の拡張基板です。
[M5GOBaseLite](https://github.com/akita11/M5GOBaseLite)の後継機で、基本的な機能・回路は同一で、裏面のメスMbusコネクタが使えるようになりました。
- Groveコネクタ(PortA(2個), PortB, PortC, PortD, PortE)（PortA/B/CはM5Stack純正のものと同等です。PortD/EはM5Stack純正品にはありませんが、UI Flowで使用することができるポートです）
- 左右5個ずつのNeoPixel (SK6812)（オプション）
- LiPoバッテリ接続端子（オプション）

# 使い方
1. M5Stackの本体(Core、底板を外した状態)に本ボードを差し込みます。
2. M5Stackのプログラムから、Groveコネクタに接続したセンサ類を使用します。
   - 各Groveコネクタのピン配置は以下の通り（中央寄りのVDDから近い側、遠い側の順）
     - PortA: GPIO21(SDA), GPIO22(SCL)
     - PortB: GPIO26, GPIO36
     - PortC: GPIO17(TXD2), GPIO16(RXD2)
     - PortD: GPIO35, GPIO34
     - PortE: GPIO13, GPIO5
   - （オプション）左右のNeoPixelの制御信号はGPIO15につながっています。UI Flowでは、Hardware→RGB LED、から使用できます

# 底面カバー

[M5GOBaseLite](https://github.com/akita11/M5GOBaseLite)用のカバーを使用できます。

# Author

Junichi Akita (@akita11, akita@ifdl.jp)
