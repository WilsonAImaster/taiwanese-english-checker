# 範例：向美國總部報告的季度簡報講稿

> 這份講稿的每一句，都是上台報告時很常說、自己以為是對的句子。
> 結果是2026-11-03用本skill（Claude）實際執行後的輸出，經作者校對。不同AI、不同次執行，措辭會略有不同。

## 輸入

```text
OK, today I want to introduce our Q3 sales data.
As you can see in the picture, our sales went up. Our revenue is 3 billion NT dollars (3億台幣) this quarter.
Our market share rose from 10% to 15%, an increase of 5%.
Next page.
That's all. Thank you.

(Q&A)
Your question is very good. I'm not sure... maybe 30%?
```

使用者說明：這是我的簡報講稿，聽眾是美國總部

## 輸出

情境：簡報與會議發言

找到8個問題：2個文法錯誤、1個可能造成誤會、5個讀起來不自然。

| # | 原句 | 等級 | 建議改法 | 為什麼 |
|---|---|---|---|---|
| 1 | today I want to introduce our Q3 sales data | 🟡 | Today I'll walk you through our Q3 sales results | introduce適合介紹人或新產品，講解資料用walk you through；I want to也比I'll弱（簡報P1） |
| 2 | As you can see in the picture, our sales went up | 🟡 | As you can see in this chart, our sales rose [20%] in Q3 | picture通常指照片，圖表要說chart；順便講出你要大家看到的數字（簡報P4） |
| 3 | 3 billion NT dollars (3億台幣) | 🔴 | 300 million NT dollars | 3億是300 million，3 billion是30億，差了十倍（簡報P8） |
| 4 | an increase of 5% | 🔴 | an increase of 5 percentage points | 從10%到15%是增加5個百分點，換算成成長率其實是50%（簡報P7） |
| 5 | Next page. | 🟡 | On the next slide, you'll see [topic]. | 簡報的一頁叫slide；轉場時說下一頁要講什麼，聽眾比較跟得上（簡報P2） |
| 6 | That's all. Thank you. | 🟡 | To sum up, [one key point]. Thank you. I'm happy to take any questions. | That's all讓結尾很突然，先用一句話總結，再邀請提問（簡報P3） |
| 7 | Your question is very good. | 🟡 | That's a great question. | 中文「你的問題很好」直翻，英文的固定說法是That's a great question（簡報P5） |
| 8 | I'm not sure... maybe 30%? | 🟠 | I don't have that number with me. I'll check and follow up with you after the meeting. | 不確定時亂猜，比承認不知道更傷專業度，說清楚你會補上答案（簡報P6） |

**改寫後全文**

方括號裡請換成你簡報的真實內容。

```text
Today I'll walk you through our Q3 sales results.
As you can see in this chart, our sales rose [20%] in Q3. Our revenue is 300 million NT dollars this quarter.
Our market share rose from 10% to 15%, an increase of 5 percentage points.
On the next slide, you'll see [topic].
To sum up, [one key point]. Thank you. I'm happy to take any questions.

(Q&A)
That's a great question. I don't have that number with me. I'll check and follow up with you after the meeting.
```

**文化提醒（美國總部）**

1. 美國主管習慣先聽結論，開場第一句就可以講最重要的數字（例如營收或成長率），細節放後面。
2. 總部平常看美金，大數字旁邊補一句約當美金（例如about USD 9.5 million），對方不用自己換算。
3. 說了I'll follow up就要真的做，會後當天寄一封Email補上數字，比在台上猜對更加分。

**最值得記住的一點**：上台前把所有「萬、億」先換算成英文數字寫在講稿上，現場才不會在數字上卡住或差十倍。
