# ライセンス
このブログは
<img src="https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png">
でライセンスされていますが、Apache Licence 2.0でライセンスされている部分もあります。
  

## 記事の書き方
記事の書き方です。  
まず、gh-pagesブランチの中の_postsディレクトリの中に、  
**yyyy-mm-dd-タイトル.md**  
という名前のファイルを作ります。  
そしたら、中に  
一番下に記述したコードを入れます。  
そうして、その後に<b>HTMLで</b>本文を書き始めてください。(brタグを忘れないようにする。)  
本文を書き終えたら、PRを作成してください。（直接CommitもOK)  

### テンプレートコード
```md

---
layout: post
title: ブログのタイトル
categories: ブログのカテゴリ（ない場合この行は省略可能）
image: 記事の画像（ない場合この行は省略可能）
highlight: false
disqus: true
author: 記事を書いた人のDiscordユーザー名とタグ（例：okaits#7534）
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
```
