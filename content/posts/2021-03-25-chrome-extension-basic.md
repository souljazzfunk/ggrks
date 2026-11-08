---
title: "【超入門】Google Chrome拡張機能の基礎と実践【ゼロ初級】"
date: "2021-03-25 18:44:05"
categories:
  - "#ほぼ週刊ググレカス"
  - "chrome extensions"
  - "EdTech"
permalink: "https://laiken.net/ggrks/chrome-extension-basic/"
tags:
  - "Chrome"
  - "chrome extension"
  - "Chrome extensions"
  - "Chrome拡張機能"
  - "google"
  - "キーボードショートカット"
  - "グーグル"
  - "クローム"
  - "クローム拡張機能"
  - "ライフハック"
  - "情報リテラシー"
  - "情報教育"
  - "拡張機能"
  - "時短"
  - "業務効率化"
url: "/chrome-extension-basic/"
image: "images/banners/2021/03/b1908d351571bcdf9bbe330072cfab3c.png"
---

あまりコンピュータやインターネットに詳しくない人に向けて、[Google Chrome拡張機能について説明したり、便利なものを紹介する機会](https://www.youtube.com/watch?v=pdk1Zz-ewQw&t=580s)を頂きました。イベントの予習・復習用に本稿をお役立て頂ければ幸いです！

## Google Chrome（グーグル・クローム）とは

まずはChromeとは何か？から説明します。

以下、できるだけ平易な言葉で説明を試みます。小難しい説明や専門用語を読みたくない人は、**色のついた囲み記事だけを読めばOK**です！では、わかりやすさを優先するため正確性を欠いた表現をしますが、あしからず。

Chromeとは、グーグルという会社が作っている、インターネットを見るためのプログラムです。他にも別の会社が同じようなプログラムを作って競争していますが、本稿執筆時点ではGoogle Chromeが世界で一番多く使われています。

ここで、「インターネットを見るためのプログラム」のことを「web browsers（ウェブブラウザ）」と呼びます。このブログでもよく出てくる用語なので、覚えておきましょう。

では、すこし専門用語や固有名詞が分かる人むけの説明です。読まなくても大丈夫。

Chromeとは、Googleが提供するWebブラウザで、PC以外にもスマホやタブレット等で利用できるアプリが無料で配布されています。Webブラウザは、AppleのSafariやMicrosoftのEdgeのように他社からも同様のものが提供されていて、シェア争いが続いています。本稿執筆時点ではGoogle Chromeが世界で一番多く使われています。

### Chromeの何が凄いのか

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-22-1-1024x551.jpg)

*Google Chrome発表当時の公式ブログ記事。昔のGoogleロゴが渋い！*

もう少し詳しく。読まなくていいです。笑

Microsoft Internet Explorerの勢いが鈍り、Mozilla Firefoxが台頭していた2008年、Googleは新しいWebブラウザとしてChromeを発表しました。AppleのWebkitエンジンやFirefoxのコンポーネント等を利用してオープンソースプロジェクトとして開発されたChromeは、その洗練された簡素なインタフェイスやページ読み込みの速さで他のブラウザを圧倒し、瞬く間に主流のWebブラウザとなりました。特に当時Internet Explorerが実現できなかったWeb規格への準拠や、「サンドボックス」と呼ばれる仕組みによるクラッシュ耐性などがWeb技術に革命を起こしたとされ、発表後10年以上たった今でもブラウザ市場を席巻しています。

## Chrome extensions（クローム拡張機能）とは

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-22-1024x353.png)

では今回の本題であるChrome拡張機能とはなんでしょう？

クローム拡張機能は小さなプログラムのことです。この小さなプログラムを使えば、クロームにもともと備わっていない機能を追加して、インターネットをより便利に見ることができます。

Chromeの拡張機能は小さなプログラムのことで、ウェブの閲覧（ブラウジング）体験をカスタマイズするためのものです。拡張機能はHTMLやCSS、javascriptといったウェブ技術で作られており、ユーザはChromeの機能や挙動を自分の好みに仕立て上げることができます。

### すべて無料

