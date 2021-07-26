---
layout: post
title: Raspberry PiでiSCSIターゲットを構築する方法
categories: iSCSI
highlight: false
disqus: true
image: https://images-na.ssl-images-amazon.com/images/I/41cLQXPYZEL._AC_.jpg
author: okaits#7534
---

   <!-- EthereumAds -->
   <div id="EthereumAds-linuxcodevblog"></div>
   <script src="https://ethereumads.com/adviewer.js">
   </script>
   <script>
       EthereumAds.initAdSlot({
           acceptedCurrencies: ["ALL"], // option ALL for all whitelisted tokens, ETH for Ethereum, DAI for DAI Stablecoin
           //validatorEndpoint:"", // optional custom validator
           mediaType: "image_320x50",
           fallback: "default", // default, none, custom url
           slot: "linuxcodevblog",
           address: "0xd404f198c4f580727eb11cd69b581d5f10c7efd9",
           platform: "",
           affiliate: "",
           keywords:"", //comma separatedy
           adult: false,
           version: "1.00"
       });
       /*
        for responsive ads add and adjust this according to your needs:
        responsive: [
            { mediaType: "image_728x90", minWidth: 728 },
            { mediaType: "image_300x600" }
        ],
       */
   </script>
   <!-- /EthereumAds -->  

# TL;DR
<hr>
今回は(初投稿）、iSCSIターゲットを構築する方法を書きます！<br>

# 作業
<hr>
## Step 1 Raspberry Pi OSをインストール
では、Raspberry PiにRaspberry Pi OSをインストールします....が、ここで解説していると記事が長くなってしまうので、<a href="https://jellyware.jp/kuragemd/raspi/raspberrypi.html">他の人の記事</a>を参考にしてください。<br>

## Step 2 OMVのインストール
では、OMVをインストールしてみましょう。<br>
OMVとは、ファイルやハードディスクを共有することに特化したソフトウェアです。<br>
インストールが終わったら、CtrlとAltとTを同時に押し、ターミナルを開き、次のコマンドを実行してください。<br>
<code>
wget https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install <br>
sudo bash install <br>
</code>
これが終わったら、再起動し、<br>
<a href="http://raspberrypi.local"></a>を開きます。<br>
なお、このリンクはRapsbery Piが起動していて、なおかつ同じWi-Fiに接続しているときにしかアクセスできません。<br>
そうすると、ログイン画面が出てきます。<br>
ユーザー名：　admin <br>
パスワード：　openmediavault <br>
でログインしてください。<br>
そして、メニューの<br>
plugin <br>
を押し、openmediavault-tgtをインストールしてください。<br>
そして、メニューの<br>
Service <br>
をクリックし、tgtを開きます。<br>
そうして、最後にTargetの名前を入力して、保存してください。<br>
それで完成です。<br>
## iqn
iqnは、iqnはiqn.作成した年-作成した月.raspberrypi:設定した名前<br>
です。<br>
  <!-- EthereumAds -->
   <div id="EthereumAds-linuxcodevblog"></div>
   <script src="https://ethereumads.com/adviewer.js">
   </script>
   <script>
       EthereumAds.initAdSlot({
           acceptedCurrencies: ["ALL"], // option ALL for all whitelisted tokens, ETH for Ethereum, DAI for DAI Stablecoin
           //validatorEndpoint:"", // optional custom validator
           mediaType: "image_320x50",
           fallback: "default", // default, none, custom url
           slot: "linuxcodevblog",
           address: "0xd404f198c4f580727eb11cd69b581d5f10c7efd9",
           platform: "",
           affiliate: "",
           keywords:"", //comma separatedy
           adult: false,
           version: "1.00"
       });
       /*
        for responsive ads add and adjust this according to your needs:
        responsive: [
            { mediaType: "image_728x90", minWidth: 728 },
            { mediaType: "image_300x600" }
        ],
       */
   </script>
   <!-- /EthereumAds -->  
