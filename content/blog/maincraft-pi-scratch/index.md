---
title: raspberry piでのマイクラッチの設定
date: "2021-04-03T00:32:03"
---
Windowsでは何故か上手くいかないので、  
raspberry piで設定してみました。   
  
ダウンロードする物さえ間違えなければ、あっさり動作します。   
Raspberry Pi OSのフルバージョンならOKです。   

オフィシャルサイトの場合は  
OK：[Raspberry Pi OS with desktop and recommended software](https://downloads.raspberrypi.org/raspios_full_armhf/images/raspios_full_armhf-2021-03-25/2021-03-04-raspios-buster-armhf-full.zip)  
NG：[Raspberry Pi OS with desktop](https://downloads.raspberrypi.org/raspios_armhf/images/raspios_armhf-2021-03-25/2021-03-04-raspios-buster-armhf.zip)  

ダウンロードしたファイルを
[Etcher for Windows](https://www.balena.io/etcher/)
でmicro SDに書き込み


すでにscratchとminecraft-piはインストールされているが  
アップデートの意味も含めてコマンドを実行

```
sudo apt update && sudo apt upgrade -y
sudo apt-get install scratch minecraft-pi tuxtype -y
curl http://scratch2mcpi.github.io/install.sh | sh
```

minecraft-piを起動後にワールド作成してスタートしたら  
タブキーを押しScratch2MCPIを起動  
scratchとterminalが起動したら、scratchの旗ボタンをクリックして  
「hello minecraft」と表示されたらOKです。  

テストを実行
[Scratch2MCPI](http://scratch2mcpi.github.io/)