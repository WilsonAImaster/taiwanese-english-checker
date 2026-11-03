# 範例：投外商的英文求職信

> 這封信的每一句，都是求職者很常寫、自己以為是對的句子。人名是虛構的。
> 結果是2026-11-03用本skill（Claude）實際執行後的輸出，經作者校對。不同AI、不同次執行，措辭會略有不同。

## 輸入

```text
To whom it may concern,

I am Kevin Lin. I am major in marketing and I have 3 years experience in social media marketing. I was responsible for our company's Instagram account.
I am a responsible and hard-working person with good communication skills. I am also familiar with Excel and Canva.
I'm very interesting in this position because I like your products very much.
Hope I can have the chance to join your company. Look forward to hear from you.

Kevin Lin
```

使用者說明：這是我的求職信

## 輸出

情境：求職

找到11個問題：4個文法錯誤、7個讀起來不自然。

| # | 原句 | 等級 | 建議改法 | 為什麼 |
|---|---|---|---|---|
| 1 | To whom it may concern, | 🟡 | Dear Hiring Manager, | 很老派，像寫給不知名單位的公文；先上LinkedIn查招募主管的名字，查不到再用Dear Hiring Manager（求職J6） |
| 2 | I am Kevin Lin. | 🟡 | I am writing to apply for the [job title] position. | 署名已經有名字了，第一句直接講你要應徵哪個職位，對方才知道這封信要放進哪一疊（規則外） |
| 3 | I am major in | 🔴 | I majored in | major當動詞要說majored in，I am major in把動詞和名詞的用法混在一起（求職J9） |
| 4 | 3 years experience | 🔴 | 3 years of experience | years和experience中間要有of，這是履歷上最容易被看到的小錯（求職J8） |
| 5 | I was responsible for our company's Instagram account | 🟡 | I managed our company's Instagram account and grew it from [number] to [number] followers | responsible for只說你「該做」，沒說你「做到」，要寫成果（求職J3） |
| 6 | I am a responsible and hard-working person with good communication skills | 🟡 | In my last campaign, I [one concrete result]. | 這三個形容詞人人都寫，招募人員會直接跳過，一件具體的事比形容詞有力（求職J2） |
| 7 | familiar with Excel and Canva | 🟡 | I use Excel (pivot tables, XLOOKUP) and Canva every day | familiar with在英文裡程度偏低，接近「用過」，要寫出具體功能或使用頻率（求職J4） |
| 8 | very interesting | 🔴 | very interested | interesting是「這件事很有趣」，寫錯會變成「我是個很有趣的人」（求職J11） |
| 9 | because I like your products very much | 🟡 | because I have used your [product] since [year], and [specific reason] | 每個應徵者都可以說喜歡你們的產品，說出具體是哪一項、為什麼，才看得出你真的了解這家公司（規則外） |
| 10 | Hope I can have the chance to join your company | 🟡 | I would welcome the opportunity to discuss how I can contribute to your team | 中文「希望有機會」很謙虛，英文讀起來像在請求施捨，結尾要有自信（求職J1） |
| 11 | Look forward to hear from you | 🔴 | I look forward to hearing from you | look forward to的to是介系詞，後面要接-ing（規則21） |

**改寫後全文**

方括號裡請換成你自己的真實內容，數字不要照抄。

```text
Dear Hiring Manager,

I am writing to apply for the [job title] position. I majored in marketing and have 3 years of experience in social media marketing. I managed our company's Instagram account and grew it from [number] to [number] followers in [number] months.
In my last campaign, I [one concrete result, e.g. led a 3-person team to launch a product video that reached 200,000 views]. I also use Excel (pivot tables, XLOOKUP) and Canva every day.
I'm very interested in this position because I have used your [product] since [year], and [specific reason].
I would welcome the opportunity to discuss how I can contribute to your team. I look forward to hearing from you.

Kevin Lin
```

**最值得記住的一點**：求職信裡每一個形容詞（responsible、hard-working、familiar with），都換成一個看得到數字的成果，這封信就會從「跟大家一樣」變成「會被記住」。
