---
title: "ChatGPTで授業準備（クイズ作成編）：読解文とQuizizzデータ作成が2分で終わる！"
date: "2023-04-23 10:58:45"
categories:
  - "#ほぼ週刊ググレカス"
  - "AI"
  - "EdTech"
permalink: "https://laiken.net/ggrks/chatgpt-to-quizizz/"
tags:
  - "ChatGPT"
  - "情報リテラシー"
  - "業務効率化"
url: "/chatgpt-to-quizizz/"
image: "images/banners/2023/04/blog-banner-1280x720-1_comp30.jpg"
---

もう、ゼロから問題文や選択肢を考えなくてもいい！「1文字もタイプすること無く」クイズが完成します。（ChatGPTのプロンプトは除きます）今回はChatGPTを使って、定番のクイズプラットフォーム、Quizizzの問題データを極めて短時間で作成する方法をご紹介します。

読むのが面倒な方はこちら！

https://www.youtube.com/watch?v=KmNGD9fo4pE

## 用意するもの

1. [ChatGPT（有料版、無料版どちらでも可）](https://chat.openai.com/)
2. [Quizizz](https://quizizz.com/) のアカウント
3. Quizizzの問題作成用テンプレート。Excel形式のファイルがこちらからダウンロードできます： [QuizizzSampleSpreadsheet.xlsx](https://support.quizizz.com/hc/en-us/article_attachments/4402409922573/QuizizzSampleSpreadsheet.xlsx)

## 1. ChatGPTで文章作成

例として今回は、ChatGPTにスティーブ・ジョブズについての物語を書いてもらいました。上のYouTube動画では無料版でも使えるGPT-3.5を使っています。

### 文章生成用のプロンプト

```
スティーブ・ジョブズについての物語を彼の面白いエピソードを交えて書いてください
```

この1行をコピペして送信するだけです。物凄い時代になりましたね。

### 文章が途中で切れて終わってしまったら「続けて」

ChatGPTは1回に出力できるおおよその文字数が決まっているので、長い文章を書かせると最後までたどり着けずに途中で切れてしまうことがよくあります。そんな時は図のように「続けて（または continue）」と一言、打ち込むだけで、その次の文字から続きを書いてくれます。（書いてくれないこともあります）

![](https://laiken.net/ggrks/wp-content/uploads/2023/04/69062be4cd80fbe6d9830b86dbf76045-edited-1.jpg)

### 【重要】ChatGPTで書いた文章は事実確認が必須

AIが書いた文章は教材として使う前に、**必ず事実確認を行ってください**。この例のスティーブ・ジョブズのように、実在する人物に関する情報を教材として使う場合には、ChatGPTが書いた情報が事実に即しているかの確認が必要です。

事実確認が面倒だ、という場合は、初めにChatGPTにフィクションを創作するように指示しましょう。これなら問題文は架空の物語になりますから、事実確認は必要ありません。

## 2. ChatGPTで多肢選択式問題の作成

いわゆる4択問題です。ChatGPTにクイズ作成を指示すると、たいてい4択問題を作ります。別の種類の問題を作りたい場合は、どのような問題形式を作りたいかを明確に指示してください。

### クイズ作成用のプロンプト

では続いて、文章の理解度を測る選択肢問題を5問、作成してもらいましょう。

```
この文章の理解度を測る選択肢問題を5つ作成してください
```

作成された問題にはおそらく、a〜dの選択肢が付いていると思います。

![](https://laiken.net/ggrks/wp-content/uploads/2023/04/image-1024x856.png)

ここまで、本当に一瞬で終わりますね。教師は、ほとんど何もしていません。

## 3. クイズ形式への変換

Quizizzでは、Excel形式のデータをインポートして一括でクイズを作成することができます。

### できあがったクイズをQuizizz形式へ変換するプロンプト

ここまでの手順で作ったクイズをExcelにそのまま貼り付けられるように、以下のプロンプトでデータ形式を変換します。このままコピペして下さい。

```
このクイズを以下のヘッダ行に合わせて、TSV形式に変換して下さい。

```
Question Text, Question Type, Option 1, Option 2, Option 3, Option 4, Option 5, Correct Answer
```
- Correct Answer はアルファベットではなく、数字 (1-4) にして下さい。
- 2列目の値は固定で、"Multiple Choice" にして下さい。
- Option 5は空欄にして下さい。 
- 結果をcode snippetで表示して下さい。
```

TSV形式というのは、タブという空白文字列で区切られたデータ形式のことです。カンマで区切られたCSV形式の方が有名ですが、区切り文字が違うだけで、同じテキストデータです。

この結果を code snippet を使って表示するように指示します。これはプログラミング言語を文章に貼り付ける時によく使うツールです。上手くいけば、以下のような結果になるはずです。

右上の「Copy code」をクリックしてデータをコピーし、ExcelやGoogle Sheetsに貼り付けます。Google Sheetsを使っている場合は、Excel形式でダウンロードします。

## 4. Quizizzにインポート

Excelができたら、あとはQuizizzにインポートするだけです。詳しい手順はYouTubeをご覧ください。

ExcelからQuizizzにインポートする方法はQuizizzの公式サイトにも詳しい説明がありますので、詳細は以下のリンクを参照してください。分かりやすいビデオもありますので、簡単にできるでしょう。

[Import a Quiz From a Spreadsheet – Help Center](https://support.quizizz.com/hc/en-us/articles/115003688491-Import-a-Quiz-From-a-Spreadsheet)

### Quizizzへのインポート時にエラーが出たら

変換ミスが起こりにくいように上記のプロンプトは既に改良済ですが、それでもExcelを取り込む時にエラーが出た場合は、Excelデータに誤りがあるはずなので確認して修正してください。

例えば以下の図では、ヘッダ行（最初の行）の2列目を「Question Type」とすべきところを「Multiple Choice」と誤って書いています。この場合は、Excelを手作業で修正すればよいでしょう。

![](https://laiken.net/ggrks/wp-content/uploads/2023/04/image-1-1024x508.png)

インポートが完了したら、クイズをプレビューして問題が正しく表示されるか確認しましょう。

以上、ChatGPTを使ってクイズを作成する方法をご紹介しました。慣れれば1〜2分でこの作業が終了するはずです。「今までの試験作成の苦労は何だったんだ」となること請け合いです。ぜひ試してみて下さい！

## 関連記事：ChatGPTで授業準備

こちらの記事も併せてどうぞ！

https://laiken.net/ggrks/lesson-prep-with-chatgpt/
