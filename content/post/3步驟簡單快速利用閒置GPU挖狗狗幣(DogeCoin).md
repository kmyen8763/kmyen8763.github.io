---
title: 3步驟簡單快速利用閒置GPU挖狗狗幣(DogeCoin)
date: 2025-01-07
lastmod: 2024-11-07
draft: false
tags:
  - 虛擬貨幣
categories:
  - 虛擬貨幣
author: KMYEN
description: 加密貨幣熱潮讓許多人對挖礦充滿好奇，這篇文章將帶你快速利用閒置 GPU 挖掘狗狗幣（DogeCoin）。
slug: dogecoin-gpu-mining
featuredImage: /images/dogecoin-gpu-mining-image3.png
showToc: true
showComments: true
showSummary: true
---
# 3步驟簡單快速利用閒置GPU挖狗狗幣(DogeCoin)

# 簡介

---

加密貨幣熱潮讓許多人對挖礦充滿好奇，但隨著電費成本上升，個人挖礦已難以獲利。如果你只是想體驗挖礦過程，利用閒置GPU挖狗狗幣（Dogecoin）是個絕佳選擇。這篇文章將帶你一步步完成，輕鬆感受加密貨幣的樂趣！

以下將分成**「3步驟」**依序進行

## 步驟1：**取得錢包地址(已有地址可跳過)**

先下載「Trustwallet」，可以在各個平台商店下載。

**下載連結：**

---

[Chrome插件版](https://chrome.google.com/webstore/detail/trust-wallet/egjidjbpglichdcondbcbdnbeeppgdph)

[Apple App Store版](https://apps.apple.com/app/apple-store/id1288339409?mt=8)

[Google Play商店版](https://play.google.com/store/apps/details?id=com.wallet.crypto.trustapp)

---

建立錢包影片：
{{< youtube XOfK4QgMxnE >}}

再來是如何創建dogecoin錢包：

Youtube：20秒建立狗幣錢包

{{< youtube IbeZOS5V6n0 >}}

## 步驟2：設定挖礦軟體_**開始挖礦**

第一步：挖礦軟體

[GitHub連結：https://github.com/Lolliedieb/lolMiner-releases](https://github.com/Lolliedieb/lolMiner-releases)

這邊使用下載狗狗幣挖礦軟體，建議使用「lolMiner」，以下會提供挖礦的Code

[下載連結：https://github.com/Lolliedieb/lolMiner-releases/releases](https://github.com/Lolliedieb/lolMiner-releases/releases)

下載下方紅色框框的檔案即可
![Image Description](/images/dogecoin-gpu-mining-image.png)


---

第二步：解壓縮
![Image Description](/images/dogecoin-gpu-mining-image1.png)

第三步：先到解壓縮的資料夾

小步驟-1.找到檔案「mine_dog.bat」點擊右鍵選擇「記事本開啟」
![Image Description](/images/dogecoin-gpu-mining-image2.png)

小步驟-2：修改成你自己的地址

修改用：

```python
@echo off
setlocal enableDelayedExpansion
Rem #################
Rem ## 編輯以下部分 ##
Rem #################
set "POOL=ethash.unmineable.com:3333"
set "WALLET=DOGE:替換成狗狗幣地址.DogeNo1#w3w6-chtu.lolMinerWorker"                    
Rem ###################
Rem ##  編輯以上部分  ##
Rem ###################
:loop
lolMiner.exe --algo ETHASH --pool !POOL! --user !WALLET! --watchdog exit
if %ERRORLEVEL% == 42 (
  timeout 10
  goto loop
)
pause
```

範例

```python
@echo off
setlocal enableDelayedExpansion
Rem #################################
Rem ## Begin of user-editable part ##
Rem #################################
set "POOL=ethash.unmineable.com:3333"
set "WALLET=DOGE:替換成狗狗幣地址.DogeNo1#w3w6-chtu.lolMinerWorker"                    
Rem #################################
Rem ##  End of user-editable part  ##
Rem #################################
:loop
lolMiner.exe --algo ETHASH --pool !POOL! --user !WALLET! --watchdog exit
if %ERRORLEVEL% == 42 (
  timeout 10
  goto loop
)
pause
```

小步驟-3：點擊檔案「mine_dog.bat」執行

![Image Description](/images/dogecoin-gpu-mining-mine_dog_bat.png)

## 步驟3：檢視餘額，**等待足額轉出狗狗幣(DogeCoin)**

小步驟1：檢視餘額

網址請自行修改：

```python
https://unmineable.com/address/狗幣錢包地址?coin=DOGE
```

挖滿30顆可以出金，點Payout按鍵會直接匯到你的地址內

⚠️PS：如果是交易所錢包，請注意是否有最低額度限制，不然會被吃掉

![Image Description](/images/dogecoin-gpu-mining-image3.png)