本稿執筆時点で入手できるChrome拡張機能は、すべて無料です。  
（[2020年9月に、Chrome Web Storeにおける課金廃止がアナウンスされました](https://developer.chrome.com/docs/webstore/cws-payments-deprecation/)）

### Googleが作っているとは限らない

いまやGoogle Chromeというブラウザはひとつの生態系となっており、その上で動く小さなプログラムを提供する個人や企業がたくさんいます。つまり、Google社が提供する拡張機能もあれば、そうでないものもあります。

すべての拡張機能は公開前にGoogleによって審査されますが、中には怪しげなものもあります。注意しましょう。

### 動くのはパソコン上のみ

基本的には、スマホやタブレット用のブラウザでは拡張機能は動きません。（例外はあります）

### Google Chrome以外でも使える

これは意外と知られていないかもしれません。Google Chromeがメインのブラウザではない人も、Chrome用の拡張機能を転用したり、または同等の機能を持ったそのブラウザ専用の拡張機能を使うことができます。すべての拡張機能がすべてのブラウザで動くわけではありませんが、例えば下記のようなブラウザでは、たいていの拡張機能が使えるようです。

- Firefox
- Safari
- Brave
- Edge
- Opera
- Linux用のブラウザ各種

## 拡張機能をインストールする

正体がわかったところで、さっそくパソコンのChromeに拡張機能をインストールしてみましょう。

[公式ドキュメント](https://support.google.com/chrome_webstore/answer/2664769?hl=ja&ref_topic=6238977)を読めば誰にでも？できなくはないのですが、画像もないし分かりにくいので、スライドを作りました。例として今回は、Google Arts & Culture という拡張機能を一緒にインストールしてみましょう！

<iframe allowfullscreen="true" frameborder="0" height="569" mozallowfullscreen="true" src="https://docs.google.com/presentation/d/e/2PACX-1vQXJ8LM3aQkmRCsBG-a3OIfNKJJQzlIn2eErZ9xGQOsmOca3TX6GEQonMkGutYZ8NKvGHahinqAK2XA/embed?start=false&amp;loop=false&amp;delayms=3000" webkitallowfullscreen="true" width="960"></iframe>

## 拡張機能の使い方

拡張機能は多種多様です。世界中のプログラマー達が技術の粋を集めて作ったものから、その辺のオタクが趣味で作った全く意味のわからないもの、ちゃんと動かないものまで千差万別なので、それぞれ使い方が違います。簡単に分類します。

### インストールするだけでいいもの

これはインストールするだけで、あなたが何かをする必要はありません。先ほどのスライドで例としてインストールした Google Arts & Culture がそのいい例で、これはブラウザの新規タブやウインドウを開いた時に世界の名画を見せてくれます。

### クリックして使うもの

たいていの拡張機能は、このスタイルのものです。クリックするとメニューが開いたり、ブラウザの画面内に表示が出たりします。便利なボタンがひとつ増えたぞ、みたいな感覚で使えます。

### キーボードショートカットで使うもの

キーボードからの操作を前提としたものもあります。ブラウザのタブやウインドウを操作するものや、Googleの検索画面やGoogleドキュメントに機能を追加するものにこのスタイルが多いです。

### 他のサイトと連動するもの

ログインが必要なものが多いです。わざわざ他のサイトを開いて別タブで作業する手間を省くために、ブラウザのメニューから小さなウインドウを出して操作ができるようなものが多いです。

## Chrome拡張機能をたくさん入れるとパソコンの動作が重くなる？

![](https://laiken.net/ggrks/wp-content/uploads/2021/04/image-4.png)

初心者から最も多い質問の一つがこれです。結論から言うと、Google Chromeの動作が遅くなる可能性が高いです。機能が重複するものをインストールした場合は、比較検討して不要なものは削除するか、設定画面でOFFにしておきましょう。  
  
拡張の機能の設定画面を開くには、  
右上にある「点が3つ縦に並んだ」アイコン（![その他](https://lh3.googleusercontent.com/E2q6Vj9j60Dw0Z6NZFEx5vSB9yoZJp7C8suuvQXVA_2weMCXstGD7JEvNrzX3wuQrPtL=w36-h36)） ![次に](https://lh3.googleusercontent.com/SaY5lqCwN7kppnS546l9ys-E2sZftTTIHjBrdV-WsGPIhGjaxcEXjfgdIfW_UNG7Sw0=w26-h36) [**その他のツール**] ![次に](https://lh3.googleusercontent.com/SaY5lqCwN7kppnS546l9ys-E2sZftTTIHjBrdV-WsGPIhGjaxcEXjfgdIfW_UNG7Sw0=w26-h36) [**拡張機能**] をクリックします。

厳密には拡張機能の「数」が問題なのではなくて中身の問題ですが、確率論として沢山インストールすればそれだけ「重いやつ」に当たりやすくなる、ということだと思います。とは言え、数百とか数千の拡張機能をインストールすれば、やはりそれなりにChromeの起動などに（著しく）影響し始めると思います。

## 「教師のためのChrome拡張機能スターターパック」リンク集

![教師のためのChrome拡張機能スターターパック](https://laiken.net/ggrks/wp-content/uploads/2021/03/banner_CE_starter_pack.png)

拡張機能ソムリエ、らいけんが調査と実験を重ねてリストアップした、「とりあえずこれを入れておけば授業準備も授業中も何とかなるだろう」という選り抜きの拡張機能リンク集です。「教師のための」と銘打っていますが、どんな仕事にも役に立つものばかりですので、ぜひ使ってみてください！

このリンク集は、3月27日開催の無料イベント「[Zoomで実践シェア会 第10弾 〜Google拡張機能で授業を楽しく！時短テク！〜](https://twitter.com/mocchee_HK/status/1372938769087664136)」のオープニングセッションでお配りします！見に来てね。

### 「Zoomで実践シェア会」お申し込みはこちら！

**Zoomで実践シェア会 申込みフォーム（無料）**

2021年3月27日（土）21:00〜22:30（香港時間 UTC+8)   
[各地域のタイムゾーンで開催時刻を確認する](https://bit.ly/38sGFlc)

開催日時は香港時間です。日本の22時スタートです。

追記：シェア会へのご参加ありがとうございました！[当日の録画が公開されています](https://www.youtube.com/watch?v=pdk1Zz-ewQw&t=580s)ので、以下の記事とあわせてご覧ください。

https://laiken.net/ggrks/10-chrome-extensions-for-teachers/

## 参考文献

- [Google’s Chrome browser is now 10 years old](https://www.theverge.com/2018/9/2/17811844/google-chrome-browser-10-years-history). (2018). Retrieved 16 March 2021, from https://www.theverge.com/2018/9/2/17811844/google-chrome-browser-10-years-history
- [Official Google Blog: A fresh take on the browser](https://web.archive.org/web/20080902000920/https://googleblog.blogspot.com/2008/09/fresh-take-on-browser.html). (2008). Retrieved 16 March 2021, from https://googleblog.blogspot.com/2008/09/fresh-take-on-browser.html
- [拡張機能をインストールして管理する - Chrome ウェブストア ヘルプ](https://support.google.com/chrome_webstore/answer/2664769?hl=ja&ref_topic=6238977). (2021). Retrieved 16 March 2021, from https://support.google.com/chrome_webstore/answer/2664769?hl=ja&ref_topic=6238977
