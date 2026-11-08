---
title: "1文字も打ち込まずに「まるごと」語彙インデックスからQuizlet問題を作成する"
date: "2021-08-22 00:13:41"
categories:
  - "#ほぼ週刊ググレカス"
  - "EdTech"
permalink: "https://laiken.net/ggrks/marugoto-quizlet/"
tags:
  - "google"
  - "Kahoot!"
  - "Quizalize"
  - "Quizlet"
  - "Quizziz"
  - "オンライン授業"
  - "キーボードショートカット"
  - "グーグル"
  - "ハイブリッド授業"
  - "ほぼ週刊ググレカス"
  - "ライフハック"
  - "情報リテラシー"
  - "情報教育"
  - "時短"
  - "業務効率化"
url: "/marugoto-quizlet/"
---

ラクダの皆さん、きょうも冒険家を背中に乗せてうひゃひゃひゃーですか？🐫  
さて、Quizletや単語帳アプリを使う時、わざわざ単語とその意味を打ち込んでいませんか？その手間、不要です！基本的に、QuizletやAnki、上級者ならKahoot!やQuizizzですら「1文字もタイプせずに」問題を作ることが可能です。今回は、「まるごと」公式サイトで教師用リソースとして公開されているデータを使って、QuizletやAnkiなどに利用できる基本的なデータの作成方法をご紹介します。

## 元データを入手する

この手順が一番重要です。良質な元データが入手できれば、その後の作業が圧倒的に楽になるからです。「まるごと」の場合は、[レベル別に語彙インデックスが公開されている](https://www.marugoto.org/teacher/resource/elementary1_c/)ので、これを使わない手はありませんね。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-10.png)

### Excel形式をGoogleスプレッドシート形式に変換する

お住いの地域や、宗教上の理由？とかで「Googleの各種サービスは使えない！」という事情がない限りは、ExcelよりもGoogleスプレッドシート（正式にはGoogle Sheets）に慣れておくのが良いでしょう。Excelにできないことが色々できますよ。  
（参考：[Google Sheetsの方がExcelよりヤバイところ | Laiken (らいけん) on Patreon](https://www.patreon.com/posts/52010041)）

#### Excel→Google Sheets変換手順

1. Googleドライブの設定を開いて、[Convert uploads]にチェックを入れる
2. まるごと公式サイトからダウンロードしたExcelファイルをGoogleドライブに放り込む

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-19-1024x465.png)

これでExcelファイルがGoogleスプレッドシートで開けるはずです。場合によっては、Google Sheets形式で保存する必要があるかもしれません。

以下の手順はGoogle Sheetsを利用している前提で書いていますが、もしかしたらExcelでも同様のことはできるかもしれません。

## 初級編：Sheet1の内容を利用する

公式の英訳データがついているという意味で、Sheet1の内容は貴重です。学習者のL1や媒介語が英語ではない場合は自動翻訳すれば対応できますが、今回はその手順は割愛します。

ここでは最も基本的なデータの利用方法として、このB列とC列のデータをそのままQuizletに利用する手順をご紹介します。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-12.png)

下図のように、B〜C列の3行目から、最後まで選択します。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-13.png)

これをそのままQuizletに貼り付けると2000件もありますから、適度な問題数に絞りたいですね。例えば、「ランダムに並べ替えて上から10件だけをクイズに使う」というようなやり方が簡単です。

上記の選択範囲はそのままで、Dataメニューから"Randomize range"を実行すると、選択範囲がランダムに並べ替えられます。この中から、好きな範囲をコピーしましょう。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-14.png)

## Quizletにインポートする

まだ[Quizlet](https://quizlet.com/)を使ったことがない人は、アカウントを作成しておいて下さい。アカウントがある人は、最上部の"Create"ボタンから"Study set"を選んで、新規のセットを作成します。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-15.png)

下記の画面で1問ずつ手入力することも可能ですが、そんな非効率で面倒なことは、できれば避けたいですね。小さな字で分かりにくいですが、"Import from Word, Excel, Google Docs, etc."をクリックします。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-16.png)

ランダムに並べ替えた語彙インデックスから例えば10行、コピーしてQuizletのインポート画面に貼り付けます。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-17-1024x583.jpg)

この後は”Import”ボタンを押して、必要ならば修正等を加えて、セットを作成すれば完了です。

## もっと色々できるよ

初級編としてSheet1のデータのみを使う方法を紹介しましたが、もう一つのシートにある情報を活用した、初出課や品詞ごとのデータ作成も比較的簡単にできます。機械翻訳を組み合わせる方法も今後紹介したいと思います。

## らいけんが作ったGoogleシートが欲しい！

Google Sheetsのイケてる関数を駆使して、初出課や品詞ごとにフィルターしたり、各国語に自動翻訳したりできる「スーパーウルトラハンディまるごと→Quizlet変換シート」を作成しました。こちらのビデオで使い勝手がわかります。

https://www.youtube.com/watch?v=F3AFEymgFf8

このシートは、らいけん公式サポーターの皆さんにお分けしてます！下記のリンクからどうぞ：  
[「まるごと」語彙インデックスからQuizletの問題を作成する | Laiken (らいけん) on Patreon](https://www.patreon.com/posts/55085589)
