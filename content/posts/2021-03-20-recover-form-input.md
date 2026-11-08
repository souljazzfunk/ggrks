---
title: "「せっかく書いた長文が消えちゃった！」を解決：フォーム入力を自動保存、回復できるChrome拡張機能"
date: "2021-03-20 15:16:03"
categories:
  - "#ほぼ週刊ググレカス"
  - "chrome extensions"
permalink: "https://laiken.net/ggrks/recover-form-input/"
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
url: "/recover-form-input/"
image: "images/banners/2021/03/Typio.jpg"
---

フォーム内容が消えてしまうことは多々あります。最近ノルディック方面の先生から聞いた話では、某LMSでは、ちょっと作業して、別のタブを見てから帰ってきたらもう作業内容が消えているそうです。すでに人類は、機械から意地悪される時代を迎えているのです。笑「また最初から書き直しぃぃぃぃぃ？」という悲劇が二度と起こらないよう、この拡張機能を使いましょう！

## [Typio Form Recovery](https://chrome.google.com/webstore/detail/typio-form-recovery/djkbihbnjhkjahbhjaadbepppbpoedaa)

[拡張機能をインストール](https://chrome.google.com/webstore/detail/typio-form-recovery/djkbihbnjhkjahbhjaadbepppbpoedaa)したら、まず使いたいタブをリロード（再読込み）するのをお忘れなく。

![](https://lh3.googleusercontent.com/00wGWdBCSf8L5u0XlYIVOQ5R0ANc1VZqZZQaP8RoTR8FX-GRa3vuljidiQgE9vLVKQXtBPc1uqa7guf2Xb_k91qe7KU=w640-h400-e365-rj-sc0x00ffffff)

インストールすると、このように入力フォームに青い時計のアイコンが表示され、そこからこれまでの入力履歴を見て、必要なものを復元することができます！場合によって、図のような小さなメニューが開く時と、検索可能な大きな画面が開くことがあります。

今後は、入力フォームでタイプしたものは自動保存されます。自動保存するかしないかはウェブサイト毎に設定可能です。保存期間は初期設定では30日間で、これも設定で変更できます。

## このChrome拡張機能の使い方と、良いところ

拡張機能のアイコンをクリックすると、こんな↓なります。

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-19-1-1024x527.jpg)

### ウェブサイト毎にフォーム内容を自動保存するかどうか設定できる

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-18.png)

このスイッチ以外にも、いくつかの方法でサイトごとに自動保存する／しないを決められます。

### 保存されている内容を検索できる

自動保存した内容が多いときは、検索が便利です。

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-19-3-1024x407.jpg)

ここでは「毎週」というキーワードを含む保存済データを検索して、見事に検索できました！

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-17.png)

### バックアップの保存期間を決められる

初期設定では30日間保存されます。歯車アイコンの設定画面から変更できます。

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-19-1024x342.png)

### キーボードショートカットが豊富

フォーム入力しているときというのは、キーボードで文字をタイプしているときですから、キーボードだけで過去の入力を呼び出せる機能はとても助かります。よく考えられた設計だと思います。

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/image-20-1024x616.png)

## 良くないところ：それでも消えちゃった！

この拡張機能も完全無欠ではないので、自動保存できないサイトもあります。この機能を過信して失敗しないように、「何ができないのか」という点は押さえておきましょう。以下のような場合、Typioは自動保存できないそうです。

- Cross domain iframes：いま見ているウェブサイトが、<iframe>というタグを利用して他のウェブサイトのフォームを埋め込んでいる場合。
- Sub domains：例えば foo.example.com で入力した内容は、bar.example.com を見ているときには呼び出せません。両者は別のウェブサイトとして扱われます。
