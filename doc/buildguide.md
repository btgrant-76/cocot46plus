# Build Guide

![cocot46plus_main12](https://user-images.githubusercontent.com/88039287/170438554-630e1c55-a0de-4021-96c9-22d9bfee850e.jpg)

cocot46plusのビルドガイドになります。
cocot46plusは中央に34mmトラックボールを備えていることが一つの特徴です。
また親指キーの中央にロータリーエンコーダを配置しており、ホームポジションを崩すことなく両手の親指でエンコーダの操作が可能となっています。
中央奥側にはOLEDには現在のレイヤー情報、トラックボールのステータス（CPIや回転軸の角度など）を表示することができます。
その他オプションとしてアクリル積層ケースを用意しているので、お好みに合わせて実装ください。

## 部品
### キット付属品

|名前|数|備考|
|---|---|---|
|スイッチプレート（FR4）|1枚||
|実装済基板|1枚|![PCB](https://user-images.githubusercontent.com/88039287/170449594-f5357de6-4e08-4077-a050-3e613a48e674.jpg)|
|ボトムプレート➀（アクリル）|1枚||
|ボトムプレート➁（FR4）|1枚||
|OLEDカバープレート（FR4）|1枚||
|M2 スペーサー 8mm（メス―メス）|15本|![Spacer_8mm](https://user-images.githubusercontent.com/88039287/170515649-114cee4e-3dec-4465-a310-c989946c1a42.jpg)|
|M2 スペーサー 6mm（メス―メス）|4本|![Spacer_6mm](https://user-images.githubusercontent.com/88039287/170515641-9056cd4a-f58b-4ec7-a39d-e395ed9dab3d.jpg)|
|M2 スペーサー 3mm（メス―オス）|4本|![Spacer_3mm](https://user-images.githubusercontent.com/88039287/170515631-8b3ecdaf-416b-4bc4-814a-b78e2ecb9564.jpg)|
|M2 ねじ 3mm|19本|![Screw_3mm](https://user-images.githubusercontent.com/88039287/170508488-f9c20e9d-b73d-4815-877d-80143e98b4a0.jpg)|
|M2 ねじ 5mm|15本|![Screw_5mm](https://user-images.githubusercontent.com/88039287/170508494-bdf5d0af-b931-436f-9bb0-2520529e32d8.jpg)|
|M2 ねじ 8mm|4本|![Screw_8mm](https://user-images.githubusercontent.com/88039287/170508513-d78bf413-0ffd-4d2b-af5c-ba677e04bc4d.jpg)|
|MX互換スイッチ用PCBソケット|46個|![SwitchSocket](https://user-images.githubusercontent.com/88039287/169816640-7a40ab51-2435-484f-a2ad-c020c374494e.jpg)|
|マウスセンサー（ADNS-5050）・レンズ|1個|![ADNS5050](https://user-images.githubusercontent.com/88039287/169820156-9035cbba-5442-4802-9604-11034021dc22.jpeg)|
|マウスセンサー用LED|1個|![SensorLED](https://user-images.githubusercontent.com/88039287/169820117-6e0fe2ec-c245-4c5a-a4a0-493fbcde3c55.jpeg)|
|OLEDモジュール・ピンソケット・ピンヘッダ|各1個|![OLED](https://user-images.githubusercontent.com/88039287/169819901-5ce452c8-a375-4aa5-b7b8-a138fdbe6984.jpeg)|
|タクトスイッチ|1個|![ResetSwitch](https://user-images.githubusercontent.com/88039287/169819952-702c3c93-5d5c-447f-826e-60da1ef909b2.jpeg)|
|ロータリーエンコーダ（EC12互換）|1個|![RotaryEncoder](https://user-images.githubusercontent.com/88039287/169816718-450c08e5-dff6-49ae-8aa3-451d7397d9e2.jpg)|
|フルカラーシリアルLED (SK6812MINI-E)|2個|![SK6812MINI-E](https://user-images.githubusercontent.com/88039287/169815407-b250e15f-a0f6-411f-9e6a-54aa07cd5fa0.jpg)|
|ゴム足|6個|![ゴム足](https://user-images.githubusercontent.com/88039287/169814183-75fbffd8-37b3-4ab7-a23b-17e0d72b70cd.jpg)|


### キット以外に必要なもの

下記パーツは[遊舎工房](https://shop.yushakobo.jp/)、[TALP KEYBOARD](https://talpkeyboard.net/)、[Daily Craft Keyboard](https://shop.dailycraft.jp/)などで揃えることが可能です。

|名前|数|備考|
|---|---|---|
|MicroUSB or USB-TypeCケーブル|1本||
|ProMicro|1個||
|コンスル―（2.5mm×12ピン）|2本||
|キースイッチ|46個|MX互換|
|キーキャップ（1U）|46個|MX互換|
|ロータリーエンコーダ用ノブ|1個|最大直径22mm以下|

各ショップの在庫状況に応じて検討ください。

### オプション部品（アクリル積層ケース）

アクリルは遊舎工房やAnymanyなどのレーザーカットサービスでお好きな色のアクリルプレートを発注することが可能です。

シリコンシートは[こちら](https://www.monotaro.com/p/3629/5253/)から購入可能です。

|名前|数|備考|
|---|---|---|
|アクリルミドルプレート（上）|1枚|アクリル積層ケース用|
|アクリルミドルプレート（下）|1枚|アクリル積層ケース用|
|シリコンシート厚さ0.5mm|1枚|アクリル積層ケース用|



## 組み立て
### 0. 部品確認

  まずはキット付属品に記載されたパーツが揃っているか確認ください。  
  その他上述の「キット以外に必要なもの」および「オプション部品」を揃えた上で組み立てに取り掛かってください。

### 1. ダイオード

  ver1.0以降は予め基板にはんだ付けされているので、ダイオードのはんだ付けは不要です。


### 2. インジケータLED

  ProMicro横の2箇所にインジケータLEDのはんだ付けを行います。4箇所あるパッドの1箇所に予備はんだを盛り、LEDの位置を固定します。PCBのシルク上の角の部分と、LEDの三角に欠けている部分の向きが揃うようにはんだ付けしてください。LEDは非常に熱に弱いので、はんだごての温度を低めに設定し、一か所はんだ付けをしたら十分時間をおいてから次のはんだ付けを行いましょう。  
  この段階で後述のファームウェアを準備し、LEDの点灯を一つずつ確認しながらはんだ付けを行うとミスの早期発見につながります。

  ![cocot46plus_bg_02_1](https://user-images.githubusercontent.com/88039287/170450128-7bccdcf2-7e3d-40a5-97e1-0080989e8aac.jpg)

  ![cocot46plus_bg_02_2](https://user-images.githubusercontent.com/88039287/170451293-cf59e7ae-fea7-4a7d-95c5-4da1931f9df6.jpg)


### 3. アンダーグロウLED

  ver1.0以降は予め基板にはんだ付けされているので、アンダーグロウLEDのはんだ付けは不要です。


### 4. ProMicro

  ProMicroの準備をします。写真の向きでコンスル―をはんだ付けします。  
  コンスル―には向きがあるので注意してください。コンスル―の向きについては[こちら](https://yushakobo.zendesk.com/hc/ja/articles/360044233974-%E3%82%B3%E3%83%B3%E3%82%B9%E3%83%AB%E3%83%BC-%E3%82%B9%E3%83%97%E3%83%AA%E3%83%B3%E3%82%B0%E3%83%94%E3%83%B3%E3%83%98%E3%83%83%E3%83%80-%E3%81%AE%E5%8F%96%E3%82%8A%E4%BB%98%E3%81%91%E6%96%B9%E3%82%92%E6%95%99%E3%81%88%E3%81%A6%E4%B8%8B%E3%81%95%E3%81%84)を参照ださい。  
  USB Type-C版のProMicroにも対応しています。マイクロUSBの場合、USBコネクタがもげやすいので、適宜補強をしてからはんだ付けを行ってください。

  ![cocot46plus_bg_04_1](https://user-images.githubusercontent.com/88039287/170452185-4f523c38-248c-4b8d-87d4-889d6da17bf8.jpg)

### 5. マウスセンサー

#### 5-1. ADNS-5050
  マウスセンサー（ADNS-5050）を基板裏面から写真の向きに設置し、表面からはんだ付けを行います。シルクの●●印と基板の●●印の位置が合うように注意してください。  
  ![cocot46plus_bg_05_1](https://user-images.githubusercontent.com/88039287/170453958-e58aca65-1f71-4da0-9e0e-cbbb40e56425.jpg)

  センサーの脚がしっかり奥まで入った状態で、浮かないようにマスキングテープなどで固定します。  
  ![cocot46plus_bg_05_2](https://user-images.githubusercontent.com/88039287/170454505-65b0aa78-7d06-4c31-b2ab-bc4f62f97776.jpg)

  表面から8本の脚をはんだ付けします。  
  ![cocot46plus_bg_05_3](https://user-images.githubusercontent.com/88039287/170454245-9da5e45f-c8a4-41ba-87e1-4c37c676beb9.jpg)

  センサーに貼られているテープを剥がし、表面からレンズを付けてマスキングテープなどで固定します。  
  ![cocot46plus_bg_05_4](https://user-images.githubusercontent.com/88039287/170454912-ce859541-987f-4614-9b10-c68802e6cfbf.jpg)

#### 5-2. センサー用LED

  マウスセンサー用LEDを取り付けます。基板裏面からLEDの脚を通します。脚の長い方を丸い穴、短い方を四角い穴に通します。  
  ![cocot46plus_bg_05_5](https://user-images.githubusercontent.com/88039287/170455005-ff9d7af7-7d88-41b9-badc-025330ba14ea.jpg)

  LEDの脚を90度曲げ、横から見た時に下の写真のような位置関係になるようにマスキングテープなどで固定します。  
  ![cocot46plus_bg_05_5_2](https://user-images.githubusercontent.com/88039287/170455581-06e7b4f3-395c-44a6-93ec-c8fb8e6215e4.jpg)

  表面からLEDの脚を2箇所はんだ付けし、余分な脚をカットします。  
  ![cocot46plus_bg_05_6](https://user-images.githubusercontent.com/88039287/170455780-9cd94127-6efa-4838-9992-78e39cf6972e.jpg)

#### 5-3. ジャンパー

  基板裏面のジャンパーの両側のパッドにはんだを盛り、ブリッジさせます。  
  ![cocot46plus_bg_05_7](https://user-images.githubusercontent.com/88039287/170455922-7b17c4ca-8e60-4abd-8a33-edb597827bff.jpg)

  ![cocot46plus_bg_05_8](https://user-images.githubusercontent.com/88039287/170455929-1655e25f-8b99-49c7-b6f9-6a1d540ee2c3.jpg)

  ここまでの作業が完了したら、ProMicroに後述のファームウェアを書き込み、動作確認を行いましょう。正しい手順を踏めている場合、全部で12個のLEDとマウスセンサー用LEDが点灯しているはずです。  
  ![cocot46plus_bg_05_9a](https://user-images.githubusercontent.com/88039287/170456116-d3602e8f-aa3c-4f3c-8777-1d4b63a35322.jpg)

  表面のレンズの前に手をかざし、マウスカーソルが動いているか確認してみてください。  
  ![cocot46plus_bg_05_9b](https://user-images.githubusercontent.com/88039287/170456125-8737a304-75ed-45ea-8600-f5e00ac87531.jpg)

### 6. MXソケット

  PCB裏面に、写真の向きでソケットをはんだ付けします。**全46箇所**はんだ付けを行ってください。

  ![cocot46plus_bg_06_1](https://user-images.githubusercontent.com/88039287/170466184-43520998-4b82-4081-b9e0-286dcfd2c209.jpg)

### 7. OLED

  OLEDピンソケットを表側から挿し、マスキングテープなどで固定します。  
  ![cocot46plus_bg_07_1](https://user-images.githubusercontent.com/88039287/170467680-c5bf1d65-fe7e-406b-a933-91ee3e93b58d.jpg)

  ![cocot46plus_bg_07_2](https://user-images.githubusercontent.com/88039287/170467910-3b9ef4bc-dfab-4c57-ae40-404f63fd76a6.jpg)

  基板裏側からピンソケットの脚4本のはんだ付けを行ってください。  
  ![cocot46plus_bg_07_3](https://user-images.githubusercontent.com/88039287/170468810-e113a686-0350-4d38-ba71-02273a7c83d9.jpg)


  OLEDモジュールにピンヘッダを通し、斜めにならないように1本ずつはんだ付けを行います。  
  ![cocot46plus_bg_07_4](https://user-images.githubusercontent.com/88039287/170474570-298a2c45-4f1e-40e6-a35a-7291a0f67d20.jpg)


### 8. タクトスイッチ

  PCB表面に、タクトスイッチ（リセットスイッチ）を取り付け、裏面からはんだ付けします。1箇所のみです。  
  ![cocot46plus_bg_08_1](https://user-images.githubusercontent.com/88039287/170474668-4fefb8fe-1c71-49c3-8657-79d88a92d53a.jpg)


### 9. ロータリーエンコーダ

  中央部分にロータリーエンコーダをはんだ付けします。ロータリーエンコーダの脚を通し、裏側からはんだ付けをしてください。  
  ![cocot46plus_bg_09_1](https://user-images.githubusercontent.com/88039287/170474731-cd817ef7-662f-4d09-a309-c73f993b37d9.jpg)

  ![cocot46plus_bg_09_2](https://user-images.githubusercontent.com/88039287/170474739-0a417432-8ab3-463f-8600-5ee963c2c427.jpg)


  全てのパーツを付け終わった状態です。  
  ![cocot46plus_bg_09_3](https://user-images.githubusercontent.com/88039287/170474753-b494944c-e7c3-4953-a648-0b03a9f9392f.jpg)

  ![cocot46plus_bg_09_4](https://user-images.githubusercontent.com/88039287/170474767-5a647ab8-ec9e-475e-a5a2-dbfa7f804846.jpg)

### 10. キースイッチ

  トッププレートにキースイッチをはめ込みます。

  ![cocot46plus_bg_10_switch](写真追加)

### 11. 組み立て

  To be updated.

  ![cocot46plus_bg_11_assembly](写真追加)


## ファームウェア

  [REMAP](https://remap-keys.app/catalog/JPk6Ey9xB6yrr5TDqoLh/firmware)からファームウェアのダウンロードおよびProMicroへの書き込みを行うことができます。キーマップは[こちら](https://remap-keys.app/configure)から更新可能です。  
トラックボール、LED含めて上記.hexファイルで確認いただけます。

（.hexファイルをQMK ToolboxなどでProMicroに書き込む従来の方法でも問題ありません。）


![REMAP](https://user-images.githubusercontent.com/88039287/169829273-3694b209-59a6-4906-a8a7-2debab667cdf.jpg)


組み立て段階で動作確認をする際も、REMAPのTest Matrix Modeを使うと便利です。

ソースコードは[こちら](https://github.com/aki27kbd/qmk_firmware/tree/master/keyboards/cocot46plus)を参照ください。  
また、VIA用のjsonファイルは[こちら](https://github.com/aki27kbd/cocot46plus/blob/main/firmware/cocot46plus_via.json)を参照ください。


## カスタムキーコード

  トラックボールの操作に関していくつかカスタムキーコードを設定することが可能です。

  Value    | Keycode   |Description
  ---------|-----------|-----------
  `0x5DA7` | `CPI_SW`  |トラックボールのCPIを変更します。デフォルトのファームウェアでは、押すたびに500→750→1000→1250→500…という順番でCPIが変わります。
  `0x5DA8` | `SCRL_SW` |スクロールモードにおけるセンサーの感度を変更します。数値が大きいほどスクロール量が小さくなります。
  `0x5DA9` | `ROT_R15` |マウスセンサーのＹ軸を時計回りに15度回転させます。
  `0x5DAA` | `ROT_L15` |マウスセンサーのＹ軸を反時計回りに15度回転させます。
  `0x5DAB` | `SCRL_MO` |押されている間スクロールモードになります。
  `0x5DAC` | `SCRL_TO` |押すたびにスクロールモードとマウスモードを切り替えます。
  `0x5DAD` | `SCRL_IN` |スクロール方向を反転させます。

  REMAPでカスタムキーコードを設定する場合は下記の画面のようにCUSTOMから上の表のValueを直接入力してください。

  ![CustomKeycode](https://user-images.githubusercontent.com/88039287/169856477-84ebf6bb-9430-44f8-a650-537ab8f0a79b.jpg)


## OLED

  OLEDにはトラックボールの情報を表示することが可能です。  
  ![cocot46plus_bg_oled_1](https://user-images.githubusercontent.com/88039287/170496379-0b8dcec6-afac-48e9-b727-ad647c4a09c9.jpg)

  OLED|Description
  ---------|-----------
  Current Layer|現在のレイヤーを示します。
  Scroll Status|C:カーソル/S:スクロールモードを示します。
  CPI|カーソルモードのCPIを示します。
  Scroll Divider|スクロールモードにおけるセンサーの感度を示します。数値が大きいほどスクロール量が小さくなります。
  Rotation Angle|マウスセンサーのY軸の回転角を示します。

  手の大きさやトラックボールへの手の置き方によって、操作しやすいY軸の回転角が異なります。`ROT_R15`、`ROT_L15`キーで調整しながら自分に合った設定を探してみてください。  
  ![cocot46plus_bg_oled_2_2](https://user-images.githubusercontent.com/88039287/170499867-b430839b-f2f0-4163-afa2-c227184bd697.jpg)

  ![cocot46plus_bg_oled_3_4_5](https://user-images.githubusercontent.com/88039287/170501028-10d08bdd-df0f-406f-9b7f-14e1f0d8a726.jpg)



## 終わりに
何かトラブルがあれば[Twitterアカウント](https://twitter.com/aki27kbd)までご連絡ください。

また、完成写真をSNSにアップいただけるととても励みになります。（アップするのがはばかられる方はDMで直接送りつけていただいても構いません。）

ハッシュタグは #cocot46plus です。