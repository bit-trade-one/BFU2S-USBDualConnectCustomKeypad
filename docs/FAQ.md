[![BTO-logo](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/05/logo.png)](https://bit-trade-one.co.jp/)
# BFU2S-よくある質問

## Q.2つのUSB端子間は絶縁されていますか

### A.はい。絶縁されております。

絶縁耐圧等の公開はしておりません。

## Q.設定ツールが反応しません。

### A.同時接続で無く、左右片方づつPCと接続し設定を行ってください。


![1台づつ接続してください](https://user-images.githubusercontent.com/85532743/169960442-45e18a9a-8fe2-4459-8532-6a263235ff17.png)  
詳しくは[設定ツールの使い方](SettingTool.md)ページをご覧ください。


## Q.PC以外の機器に接続したら反応しません。

### A.キーボードのみファームウェアをお試しください。  

BFU2Sはキーボード/マウス/ゲームパッドの 機能を持った複合デバイスのため、  
複合デバイスを認識できていない機器では使用できない事があります。  
  
そのような機器でBFU2Sを使用できるようキーボードのみとして振る舞う専用設定ツール・ファームウェアを用意しました。

- [キーボードのみ用設定ツール_BFU2S_CT_v900.exe クリックでダウンロード](https://github.com/bit-trade-one/BFU2S-USBDualConnectCustomKeypad/raw/master/App/KeyboardOnly/BFU2S_CT_v900.zip)  
- [キーボードのみ用ファームウェア_BFU2S_v901.hex クリックでダウンロード](https://github.com/bit-trade-one/BFU2S-USBDualConnectCustomKeypad/raw/master/Firmware/KeyboardOnly/BFU2S_v901.zip)  

キーボードのみモードで使用する場合  
キーボードのみの設定ツールと  
キーボードのみのファームウェアが書き込まれたBFU2Sが必要です。  
ファームウェアとはハードウェアの中に書き込まれているプログラムの事を指します。  

BFU2Sは左右それぞれのUSBに１つづつ独立したコンピュータを持っています。  
そのため、左右双方でキーボードのみ仕様にするには左右両方のファームウェアをアップデートする必要があります。  
ファームウェアアップデート方法は[こちら](FirmwareUpdate.md)に記載がございます。
上記をダウンロードして手順に従いファームウェアアップデートを行ってください。  
(キーボードのみファームウェアから元の複合デバイスに戻す場合、リンク先手順「2. ファームウェア書き込み」  
にて機器のBOOTモード化を記事上では「BFU2S設定ツール(BFU2S_CT_v100)」にて行っていますが  
こちらを「キーボードのみ用設定ツール_BFU2S_CT_v900.exe」で行うと読み変えてください。)

![内部説明](https://user-images.githubusercontent.com/85532743/178431549-345b9266-52a3-413d-985d-f7f0f4925fcc.png)
[クリックで拡大](https://user-images.githubusercontent.com/85532743/178431549-345b9266-52a3-413d-985d-f7f0f4925fcc.png)  
  
  
左右で別々のファームウェアを持たせることも可能ですが、設定時はファームウェアに合わせた設定ツールを  
ご使用ください。  

![キーボードのみ説明](https://user-images.githubusercontent.com/85532743/178428018-c94cb56f-0b8b-4205-af9c-bf50155bb82e.png)  
[クリックで拡大](https://user-images.githubusercontent.com/85532743/178428018-c94cb56f-0b8b-4205-af9c-bf50155bb82e.png)


