---
title: "【かんたん】Googleスライドのサムネイル表示／非表示を切り替える！【拡張機能不要】"
date: "2021-03-12 06:54:00"
categories:
  - "#ほぼ週刊ググレカス"
  - "chrome extensions"
  - "EdTech"
permalink: "https://laiken.net/ggrks/toggle-gslides-thumbnail/"
tags:
  - "Chrome"
  - "google"
  - "Google Slides"
  - "Googleスライド"
  - "PowerPoint"
  - "キーボードショートカット"
  - "グーグル"
  - "クローム"
  - "スライド"
  - "プレゼン"
  - "ライフハック"
  - "情報リテラシー"
  - "情報教育"
  - "時短"
  - "業務効率化"
url: "/toggle-gslides-thumbnail/"
image: "images/banners/2021/03/2baac19ff85737c9991a2eb0cdf220df.png"
---

好評を頂いた[前回の記事](https://laiken.net/ggrks/fullscreen-interactive-google-slides/)で質問が多かった「サムネイル消えたのはいいけど、元に戻らないじゃん」という問題の解決方法がわかりましたのでご紹介です。手っ取り早いのはタブをリロードすることですが、スライドが何十枚もあると時間がかかってしまいます。そこで、下記でご紹介する方法をおすすめします！

## すぐ終わる手順！

1. [Toggle Thumbnail Pane](javascript:(function() %7Bvar e%3Ddocument.getElementsByClassName(%27filmstrip%27)%5B0%5D%3Be.style.display%3D(e.style.display!%3D%27none%27)%3F%27none%27:%27table-cell%27%3B%7D)()%3B) ←このリンクをブックマークにドラッグする！
2. [https://slide.new/](https://slide.new/) で新規Googleスライドを開く！
3. いま作ったブックマークをクリック！（サムネイル消えるはず）
4. もう一度クリック！（サムネイル戻るはず）

![Googleスライドのサムネイル表示／非表示を切り替える！](https://laiken.net/ggrks/wp-content/uploads/2021/03/Screen-Recording-2021-03-11-at-3.49.59-PM-00.00.00.000-00.00.02.052.gif)

**↑リンクを含んだテキストは、直接ドラッグできます！**

## レイアウトが変なときは、一度フルスクリーンにする

最初は「サムネイルは消えたんだけど、なんかスライド部分が右に寄ったままで、大きさ変わらないよ！」という状態だと思います。この状態で、一旦ブラウザの機能でフルスクリーンにしてみましょう。

**Google Chromeをフルスクリーン表示にする**

[Mac] ⌘ + Ctrl + f  
[Win] Alt + Ctrl + f、または F11

Windowsのショートカットについては、ちょっと自信がありません。間違ってたら教えて下さい！

フルスクリーンにするとスライドの大きさ、レイアウトともにいい具合に落ち着くと思います。そしたらもう一度ショートカットを押して、編集モードに戻ります。これで完了です。

## フルスクリーンにしないで、サムネイルの表示だけを切り替えられる

このブックマークレットが[前回の拡張機能](https://laiken.net/ggrks/fullscreen-interactive-google-slides/)よりも優れているのは、いちいちフルスクリーンモードが発動しないことです。これによって、

- ブラウザのフルスクリーンのON/OFF
  と、
- サムネイルの表示／非表示

の組み合わせを、好きなように切り替えられるようになります。例えばフルスクリーン編集モードで授業中に、ちょっとだけサムネイルが見たくなったらブックマークレットをクリックして、用が済んだらまた消しておく、といった使い方です。

## 動作が軽快！気軽に使える

このブックマークレットはjavascriptでCSSの表示を制御しているだけなので、押しまくってもコンピュータやネットワークに高い負荷がかかることはありません。

## 参考文献

こちらで既出の問題でした。ググれよ、然らば与えられん。  
[https://webapps.stackexchange.com/questions/138746/how-do-i-hide-the-left-thumbnail-panel](https://webapps.stackexchange.com/questions/138746/how-do-i-hide-the-left-thumbnail-panel)

前回の記事はこちら。

https://laiken.net/ggrks/fullscreen-interactive-google-slides/
