[![BTO-logo](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/05/logo.png)](https://bit-trade-one.co.jp/)
# ファームウェアアップデート方法
ファームウェアはハードウェアの中に書き込まれているソフトウェアです。  
不具合修正や機能追加された新しいBFU2Sのファームウェアが公開された際、  
ファームウェアをアップデートすることで新しい機能が使用できます。  

## 1.準備
- __HIDBootLoader.exeを任意の場所にダウンロードしてください。__  
 [HIDBootLoader.exeダウンロードリンク](https://github.com/bit-trade-one/BFU2S-USBDualConnectCustomKeypad/raw/master/Firmware/HIDBootLoader.exe)   
  こちらは、Microchipが公開しているライブラリ「MCHPFSUSB」の中にある物と同一です。  
  HIDBootLoader.exeは.NET framework 2.0を用いて作成されています。
  HIDBootLoader.exeがうまく起動しない場合、MicrosoftのHP等からダウンロードし、インストールする必要があります。
  “Microsoft .NET framework”等のキーワードで検索を行い入手してください。  

- __BFU2Sの必要なファームウェアを任意の場所にダウンロードしてください。__  
(最新)[BFU2Sファームウェアダウンロードリンク(v001)](https://github.com/bit-trade-one/BFU2S-USBDualConnectCustomKeypad/raw/master/Firmware/BFU2S_v001full.zip)
  
## 2. ファームウェア書き込み
- __BFU2S設定ツール右下、ファームウェアアップデートよりBOOTモードにします。__  
![image](https://user-images.githubusercontent.com/85532743/169973945-58bb5562-a946-4bd4-a594-c87b252aa4d1.png)  

- __ファームウェアの書き換えウィンドウで「はい」を選択してください。本体がBOOTモードに入ります。__    
![image](https://user-images.githubusercontent.com/85532743/169974361-e444d12f-f16a-44c8-b4d0-2254f0bf1330.png)  

- __先程ダウンロードしたHIDBootLoader.exeを立ち上げてください。__    
![image](https://user-images.githubusercontent.com/85532743/170158526-76b20a94-d8ee-4429-b6af-8e27f3d92fe6.png)  
デバイスが認識されると上図の様に「Device attached」と表示されます。  
初めてBOOTモードで接続した時には、自動的にPCにドライバがインストールされます。（約１分程時間かかります） 
   
 
- __「Open Hex File」を押し、書き込みたいファームウェア(Hexファイル)を選択します。__  
![image](https://user-images.githubusercontent.com/85532743/169975424-6d0913f8-7b8a-43fa-84dc-eec7b0a77bd0.png)  

- __「Program/Verify」を押すとファームウェアが書き込まれます。__  
![image](https://user-images.githubusercontent.com/85532743/169975956-b5d252c5-158b-45fe-b4ad-20486a0c2c2f.png)  

- __「Erase/Program/Verify Completed Successfully」とウィンドウに表示され、緑のインジケータが最大になれば完了です。__    
USBケーブルを抜差しして再起動すると、ファームウェアが適応されます。
![image](https://user-images.githubusercontent.com/85532743/169977504-b4b4a0e0-5e7d-43fa-a13c-f173bf783330.png)

以上でファームウェアアップデートは完了です。


