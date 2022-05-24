[![BTO-logo](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/05/logo.png)](https://bit-trade-one.co.jp/)
# ファームウェアアップデート方法
ファームウェアはハードウェアの中に書き込まれているソフトウェアです。  
不具合修正や機能追加された新しいBFU2Sのファームウェアが公開された際、  
ファームウェアをアップデートすることで新しい機能が使用できます。  

## 1.準備
- ### HIDBootLoader.exeを任意の場所にダウンロードしてください。
   [HIDBootLoader.exeダウンロードリンク](https://github.com/bit-trade-one/BFU2S-USBDualConnectCustomKeypad/raw/master/Firmware/HIDBootLoader.exe) 


   こちらは、Microchipが公開しているライブラリ「MCHPFSUSB」の中にある物と同一です。  
   HIDBootLoader.exeは.NET framework 2.0を用いて作成されています。
   HIDBootLoader.exeがうまく起動しない場合、MicrosoftのHP等からダウンロードし、インストールする必要があります。
   “Microsoft .NET framework”等のキーワードで検索を行い入手してください。  

- ### BFU2Sの必要なファームウェアを任意の場所にダウンロードしてください。
   (最新)[BFU2Sファームウェアダウンロードリンク(v001)](https://github.com/bit-trade-one/BFU2S-USBDualConnectCustomKeypad/raw/master/Firmware/BFU2S_v001full.zip)
  
## 2. BOOTモード
- ### BFU2S設定ツール右下、ファームウェアアップデートよりBOOTモードにします。
![image](https://user-images.githubusercontent.com/85532743/169973945-58bb5562-a946-4bd4-a594-c87b252aa4d1.png)  

- ### ファームウェアの書き換えウィンドウで「はい」を選択してください。本体がBOOTモードに入ります。  
![image](https://user-images.githubusercontent.com/85532743/169974361-e444d12f-f16a-44c8-b4d0-2254f0bf1330.png)  

- ### 先程ダウンロードしたHIDBootLoader.exeを立ち上げてください。  
 ![image](https://user-images.githubusercontent.com/85532743/169975152-20120bc4-86d2-4408-8ef2-771e46ad56bd.png)  
 デバイスが認識されると上図の様に「Device attached」と表示されます。  
 初めてBOOTモードで接続した時には、自動的にPCにドライバがインストールされます。（約１分程時間かかります） 
   
 
 「Open Hex File」を押し、書き込みたいファームウェア(Hexファイル)を選択します。
 ![image](https://user-images.githubusercontent.com/85532743/169975424-6d0913f8-7b8a-43fa-84dc-eec7b0a77bd0.png)  

「Program/Verify」を押すとファームウェアが書き込まれます。
![image](https://user-images.githubusercontent.com/85532743/169975956-b5d252c5-158b-45fe-b4ad-20486a0c2c2f.png)  

「Erase/Program/Verify Completed Successfully」とウィンドウに表示され、緑のインジケータが最大になれば完了です。  
USBケーブルを抜差しして再起動すると、ファームウェアが適応されます。
![image](https://user-images.githubusercontent.com/85532743/169977504-b4b4a0e0-5e7d-43fa-a13c-f173bf783330.png)

以上でファームウェアアップデートは完了です。


