---
layout: post
title: UbuntuにGithub Desktopをインストールする
categories: Github
highlight: false
disqus: true
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

<h1>インストール</h1>
まず、<a href="https://github.com/shiftkey/desktop/releases/download/release-2.9.0-linux4/GitHubDesktop-linux-2.9.0-linux4.deb">ここ</a>からインストーラーをダウンロードします。<br>
そして、ターミナルで<br>
cd ~/ダウンロード<br>
sudo apt install ./GitHubDesktop-linux-2.9.0-linux4.deb<br>
と実行してください。<br>
<h1>初期設定の注意事項</h1>
途中でメールアドレスに謎のメールアドレスが入力されていますが、これはスルーです。<br>
<h1>使いやすいように設定</h1>
<ui>
<li>
Visual Studio Codeのインストール<br>
vscodeをインストールすると、Github Desktopからファイルを編集できます。<br>
vscodeのインストールはsnapからいけますが、日本語入力が使えなくなります。<br>
<a href="https://code.visualstudio.com/docs/?dv=linux64_deb">Microsoftの公式からダウンロード</a>してインストールします。<br>
ダウンロードしたら、<br>
cd ~/ダウンロード<br>
sudo apt install ./code*.deb<br>
を実行してください。<br>
</li>
<li>
GithubにPushできないのを改善する<br>
環境によりますが、Github DesktopでPushするときにエラーが出てくる可能性があります。<br>
解決策は、最もかんたんなのは、Pushを自動的に実行する.desktopファイルをデスクトップやDashに置くことです。<br>
Dashに置くことで、お気に入り登録もできます。<br>
やり方は、まず<br>
~/.local/share/applications/<br>
や<br>
~/デスクトップ/
<br>
に、<br>
<script src="https://gist.github.com/okaits/725da880b0113d36a5994b4375bc168b.js"></script><br>
を置くと、デスクトップやDashに登録できます。
<li>
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