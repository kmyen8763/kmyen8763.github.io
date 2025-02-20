---
title: OSCP+-如何"一次"通過OSCP+考試-(含一點點CPENT、LPT心得)
date: 2024-12-27
lastmod: 2024-12-27
draft: false
tags:
  - OSCP+
  - 資安考試
  - 滲透測試
  - 考試心得
categories:
  - 資訊安全
  - 證照考試
author: KMYEN
description: 本文分享 OSCP+ 考試心得、準備方式以及考試資源，幫助考生順利通過 OSCP+ 認證。
slug: oscp-plus-exam-experience
featuredImage: /img/cover.jpg
showToc: true
showComments: true
showSummary: true

---


# 摘要：
首先感謝**科長、公司團隊**讓我有這次的機會參加考試，也特別感謝**不可思議的奇蹟、令姊、阿丸、瑩姊、Adam、Bo、schsu、yo豪、以及各個隊友**在這段時間內的協助以及指導，可以說是沒有這些隊友，我不可能過這個考試，所以大家記得~~推坑朋友一起花錢考(X)~~
由於網路上已經很多OSCP的考試說明已經在網路上很多了，所以本文主要針對OSCP+的感想以及準備的資源說明為主。

# 人權：
![2024-12-27 16_03_31-Clipboard](https://hackmd.io/_uploads/S1BdJJhBke.jpg)

## 個人背景
因為每個人的能力背景不同，所以有講述個人背景的文章才有參考的價值，
我是某國立大學的研究所資管所畢業，老實說只會寫簡單的Python，對於C語言等都不太熟悉，大概連腳本小子也不到的程度吧~
主要工作也跟資訊領域也沒有太大的關係。純粹是有機會進到公司某PartTime性質的團隊，才有機會能跟一群夥伴們一起踏入這個領域去學習。
而像是ChatGPT的出現，真的讓跨領域的學習門檻降低非常多，也鼓勵大家只要能跨出第一步，在這個AI的時代一定可以學到東西。

#### 學習到考過(一年)：
上課時間：2023-11(和團隊一起上課
續約時間：2024-06(因為自認還沒準備好，再續約30天來延長考試時間
考試日期：2024-11(剛好時間要到，而且改版OSCP+，下定決定考試(拒絕拖延症XD)

# 參考資源：
## 考試前：
### 心得類：
在考前都會擔心，甚至覺得自己準備的方向方式是否正確，因此可以多看別人的文章，來幫自己做心理建設。

[揭露 OSCP 所有秘密！-2024-06-28](https://eins.li/posts/oscp-secret-sauce/)
[適應新考試：OSCP AD Assumed Breach 情境解析與準備指南-2024-08-31](https://www.reddit.com/r/oscp/comments/1f5ojaq/assumed_breach_ad_what_you_may_need_to_know/)
[如何在半年內通過OSCP-2024-09-18](https://warranty-v01d.pages.dev/posts/how-i-passed-the-oscp/)
-->這幾篇文章很清楚的解釋上課前的準備，以及考試的詳細過程，並且提供了多種工具，很推薦大家多看一下。
[YouTube影片：Ultimate OSCP Guide 2024 - How To Pass The OSCP 2024-2024-05-10](https://www.youtube.com/watch?v=JAnC1DbjwVc)

### OSCP課程外工具

#### 建議學的：
##### 掃描(Enumeration)類：
1. [Tib3rius/AutoRecon](https://github.com/Tib3rius/AutoRecon)
-->考試畢竟是跟時間競賽，所以推薦用這個，可以快速完成許多人工步驟，當然你必須先了解他在做甚麼，並且做不到甚麼，在考試中你才會下人工指令去做更詳細的掃描。
2. [Pennyw0rth/NetExec: The Network Execution Tool](https://github.com/Pennyw0rth/NetExec)
-->在OSCP課程內學的是[CrackMapExec](https://github.com/byt3bl33d3r/CrackMapExec)，但現在已經有更好用的NetExec，建議可以學一下怎麼使用，PS：但我考試時還是使用CrackMapExec
3. [pspy](https://github.com/DominicBreuker/pspy)
-->由於考試跟課程中會有排程的題目，而要如何快速找出哪個是可以利用的排程，可以用這個，算是方便很多。
4. [wp-scan](https://www.davila.me/menu/tools-of-the-trade/wpscan)
5. [建立自己的字典檔](https://eins.li/posts/make-your-own-wordlist/)
-->這篇文章蠻推薦的，畢竟自己常常會不確定字典黨會不會lost掉，建一個整合的就不會忘記

##### 隧道(Tunneling)類：

* [ligolo-ng](https://github.com/nicocha30/ligolo-ng)
-->在課程中，他會教你怎麼使用chisel，但是建議使用ligolo，因為他會向是建立VPN一樣做tunneling，變得很簡單。([教學影片-1](https://www.youtube.com/watch?v=DM1B8S80EvQ&t=20s&pp=ygUJbGlnb2xvLW5n)、[教學影片-2](https://www.youtube.com/watch?v=qou7shRlX_s&pp=ygUJbGlnb2xvLW5n)推薦吃飯做事時可以聽2，實際要操作在按照1的慢慢學)

##### 其他(other)類：
* [tmux](https://github.com/tmux/tmux)
-->在多台機器內妳可以很方便地進行管理和自訂你的控制台
[教學影片](https://www.youtube.com/watch?v=Lqehvpe_djs&pp=ygUEVE1VWA%3D%3D)![image](https://hackmd.io/_uploads/ByyBVpoHye.png)


#### 課程
* [HTB Academy邀請連結](https://referral.hackthebox.com/mzwErlC)
-->光靠OSCP裡面的課程，可能理解的不夠詳細，我會在Academy裡面在詳細去理解實際的運作以及指令怎麼下

#### 靶機表：
* [Lainkusanagi OSCP Like](https://docs.google.com/spreadsheets/u/0/d/18weuz_Eeynr6sXFQ87Cd5F0slOj9Z6rt/htmlview?pli=1)
* [NetSecFocus Trophy Room](https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit?gid=129517485#gid=129517485)
* [vulnlab.com](https://wiki.vulnlab.com/intro/recommendations)
 -->俗話說Practice Make Perfect，以上靶機推薦大家多練習。
![image](https://hackmd.io/_uploads/HyTAmiirJl.png)

#### CheatSheet參考：
* [aditya-3.gitbook.io/oscp](https://aditya-3.gitbook.io/oscp)
-->建立自己的CheatSheet or MindMap很重要，你可以快速知道自己做了甚麼或甚麼還沒做。
-->Google還會有很多CheatSheet可以參考，最重要的是**Make your OWN CheatSheet or MindMap**.

## 考試後：

### 報告相關：
* [官方報告規格](https://help.offsec.com/hc/en-us/articles/360046787731-PEN-200-Reporting-Requirements)
* [報告撰寫影片](https://www.youtube.com/watch?v=8Biyy8B5maw)
![image](https://hackmd.io/_uploads/HJZ3rajSkg.png)





# 其他QA：
Q：OSCP+的加分算變難or變簡單?
A：因為AD不用Initial Access了(直接給帳密)，而且提權的方式很簡單。所以10分算是送你的，而且每台都有分數。
Q：OSCP教的是甚麼？
A：在OSCP的課程裡面會教你如何像是打撲克牌一樣，照某種套路(MindMap)，對每一個可能的方式都去嘗試(Try Harder)，就可以打穿。所以重點是你如何透過他的課程來建立自己的MindMap。

Q：CPENT跟OSCP的差異？
A：先上圖，最近剛上日麻的雀豪，請容我用雀魂的段位或是LOL英雄聯盟的段位來做說明
![image](https://hackmd.io/_uploads/Hy-_UpiBJg.png)
老實說，CPENT跟OSCP算是截然不同的考試，CPENT模擬一個企業環境你要在裡面找到你的目標靶機來打，但難度不會太高，OSCP則是給你確定的機器要你取得RCE，用遊戲段未來形容的話，CPENT有點像是大草原上面有好幾個牌桌(英雄聯盟則是段位場)，你要在裡面找到你要打的那幾張牌桌，而對手的水平大概是銅牌場的水準。而在OSCP則是確實的給你牌桌(3台StandAlone，1組AD)你要靠你所學的打牌理論打贏這幾場牌桌(水準大概在金之間，金牌場左右)，以上是我的體感。
**CPENT be Like：**(難度在於你要找到你要打哪幾桌)
![2024-12-27 14_23_07-Clipboard](https://hackmd.io/_uploads/HJJ1uaiHke.jpg)
**OSCP be Like：**(難度在於你學會招數，照著理論打通，不難但你要都知道)
![2024-12-27 14_26_45-Clipboard](https://hackmd.io/_uploads/SJoxFpjSye.jpg)

Q：其他QA
A：歡迎留言或加我LINE討論(lazycpumis)


### CPENT、LPT人權圖：

![2024-12-27 14_29_12-Clipboard](https://hackmd.io/_uploads/HyW5tTjSke.jpg)


# 記得OSCP、CPENT、LPT只是開始......
[Offsec_Rank #OSCP #OSCE #OSEE](https://youtu.be/6-05YGBR-Hw?si=v-MglVle123N2TDn)
![image](https://hackmd.io/_uploads/HJZKsasSyl.png)

# 最後學累了就聽歌休息吧，人生還有很多有趣的事情，加油
https://www.offsec.com/offsec/say-try-harder/
![image](https://hackmd.io/_uploads/ryukH6oB1g.png) 

```
現在聽好了！
這首獻給所有完成 Offsec 認證的人，
那些不動搖、不猶豫的人，
那些更加努力、變得更勇敢的人！
你們不能失敗，不能讓這成為一場空，
你必須更加努力！

Offsec 說要更努力！
這是取得你的 OSCP 的唯一方法
你必須比你想像的更努力
因為那是 Offsec 的哲學！ X 2
把頭猛敲在桌子上
不敢相信自己陷入如此困境
深陷在 Offsec 滲透測試的六英尺深
當你在隧道中穿梭和轉向，像挖土一樣撞到地面
痛苦和忍耐，孩子，你說你知道它，你活在其中！
但你必須打破自己的极限
當你想要放棄，只要說放棄吧，就放棄吧，

說 Bob，我真的不明白，答案是什麼？
他說“忘了吧孩子，這是 Offsec，你必須適應它”。
你想成為巨人還是侏儒，
你想成為 Offsec 認證者還是在外面開發小工具，
抬起頭，把手指放在那些數字上
我們這裡有句話，
我們呼吸它，我們活在其中，那就是

Tricia 那惡毒的女人她在你面前大笑！
你在網絡空間被謙卑的人羞辱！
這條路像馬拉松一樣長，不是短短的 50 米賽跑
不想墜落不想失敗不想失去恩典！
24 小時的測試，想把頭放在枕頭上 –
但你現在不能放棄，這是你必須擁抱的挑戰！
坐直，用那些好牙膏刷牙
做一些伏地挺身，喝些咖啡，在臉上潑冷水....
然後重新回到比賽中，
讓世界知道你的名字
那 Offsec 認證是黑客名人堂
這是無盡的讚揚，所以恢復你的信心，
你已經走了這麼遠，現在停下來只會
成為一個巨大的遺憾
你必須拋棄所有疑慮
這考試你不能失敗
你也不能停止，所以
像 Suey，你必須剁碎它！
像地板，你必須擦乾淨它！
像 Woodstock，你必須搖滾它！
振作起來，只要更努力。
我告訴你，你能做到。
更努力，更努力，更努力，更努力...
生命如此短暫，所以要全力以赴，你得做到
這次滲透測試只是未來事情的一個範例
生命如此短暫，在你的生活中你必須得到一些……
```