---
layout: post
title: Folding@home(FAH)を使って新型コロナウイルスやガンを解析
categories: Folding@home
image: https://newscast.jp/attachments/E6EZAO3dyveSk5kHMldG.png
highlight: false
author: okaits#7534
---
<!-- MarkDown Settings -->
<script src="https://taisukef.github.io/marked_md/marked.min.js">
<!-- /Markdown Settings -->
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
 <h1>TL;DR</h1>
今回は、<a href="https://foldingathome.org">Folding@home(FAH,F@H)</a>を使って、新型コロナウイルスやガンなどを解析します。<br>
<h1>インストール</h1>
<h2>Windowsの場合</h2>
Windowsの場合、<a href="https://download.foldingathome.org/releases/public/release/fah-installer/windows-10-32bit/v7.6/fah-installer_7.6.21_x86.exe">ここ</a>からFolding@homeのインストーラーをとってきます。<br>
そしたら、fah-installer_7.6.21_x86.exeがダウンロードされると思います。<br>
そしたら、それを起動して、初期設定のままで最後までいき、インストールします。<br>
<h2>Ubuntuの場合</h2>
Ubuntuの場合、<a href="https://download.foldingathome.org/releases/public/release/fahclient/debian-stable-64bit/v7.6/fahclient_7.6.21_amd64.deb">ここ</a>からインストーラーをとってきます。<br>
そしたら、CtrlとAltとTを同時に押し、ターミナルを開き、<br>
cd ダウンロードしたディレクトリ<br>
<script>md(`
```
sudo apt install ./fahclient_7.6.21_amd64.deb
```
`)</script>
を実行します。<br>
途中で質問されたら、全てEnterを押してください。
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
<h1>初期設定</h1>
インストールが終わったら、<a href="https://client.foldingathome.org">ここ</a>を開きます。<br>
すると、<img src="https://pc.watch.impress.co.jp/img/pcw/docs/1243/458/03.png">このような画面が表示されます。<br>
そしたら、Set up an identifyを選択し、Start Foldingを押します。<br>
<h2>ただ単に貢献だけをしたい人</h2>
貢献をして、ポイント（換金不可(例外あり)）とかはいらない人は、<br>
User: 2x3m7aufjcj7<br>
Team Number: 234980<br>
Passkey: 無し<br>
にしてください。<br>
なお、この設定だとポイントはokaitsの方に入っていきます。<br>
<h2>自分の名前で貢献したい人</h2>
ポイントを自分でためたり、自分の名前（ニックネーム）で貢献したい人は、<br>
User: 自分で決めたユーザー名<br>
Team Number: 1061846<br>
<h2>自分のチームで貢献したい人</h2>
自分が作ったチームで貢献したい人は、<a href="https://apps.foldingathome.org/team">ここ</a>からチームを作ります。<br>
作り終わったら、Team Numberが出てくるので、<br>
User: 自分で決めたユーザー名<br>
Team Number: 登録時に出てくる数字<br>
<br>
で、登録してください。<br>
登録が終わったら、自動的に貢献が開始されます。<br>
なお、linuxでは、再起動時に貢献が自動的に開始されません。<br>
開始されるようにしたい場合、<br>
<script>md(`
```
sudo systemctl enable FAHClient
sudo systemctl start FAHClient
```
`)</script>
を実行してください。
