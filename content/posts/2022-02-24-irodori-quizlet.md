---
title: "1文字も打ち込まずに「『いろどり』のことばリスト」からQuizlet問題を作成する"
date: "2022-02-24 14:11:31"
categories:
  - "#ほぼ週刊ググレカス"
permalink: "https://laiken.net/ggrks/irodori-quizlet/"
tags:
  - "Gimkit"
  - "google"
  - "Kahoot!"
  - "Quizizz"
  - "Quizlet"
  - "いろどり"
  - "オンライン授業"
  - "グーグル"
  - "まるごと"
  - "ライフハック"
  - "情報リテラシー"
  - "日本語教育"
  - "時短"
  - "業務効率化"
url: "/irodori-quizlet/"
---

日本語教師の皆さん！🐫 単語帳やクイズを作る時に、わざわざ単語とその意味をタイプして打ち込んでいませんか？その手間、不要です！1文字も打ち込まないシリーズ第2弾は、「いろどり 生活の日本語」の付属資料を使った方法です。

## いろどりとは？

「日本語コースブック『いろどり　生活の日本語』は、外国の人が日本で生活や仕事をする際に必要となる、基礎的な日本語のコミュニケーション力を身につけるための教材」だそうです。無料でかつデジタルデータを入手できるというのが、現代に相応しい配布方法ですね。詳しくはこちらをどうぞ。>> [いろどり　とは？ | いろどり　生活の日本語](https://www.irodori.jpf.go.jp/about.html)

## 元データを入手する

まず、公式サイトの「付属教材・資料」というセクションで配布されている「ことばリスト」のExcelデータを入手しましょう！>> [付属教材・資料 | いろどり　生活の日本語](https://www.irodori.jpf.go.jp/resources.html)

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image.png)

配布されているデータはExcel形式ですが、Googleシートに変換することもできます。詳しくはこちらの記事をどうぞ。

https://laiken.net/ggrks/marugoto-quizlet/#toc2

### 媒介語に注意！

上記で配布されているデータは、**単語が英訳されたもの**です。別の言語に翻訳されたExcelデータは、「各国語版」のサイトから探してみて下さい。>> [各国語版 | いろどり　生活の日本語](https://www.irodori.jpf.go.jp/editions.html)

### Googleシート＋Google翻訳を使う方法

各国語版にも無い言語でQuizletや単語帳データを作りたい場合は、GoogleのスプレッドシートとGoogle翻訳を組み合わせて、英訳を各国語訳に変換する方法があります。これは時間ができたら別記事で紹介したいと思います。

お急ぎの方は、過去に筆者が作った「まるごと」用の翻訳シートをお配りしていますので、そちらを改造してみて下さい。>> [「まるごと」語彙インデックスからQuizletの問題を作成する | Laiken (らいけん) on Patreon](https://www.patreon.com/posts/55085589)

## シートの内容を理解する

ここからは、データをGoogleシート上で開いている前提で進めます。Excelでもほとんど同じはずです。

### Quizletの内容となる基本データ

まず必要になるのはD〜G列のデータでしょう。D列のカナ表記に対してG列の英訳を組み合わせるのが一般的な単語帳ですが、アクセントを覚えるためのクイズや、入門に限れば、ローマ字で読み方のクイズを作ることもできますね。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-1-1024x347.png)

### データ抽出に使える品詞分類や初出箇所

見て下さい、この品詞分類を。動詞グループまで入ってますよ！「〜課で出てくる2グループの動詞だけ練習」みたいなことが簡単にできます！これは教師の強い味方になることでしょう。

初出箇所の見方は独特で、「再出」が空欄のものが初出ということのようです。これで新出単語のみのクイズも容易に作成できます。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-2.png)

## データ抽出の仕方

では例として、「初級2の1〜3課で初出の1グループの動詞」だけを取り出してみましょう。データ抽出には、この「ことばリスト」データをGoogleシートを開いた時点で有効になっているフィルター機能を使います。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-3.png)

**大量のデータから必要なものだけを抽出できる能力は、検索エンジンが使えることと同じくらい重要なことです。**この機能はぜひ覚えましょう！

## Quizletにインポートする

まだ[Quizlet](https://quizlet.com/)を使ったことがない人は、アカウントを作成しておいて下さい。アカウントがある人は、最上部の”Create”ボタンから”Study set”を選んで、新規のセットを作成します。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-15.png)

下記の画面で1問ずつ手入力することも可能ですが、そんな非効率で面倒なことは、できれば避けたいですね。小さな字で分かりにくいですが、”Import from Word, Excel, Google Docs, etc.”をクリックします。

![](https://laiken.net/ggrks/wp-content/uploads/2021/08/image-16.png)

### データをQuizlet形式に整形する

下の画像を見て下さい。「WordやExcelからデータをコピペしてね」と書いてありますが、決められたデータ形式があります。Quizletでは、各行に単語とその意味が並んだ、**2列の形式**である必要があります。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-4.png)

一方、先程データ抽出をした「ことばリスト」は「読み、アクセント、ローマ字、英訳」の**4列（D〜G列）のデータ**から成ります。このままでは、Quizletに貼り付けることができません。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-5.png)

そこで作業用の新規シートを開いて、不要な列を削除しましょう。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-6.png)

新しく開いたSheet1に「ことばリスト」から抽出した4列のデータを貼り付けて、不要なデータ（ここではアクセントとローマ字の列）を削除します。

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-7.png)

さあ、これで2列のデータが出来上がったはずです。これをQuizletに貼り付けましょう！

![](https://laiken.net/ggrks/wp-content/uploads/2022/02/image-8.png)

この後は”Import”ボタンを押して、必要ならば修正等を加えて、セットを作成すれば完了です。

## 1文字も打ち込まなかった！

いかがでしたか。無事に1文字も打ち込むことなく、Quizletを作成することができたと思います。分からないことがあれば、筆者が直接レッスンをできますので[お問い合せ下さい](https://laiken.net/ggrks/contact/)。

Quizlet以外にもQuizizzやKahoot!のようなツールが沢山あります。最近の筆者のおすすめはGimkitです。

https://laiken.net/ggrks/gimkit-goes-free/

### QuizletのデータをKahoot!とQuizizzとGimkitに自動変換する

実は、QuizizzとKahoot!とGimkit用のデータは、今回作成したQuizlet用のデータから自動的に変換して作成することが可能です。基になるQuizletのデータさえあれば、ほとんど手間を掛けずに、多様な見せ方で楽しく授業や演習をすることが可能になります。

筆者が作成した自動変換用Googleシートをサポーターの皆様にお配りしております。以下が当該記事です。この機会にぜひご検討下さい。

- [Quizletの問題をKahoot!とQuizizzの形式に自動変換する | Laiken (らいけん) on Patreon](https://www.patreon.com/posts/53849436)
- [Quizlet→Quizizz変換シート デモ動画 | Laiken (らいけん) on Patreon](https://www.patreon.com/posts/55755138)
- [Quizlet→Gimkit変換に対応しました | Laiken (らいけん) on Patreon](https://www.patreon.com/posts/59122845)
