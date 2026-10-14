# 範例：寫給德國客戶的出貨通知

> 這封信的每一句，都是英文不錯的業務常寫、自己以為是對的句子。
> 結果以2026-10-13用本skill（Claude Sonnet）實際執行的輸出為基礎；收件人國家改為德國，文化提醒依德國調整。不同AI、不同次執行，措辭會略有不同。

## 輸入

```text
Dear Mr. Thomas,

Here is Wilson from ABC Company. We have sent the samples last Friday. Please be noted that the tracking number is as below.
Our price is cheap and there are many customers like this model.
The goods will ship on 03/04 and the price is $12 per unit. Please kindly confirm the order and revert to me ASAP.
Thank you for choosing us. Welcome to contact us if you have any questions.
Look forward to hear from you.
```

收件人：德國客戶

## 輸出

情境：通用

找到13個問題：4個文法錯誤、6個可能造成誤會、3個讀起來不自然。

| # | 原句 | 等級 | 建議改法 | 為什麼 |
|---|---|---|---|---|
| 1 | Dear Mr. Thomas, | 🟠 | Dear Mr. Weber,（換成對方的姓） | Mr.後面要接「姓」，不是名字，會讓對方覺得你搞不清楚他的稱呼（規則24） |
| 2 | Here is Wilson | 🟡 | This is Wilson | 中文「這裡是Wilson」直翻，英文自我介紹要用This is…（規則23） |
| 3 | We have sent the samples last Friday | 🔴 | We sent the samples last Friday | 有last Friday這種明確過去時間，就不能用現在完成式（規則20） |
| 4 | Please be noted that…as below | 🔴 | Please note that the tracking number is below | be noted的主詞該是事，不是人；as below是亞洲商務信的老習慣（規則26） |
| 5 | Our price is cheap | 🟠 | Our prices are competitive | cheap常帶「廉價、品質差」的意思，報價要用competitive（規則8） |
| 6 | there are many customers like this model | 🔴 | many customers like this model | There are…後面要接who／that才能再接動詞（規則16） |
| 7 | 03/04 | 🟠 | March 4 | 德國習慣日在前，03/04會被讀成4月3日（規則29） |
| 8 | $12 per unit | 🟠 | USD 12 per unit | 很多國家的貨幣都用$，德國客戶平常用歐元，報價一定要寫幣別（規則30） |
| 9 | Please kindly | 🟡 | Could you please | please和kindly疊用像過度客氣，讀起來僵硬（規則1） |
| 10 | revert to me | 🟠 | get back to me | revert當「回覆」是南亞商務用法，歐美讀者會理解成「恢復原狀」（規則27） |
| 11 | ASAP | 🟠 | by Friday, February 27 | ASAP沒有期限又帶催促感，給具體日期比較容易配合（規則4） |
| 12 | Welcome to contact us | 🟡 | Feel free to contact us | 中文「歡迎聯絡」直翻，Welcome to後面該接地方（規則12） |
| 13 | Look forward to hear from you | 🔴 | I look forward to hearing from you | look forward to的to是介系詞，後面要接-ing（規則21） |

**改寫後全文**

```text
Dear Mr. Weber,

This is Wilson from ABC Company. We sent the samples last Friday. Please note that the tracking number is below.
Our prices are competitive, and many customers like this model.
The goods will ship on March 4, and the price is USD 12 per unit. Could you please confirm the order and get back to me by Friday, February 27?
Thank you for choosing us. Feel free to contact us if you have any questions.
I look forward to hearing from you.
```

**文化提醒（德國客戶）**

1. 德國的日期寫法是「日.月.年」（04.03.2026），03/04很容易被讀成4月3日，月份一定要拼出來。
2. 德國商務往來通常用「Mr./Ms.＋姓」稱呼，等對方先改用名字再跟著改，不要一開始就寫Hi Thomas。
3. 德國客戶重視準確和守時，ASAP這種模糊的期限不如直接給日期，承諾的時間也要做得到。

**最值得記住的一點**：be noted、as below、revert、welcome to contact這幾個商務套話，台灣業務幾乎人人在用、也以為是對的，但歐美客戶讀起來生硬或看不懂，最值得優先改掉。
