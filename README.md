# mypkg
ロボットシステム学練習用リポジトリ
# 機能
* talkerで0から数字をカウントする。
* listenerはtalkerでカウントした数字を標準出力する。

# コマンドのテスト
![test](https://github.com/Aya0801/mypkg/actions/workflows/test.yml/badge.svg)

# ダウンロード方法
ターミナルに入力
```
$ git clone https://github.com/Aya0801/robosys2022.git
```
# 動作例1
端末を二つ開く
端末１
入力

```
$ cd ros2_ws
$ ros2 run mypkg talker　
```
端末2
```
$ cd ros2_ws
$ ros2 run mypkg listener　
```

出力(端末2）
```
[INFO] [1671708122.690112083] [listener]: Listen: 0
[INFO] [1671708123.184632337] [listener]: Listen: 1
[INFO] [1671708123.683623315] [listener]: Listen: 2
[INFO] [1671708124.184743145] [listener]: Listen: 3
[INFO] [1671708124.685106613] [listener]: Listen: 4
[INFO] [1671708125.184969373] [listener]: Listen: 5　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　
```
# 動作例2
入力
```
$ cd ros2_ws
$ ros2 launch mypkg talk_listen.launch.py
```
出力
```
[listener-2] [INFO] [1671708720.257121408] [listener]: Listen: 0
[listener-2] [INFO] [1671708720.748691345] [listener]: Listen: 1
[listener-2] [INFO] [1671708721.248766431] [listener]: Listen: 2
[listener-2] [INFO] [1671708721.748684844] [listener]: Listen: 3
[listener-2] [INFO] [1671708722.249065043] [listener]: Listen: 4
[listener-2] [INFO] [1671708722.749031046] [listener]: Listen: 5
```


## 必要なソフトウエア
* Python 3

## テスト環境
* Ubuntu 20.04.5LTS
# 権利
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* © 2022 Atsuya Sawayama
i
