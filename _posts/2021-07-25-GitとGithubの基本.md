---
layout: post
title: GitとGithubの基本
categories: git
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
<h1>Commit</h1>
Commitとは、レポジトリに変更を反映することです。<br>
<h1>Clone</h1>
Cloneとは、リモートレポジトリ（Githubなどにあるレポジトリ）から自分のハードディスクにダウンロードすることです。<br>
<h1>Pull</h1>
Pullとは、一度Cloneしたレポジトリに、リモートレポジトリの変更を適用させることです。<br>
<h1>Push</h1>
Pushとは、一度Cloneしたレポジトリに加えた変更を、リモートレポジトリに適用させることです。<br>
なお、これをする前に、Commitしないと変更とみなされません。<br>
<h1>Pull Request(PR)</h1>
PRとは、Githubで、リモートレポジトリの編集権限がないときに、管理者に編集をリクエストすることです。<br>
また、管理者が他の管理者に変更していいかを確認する時もPRは使われます。<br>
<h2>Merge</h2>
PRを管理者が承認することです。<br>
<h1>Fork</h1>
Forkとは、Githubで、他の人のレポジトリをコピーして自分が自由に変更できるものです。<br>
PRでも使われます。<br>