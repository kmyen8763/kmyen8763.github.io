---
title: CEH-V11 考試心得 & 題庫資源分享
date: 2023-08-12
lastmod: 2023-08-12
draft: false
tags:
  - CEH-V11
  - 資安考試
  - 題庫分享
  - 網路安全
categories:
  - 資訊安全
  - 證照考試
author: KMYEN
description: 本文分享 CEH-V11 考試心得、準備方式以及考題資源，幫助考生順利通過 CEH-V11 認證。
slug: ceh-v11-exam-experience
featuredImage: /images/CEH_Logo.jpg
showToc: true
showComments: true
showSummary: true
---

# CEH-V11-考試心得&題庫資源分享

## 考試成績：124/125

![https://hackmd.io/_uploads/By_N2SZyT.png](https://hackmd.io/_uploads/By_N2SZyT.png)

PS:敗在IOT Seeker那題，當時在思考是IOT Inspector還是IOT Seeker，如果是我自己應該會用IOT Inspector聽起來比較厲害。

## 心得

一直以來對資安這一塊有興趣但又不知道怎麼入門，剛好有幸能有研究所朋友推坑，一起花了五六萬塊來上CEH的課程，整體課程僅有5天(可重聽一次但我沒去)，上完其實能得到的收穫不多，事後發現這一門領域還是要靠自己去學習。

近期便買了「HTB Academy」來玩，真的學到蠻多的，在準備Nmap的題目時候「HTB Academy」裡面有一個Module(如下圖)透過裡面實際操作學習後，可以把很多題目變成不是死背而是真的利用到知道怎樣用，非常推薦準備考試的人可以使用(裡面有許多免費課程，可以先從免費的用了之後覺得喜歡再考慮購買)

![https://hackmd.io/_uploads/HJG60BW1T.png](https://hackmd.io/_uploads/HJG60BW1T.png)

![https://hackmd.io/_uploads/Bko5kI-kT.png](https://hackmd.io/_uploads/Bko5kI-kT.png)

## 準備方式：

由於我比較懶惰，所以從去年上完課程後只有少數時間做做考古題，有友人大神做了google表單版本的考古題，但Google表單的缺點是我考完400題目後才能確認答不不不之案以及我不能確認答案是否正確(CEH有許多官方答案是錯誤的)

因此後來找到一個網站

[「Examtopics」-CEH-V11考題](https://www.examtopics.com/exams/eccouncil/312-50v11/view)

，CEH考試的題目與答案均100%相同，故可以透過考古題方式快速準備，該網站的優點為下方有許多人的討論，可以幫助你判斷正確答案是甚麼。

![https://hackmd.io/_uploads/SkJ11Ibkp.png](https://hackmd.io/_uploads/SkJ11Ibkp.png)

判斷正確答案之技巧：
1. 若大家投票=官方正確答案時–>該答案為正確答案
3. 大家投票遠大於官方正確答案–>大家投票為正確答案
2. 大家投票有多選項均為相同比例時–>至網路上Google找到詳細官方資訊來判斷哪個是正確答案。

該網站詳細的網址請參考文章末點，他免費資源開放到190題後就要付費才能觀看，但在這邊我們運用GoogleDorking的技巧，透過搜尋「exam 312-50v11 topic 1 question 題號 discussion inurl:discussions/eccouncil/view inurl:discussions/eccouncil/view」就可以繞過該網站的付費機制直接看到題目以及討論。
> 範例：exam 312-50v11 topic 1 question 191 discussion inurl:discussions/eccouncil/view

透過上述網站，邊做題邊紀錄我總共做完了3次題目，每次做完題目後都會將錯誤題目再作答一次，如果又錯就會詳細看大家下方的解釋並且在網路上找答案。

![https://hackmd.io/_uploads/By2bDUZ1T.png](https://hackmd.io/_uploads/By2bDUZ1T.png)

以上大概是我準備CEH的心得，希望能幫助到大家準備該考試。
> 接下來要準備CPENT了，希望一切順利~

## 參考資源：

1.[我的練習考古題紀錄](https://docs.google.com/spreadsheets/d/11RKp8uWCUmSekHSXexOPa4nQGFJHIRIQ6kToHmYAkvc/edit?usp=sharing)
2.Examtopics-CEH-V11考古題
* 1~10題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/1
* 11~20題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/2
* 21~30題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/3
* 31~40題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/4
* 41~50題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/5
* 51~60題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/6
* 61~70題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/7
* 71~80題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/8
* 81~90題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/9
* 91~100題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/10
* 101~110題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/11
* 111~120題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/12
* 121~130題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/13
* 131~140題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/14
* 141~150題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/15
* 151~160題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/16
* 161~170題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/17
* 171~180題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/18
* 181~190題：https://www.examtopics.com/exams/eccouncil/312-50v11/view/19
* 194題：https://www.examtopics.com/discussions/eccouncil/view/50380-exam-312-50v11-topic-1-question-194-discussion/
* 285題：https://www.examtopics.com/discussions/eccouncil/view/58483-exam-312-50v11-topic-1-question-285-discussion/
* 319題：https://www.examtopics.com/discussions/eccouncil/view/62890-exam-312-50v11-topic-1-question-319-discussion/
* 337題：https://www.examtopics.com/discussions/eccouncil/view/62963-exam-312-50v11-topic-1-question-337-discussion/
* 358題：https://www.examtopics.com/discussions/eccouncil/view/63038-exam-312-50v11-topic-1-question-358-discussion/
* 360題：https://www.examtopics.com/discussions/eccouncil/view/63041-exam-312-50v11-topic-1-question-360-discussion/
* 371題：https://www.examtopics.com/discussions/eccouncil/view/66614-exam-312-50v11-topic-1-question-371-discussion/
* 376題：https://www.examtopics.com/discussions/eccouncil/view/63092-exam-312-50v11-topic-1-question-376-discussion/