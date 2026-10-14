# 台式英文抓蟲器 · Taiwanese English Checker

繁體中文 | [English](README.en.md)

> 貼上你的英文Email，AI幫你抓出台式英文：外國人讀起來哪裡怪、為什麼，再給你自然的改法。
> 一個給AI用的skill（`SKILL.md`）。專抓**英文不錯的人也常寫、自己以為是對的**30條台式英文。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

**👉 介紹頁＋免費線上試用：https://wilsonaimaster.github.io/taiwanese-english-checker/**

---

## 為什麼做這個

這些句子，你可能每天都在寫，而且覺得完全沒問題：

- `Look forward to hear from you.`：to後面要接-ing，幾乎每封台式英文信都有
- `Please be noted that…`：英文其實要說Please note that
- `Welcome to contact us.`：中文「歡迎聯絡」直翻，英文說Feel free to contact us
- `Please revert to me.`：美國客戶可能看不懂你要他做什麼
- `The goods will ship on 03/04.`：歐洲客戶會以為是4月3日

外國客戶通常不會糾正你，但會影響他們對你的專業印象。

一般的AI改寫只會幫你「改好」，不會告訴你**為什麼**。下次你還是會寫錯。

這個skill讓AI用英文老師的方式檢查：**每個問題都分等級、講原因、標規則編號**，最後挑出一個最值得記住的習慣。改一次、學一次。

## 效果

**修改前**

```text
Dear Mr. Thomas,

Here is Wilson from ABC Company. We have sent the samples last Friday. Please be noted that the tracking number is as below.
Our price is cheap and there are many customers like this model.
The goods will ship on 03/04 and the price is $12 per unit. Please kindly confirm the order and revert to me ASAP.
Thank you for choosing us. Welcome to contact us if you have any questions.
Look forward to hear from you.
```

**AI抓到的問題（節錄）**

| 原句 | 等級 | 建議改法 | 為什麼 |
|---|---|---|---|
| Dear Mr. Thomas | 🟠 誤會 | Dear Mr. Weber | Mr.後面要接姓，不是名字 |
| We have sent the samples last Friday | 🔴 錯誤 | We sent the samples last Friday | 有明確過去時間，不能用現在完成式 |
| Please be noted that…as below | 🔴 錯誤 | Please note that…below | be noted的主詞該是事，不是人 |
| Our price is cheap | 🟠 誤會 | Our prices are competitive | cheap常帶「廉價、品質差」的意思 |
| Look forward to hear from you | 🔴 錯誤 | I look forward to hearing from you | look forward to的to是介系詞，要接-ing |

**修改後**

```text
Dear Mr. Weber,

This is Wilson from ABC Company. We sent the samples last Friday. Please note that the tracking number is below.
Our prices are competitive, and many customers like this model.
The goods will ship on March 4, and the price is USD 12 per unit. Could you please confirm the order and get back to me by Friday, February 27?
Thank you for choosing us. Feel free to contact us if you have any questions.
I look forward to hearing from you.
```

完整輸出（13個問題＋文化提醒）見[examples/client-email.md](examples/client-email.md)。

## 30條地雷，分四類

| 類別 | 例子 |
|---|---|
| 語氣與禮貌 | Please kindly、I want to、ASAP、Hope you can understand、Our price is cheap |
| 中文直翻 | contact with、Welcome to contact us、Wish you have a nice day、There are many people like… |
| 文法常錯 | feedbacks／staffs、We have sent it yesterday、Look forward to hear from you、Here is Wilson |
| 商務Email習慣 | Mr. + 名字、Please be noted that、as below、revert、日期03/04、金額只寫$ |

完整規則和例句：[references/rules.md](references/rules.md)

## 7個情境包

不只寫給外國客戶的信。告訴AI這是什麼文件（或讓它自己判斷），它會在30條通用規則之外，再套用該情境專屬的規則：

| 情境 | 代號 | 適用 | 例子 |
|---|---|---|---|
| [求職](references/scenarios/job.md) | J | 履歷、求職信、LinkedIn簡介、面試 | Hope I can have the chance to…、3 years experience、I am major in… |
| [外商職場](references/scenarios/workplace.md) | W | 同事與主管、Teams／Slack、會議、週報 | Please help to check、只回Noted.、Let me double confirm |
| [簡報與會議發言](references/scenarios/presentation.md) | P | 簡報開場、轉場、數據、Q&A | Next page、That's all. Thank you.、百分比和百分點 |
| [跨境電商與客服](references/scenarios/ecommerce.md) | E | 商品頁、回覆買家、退貨、評價 | We will try our best、Please understand、請買家給五星 |
| [學術與升學](references/scenarios/academic.md) | A | 讀書計畫、論文、投稿信 | With the development of…、researches、such as…etc. |
| [社群與個人品牌](references/scenarios/social.md) | S | LinkedIn、IG、YouTube | Welcome to follow me、recommend you to… |
| [旅遊與生活](references/scenarios/travel.md) | T | 訂房、點餐、問路、客訴 | Give me a coffee、luggages、Is here the bus stop? |

用法很簡單，在貼上英文時多說一句就好，例如「這是我的求職信」「這是要回給同事的Teams訊息」。

## 安裝

### Claude Code

```bash
git clone https://github.com/WilsonAImaster/taiwanese-english-checker ~/.claude/skills/taiwanese-english-checker
```

之後直接說「幫我檢查這封信有沒有台式英文」，再貼上內容。

### 其他支援SKILL.md的AI工具

把整個資料夾放進該工具的skills資料夾。

### ChatGPT、Claude、Gemini網頁版

不用安裝：把[SKILL.md](SKILL.md)和[references/rules.md](references/rules.md)的內容貼進「專案」或「自訂指令」，之後在對話裡貼上英文就好。

## 使用小技巧

- **告訴它收件人是哪國人**（例如「收件人是德國客戶」），會多一段文化提醒。
- **它不會過度修改**：寫對的句子不會被挑出來，沒問題就會直接說沒有。
- **每次只看「最值得記住的一點」**：一次改掉一個習慣，比一次記30條有效。
- AI也會出錯。重要的信，改完自己再讀一遍。

## 一起讓規則更好

這份規則會持續更新，歡迎一起補：

- **遇過其他台式英文？** → [分享一個台式英文](https://github.com/WilsonAImaster/taiwanese-english-checker/issues/new?template=new-pattern.yml)
- **覺得某條規則不對？** → [回報規則有誤](https://github.com/WilsonAImaster/taiwanese-english-checker/issues/new?template=rule-error.yml)

被採用的例子，會在這裡致謝你的GitHub帳號。

想在新增情境包或規則時收到通知？加入[Skool免費社群](https://www.skool.com/wilson-9076)，每次更新都會在那裡公告。

## 關於作者

Wilson，英文老師，教學16年，研究怎麼用AI讓英文真的派上用場。

這些規則挑的是英文不錯的人也常寫、最容易造成誤會的句子。發現規則有誤，或遇過其他台式英文，歡迎[開issue](https://github.com/WilsonAImaster/taiwanese-english-checker/issues)告訴我。

想要更多AI工具實測？[網站](https://wilsonaienglish.com/)・[YouTube](https://www.youtube.com/@WilsonAILab)・[Skool](https://www.skool.com/wilson-9076)・[Instagram](https://www.instagram.com/wilsonailab/)・[Threads](https://www.threads.com/@wilsonailab)

## 授權

MIT。歡迎使用、修改、分享，請保留出處。
