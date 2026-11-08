---
title: "Google Classroomで採点時のコメント欄を広くする"
date: "2022-12-27 12:11:52"
categories:
  - "#ほぼ週刊ググレカス"
  - "EdTech"
permalink: "https://laiken.net/ggrks/toggle-google-classroom-side-panel-width/"
tags:
  - "google"
  - "グーグル"
  - "ライフハック"
  - "情報リテラシー"
  - "業務効率化"
url: "/toggle-google-classroom-side-panel-width/"
---

Google Classroomで提出物の管理をしている皆さん、コメント欄の幅が狭すぎると思いませんか？今回はイライラを解消すべく、簡単なブックマークレットを書いてみましたのでご紹介します。

## Google Classroom採点画面のコメント欄の幅：通常時と改善後

Google Classroomで採点する時、右側のサイドパネルはこのくらいの幅しかありませんね。

![](https://laiken.net/ggrks/wp-content/uploads/2022/12/image-2-1024x576.png)

単なるCSS上の問題だったので、ブックマークレットを書きました。こうなります：

![](https://laiken.net/ggrks/wp-content/uploads/2022/12/image-3-1024x428.png)

## この機能の使い方

![](https://laiken.net/ggrks/wp-content/uploads/2021/03/Screen-Recording-2021-03-11-at-3.49.59-PM-00.00.00.000-00.00.02.052.gif)

1. [Toggle Side Panel Width](javascript:(function() %7Bvar e%3Ddocument.getElementsByClassName(%27uoiRud%27)%5B0%5D%3Be.style.width%3D(e.style.width!%3D%27512px%27)%3F%27512px%27:%27256px%27%3B%7D)()%3B) ←このリンクをブックマークにドラッグする！
2. Google Classroomの採点画面を開く
3. ブックマークレットをクリックする。幅がひろーい！
4. もう一度クリックすると、もとに戻ります。
