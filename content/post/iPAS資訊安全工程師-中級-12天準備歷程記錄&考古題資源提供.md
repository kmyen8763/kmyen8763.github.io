---
title: iPAS 資訊安全工程師-中級 12天準備歷程記錄 & 考古題資源提供
date: 2023-09-15
lastmod: 2023-09-15
draft: false
tags:
  - iPas
  - 資訊安全
  - 資安證照
  - 考古題
  - CVSSv3
categories:
  - 資訊安全
  - 證照考試
author: KMYEN
description: 本文分享 iPAS 資訊安全工程師-中級考試心得、準備方式以及考題資源，幫助考生順利通過 iPAS 認證。
slug: ipas-security-engineer-exam-prep
featuredImage: /img/cover.jpg
showToc: true
showComments: true
showSummary: true
---


# iPAS資訊安全工程師-中級-12天準備歷程記錄&考古題資源提供

## 結果：PASS

![https://hackmd.io/_uploads/HkbPIHbka.png](https://hackmd.io/_uploads/HkbPIHbka.png)

## 心得：

透過考古題可以發現該科考試的範圍極廣，不是短時間內可以準備完成的，而且有讀過法規的相關資安認證的更有優勢，這次有幸能夠在12天內就考過也是運氣好，沒有考太多法規面的東西。
事後回顧為什麼會過可能是同時也在準備CEH考試的關係，CEH考科跟這邊實務面的東西有許多相似之處，雙方都有各自沒有的範圍。
PS:[CEH準備心得筆記](https://hackmd.io/@7ZcmfE2ETz-ntel2Ma6uTg/rJvhYym62)

## 歷屆考古題：

iPas_資訊安全規劃實務_中級_歷屆考題：
>https://forms.gle/bXEeyXWP5RtuHxcC7

iPas_資訊安全防護實務_中級_歷屆考題：
>https://forms.gle/KRpoLr4sMuXi6EzD7

## 錯誤題目檢討：

> https://docs.google.com/spreadsheets/d/1Nj3shzjCJZBqBOhLjRVV2iIYokPLWThtbadLJT9izfE/edit?usp=sharing
> 

## 考試DeadLine

考試日期：112年08月12日（六）
考試時間：09:00-10:30資訊安全規劃實務；11:00-12:30資訊安全防護實務
## 準備時間(11 Days)：
0801：iPas_資訊安全規劃實務_中級_歷屆考題-製作完成
0803：iPas_資訊安全防護實務_中級_歷屆考題-製作完成
0804：iPas_資訊安全規劃實務_中級_歷屆考題-50%做完
0805：iPas_資訊安全防護實務-中級_歷屆試題-第一次裸考(正確率66.33%(132/199))
0806：iPas_資訊安全防護實務-中級_歷屆試題-第一次裸考(正確率53.06%(105/196))
0807：上班
0808：白天上班(08-20)、防護實務(錯誤題目-檢討詳解)-複習至109-07
0809：白天上班(08-20)、防護實務(錯誤題目-檢討詳解)-檢討完成
0810：白天上班(08-20)、完成歷屆試題重考-第二次、看iThome、了解zero trust
0811：白天上班(08-20)、完成歷屆試題重考-第三次、看iThome
0812：考試

## CVSSv3

- 基本矩陣群 (Base metric group)
1. 攻擊向量 (Attack Vector, AV)
*Network (N)：由網際網路網路進行攻擊*
Adjacent (A)： 由受限制的網路進行攻擊，如區域網路及藍芽等
*Local (L)：在不連接網路的狀況下進行攻擊*
Physical (P)：需接觸到實體機器才能進行攻擊
2. 攻擊複雜度 (Attack Complexity, AC)
*Low (L)：低，攻擊可被輕易重現*
High (H)：高，須由攻擊者達成數項條件後才能成功
3. 是否需要提權 (Privileges Required, PR)
*None (N)：不需要*
Low (L)：需要一般使用者權限
*High (H)：需要管理者權限
4. 是否需要使用者操作 (User Interaction, UI)
*None (N)：不需要*
Required (R)：需要使用者操作某些動作才能讓攻擊成功
5. 影響範圍 (Scope, S)
*Unchanged (U) ：僅影響含有漏洞的元件本身*
Changed (C)：會影響到含有漏洞的元件以外的元件
6. 機密性影響 (Confidentiality, C)
*None (N)：無影響*
Low (L)：攻擊者可以取得機密資料，但無法使用該資料
*High (H)：攻擊者可以取得機密資料，且可以使用該資料
7. 完整性影響(Integrity, I)
*None (N) ：無影響*
Low (L) ：攻擊者有部分權限以竄改某些資料，對含有漏洞之元件影響較小
*High (H)：攻擊者有權限竄改所有資料，對含有漏洞之元件有嚴重影響
8. 可用性影響 (Availability, A)
*None (N)：無影響*
Low (L)：可用性受到影響，導致服務或元件仍可被部分取得，或是時好時壞
*High (H)：可用性受到嚴重影響，導致服務或元件完全不可被取得
- 暫時矩陣群 (Temporal metric group)
- 環境矩陣群 (Environmental metric group)
    
    ![https://hackmd.io/_uploads/SJDFl612h.png](https://hackmd.io/_uploads/SJDFl612h.png)
    

## 參考資源：

iPAS資訊安全工程師中級筆記
https://hackmd.io/@Not/iPASInformationSecuritySpecialist#iPAS%E8%B3%87%E8%A8%8A%E5%AE%89%E5%85%A8%E5%B7%A5%E7%A8%8B%E5%B8%AB%E4%B8%AD%E7%B4%9A%E7%AD%86%E8%A8%98