# # 臺大生機系論文 Zotero 引用格式

臺灣大學生物產業機電工程學系碩博士論文使用之非官方 Zotero CSL 樣式。

> [!IMPORTANT]
> 本專案並非臺大生機系官方發布之引用格式。
> Zotero 的基本安裝、書目匯入、Word 引用與引用格式操作，建議先參考臺灣大學圖書館官方 Zotero 教學。
> 本專案主要補充「臺大生機系論文引用格式」以及中英文文獻排序與格式設定。

## 📚 Zotero 基本教學

第一次使用 Zotero 的同學，建議先閱讀臺灣大學圖書館提供的：

### [書目管理軟體 Zotero 指引第一站](https://tul.blog.ntu.edu.tw/archives/37353)

內容包含：

- Zotero 安裝
- Zotero Connector
- 文獻資料匯入
- 文獻管理
- Microsoft Word 引用
- Bibliography 建立
- Citation Style 設定

---
## 🔧 本專案提供什麼？

本專案主要針對臺大生機系碩博士論文引用格式進行調整，包括：

- Author–Year 文中引用格式
- 中文、日文、英文文獻排序
- 中文文獻標點格式
- 英文文獻作者格式
- 同一作者依發表年份排序
- 中文姓氏筆畫人工排序方式
- Zotero `Language` 欄位設定
- Zotero `Extra / Annote` 欄位設定

本專案主要補充：

> **臺大生機系論文引用格式、中英文文獻格式與排序設定。**

---

# 📥 1. 安裝 NTU BME Thesis CSL

## Step 1：進入 Zotero Settings

開啟 Zotero 後：

`Edit → Settings`

![Open Zotero Settings](images/01-zotero-settings.png)

---

## Step 2：進入 Cite

在 Settings 左側選擇：

`Cite`

接著按：

`Add from File...`

![Add CSL Style](images/02-add-csl-style.png)

---

## Step 3：選擇 CSL 檔案

選擇本專案提供的：

NTU-BME-Thesis.csl

![Add CSL Style](images/03-select-csl-file.png)

# 📝 2. 在 Microsoft Word 套用格式

開啟 Word 後，進入：

`Zotero → Document Preferences`

![Add CSL Style](images/04-word-document-preferences.png)

在 Citation Style 中選擇：

`NTU-BME-Thesis`

![Add CSL Style](images/10-choose-style-in-word.png)


# 🌏 3. Language 設定

請在 Zotero 中統一設定文獻語言：

| 文獻語言 | Language |
|---|---|
| 中文 | `zh-TW` |
| 日文 | `ja` |
| 英文 | `en-US` |

此設定用於中、日、英文文獻的分組與排序。

中文:

![Add CSL Style](images/11-chinese-language.png)

英文:

![Add CSL Style](images/07-english-language.png)

請不要混用：
```text
Chinese
中文
Traditional Chinese
zh_TW
English
ENG
```

---

# 🇨🇳 4. 中文文獻設定

中文文獻的：
```text
Language
```
請設定成：
```text
zh-TW
```
另外，由於臺大生機系規定：

> **中文文獻應依作者姓氏筆畫順序排列。**
> 
目前 Zotero / CSL 無法可靠自動判斷繁體中文姓氏筆畫，因此本 CSL 使用 Zotero 的 `Extra `欄位人工指定排序。
例如第一順位：
```text
Language: zh-TW

Extra:
Annote: 001
```
![Add CSL Style](images/05-chinese-language-order-001.png)

下一順位：
```text
Language: zh-TW

Extra:
Annote: 002
```
![Add CSL Style](images/06-chinese-language-order-002.png)

依此類推：
```text
Annote: 001
Annote: 002
Annote: 003
...
Annote: 010
Annote: 011
```
> **⚠️ `Annote` 除了作為中文文獻排序鍵，也用來觸發本 CSL 的中文格式，例如中文句號 `。`。**

# 🇺🇸 5. 英文文獻設定

中文文獻的：
```text
Language
```
請設定成：
```text
en-US
```
![Add CSL Style](images/07-english-language.png)

---
英文文獻的 `Extra` 不需要加入 `Annote`。
例如：
```text
Language: en-US

Extra:
（留空）
```
# 🔤 6. 文獻排序規則

臺大生機系論文參考文獻要求依：
1. 中文
2. 日文
3. 英文／歐文
排列。
同一作者有數篇文獻時，再依發表年份由舊至新排列。
本 CSL 的排序概念為：

```text
Language
↓
Chinese manual stroke-order key
↓
Author
↓
Year
↓
Title
```
因此請務必確認每篇英文文獻都有：
```text
Language: en-US
```
如果英文文獻沒有填寫 Language，可能會造成英文文獻無法正常依姓氏字母排序。

# ✍️ 7. 中文文獻格式

本csl檔已經設定好，當語言`zh-TW`會用`。` ， 語言`en-US`會用`.`


中文文獻範例：

> 田秉才、陳世銘、馮丁樹。1989。檸檬顏色選別裝置之研製。農業工程學報 35(4): 73-82。

英文文獻範例：

> Anderson, G. T., C. V. Renard, L. M. Strein, E. C. Cayo, and M. M. Mervin. 1998. Article title. Applied Eng. in Agric. 23(2): 34-42.

中文與英文文獻會依各自格式使用不同標點。

# 🔠 8. 英文文獻格式

英文文獻例如：
```text
Anderson, G. T., C. V. Renard, L. M. Strein, E. C. Cayo, and M. M. Mervin. 1998. Article title. Applied Eng. in Agric. 23(2): 34-42.
```
英文作者格式：
第一作者：

```text
Anderson, G. T.
```
第二作者之後：

```text
C. V. Renard
```
最後一位作者前使用：

```text
and
```

# 📖 9. 文中引用格式

## 括號式引用
一位作者：

```text
(Smith, 2020)
```
兩位作者：
```text
(Smith and Wang, 2020)
```
三位以上：
```text
(Smith et al., 2020)
```

## 敘述式引用：

如果作者名稱已經出現在句子中：

```text
Smith (2020) reported that ...
```
或：
```text
Smith et al. (2020) found that ...
```
在 Zotero Word Plugin 中可使用：

```text
Omit Author / Suppress Author
```
讓 Zotero 僅產生年份。

![Add CSL Style](images/12-omit-author.png)

應該在內文中顯示:

```text
(2014)
```

---

# 🛠️ 10. 修改 CSL

如果需要自行調整 CSL，可以使用 Zotero 內建的 Style Editor。

![Add CSL Style](images/01-zotero-settings.png)

進入：

`Settings → Cite`

往下找到：

`Style Editor`

![Add CSL Style](images/08-style-editor.png)

開啟後即可查看與修改 CSL 程式碼：

![Add CSL Style](images/09-style-code.png)

修改完成後，可以使用：

```text
Save As...
```

另存新的 `.csl`。

> **建議修改前先備份原本的 CSL。**
>
# ⚠️ 注意事項

正式提交論文前，建議人工再次確認：
- 中文文獻是否位於最前方
- 日文是否位於中文與英文之間
- 英文文獻是否依作者姓氏 A–Z 排列
- 中文姓氏是否符合筆畫順序
- 同一作者是否依年份由舊至新排列
- 中文文獻是否使用 `。`
- 英文文獻是否使用 `.`
- Journal abbreviation 是否正確
- Thesis、Book、Conference 等特殊文獻類型是否符合系所規範

---

# 🦈 最後的小小祝福 🦈

**祝每一位看到這裡的人，都能順利寫完論文、順利口試、順利畢業！🎓**

希望這份 CSL 可以幫大家省下一點整理格式的時間。  
少一點被 Zotero 搞到崩潰，多一點時間好好做研究 XD

**畢業加油！🦈🦈🦈**

---


## 📌 Based on

本 CSL 以：
American Society of Agricultural and Biological Engineers (ASABE)
Citation Style Language 為基礎進行修改，並依臺大生機系論文撰寫格式進行調整。
原始 CSL 的作者與授權資訊保留於 `.csl `檔案中。

## ⚠️ Disclaimer

This is an unofficial community-maintained CSL style.
本專案不是臺灣大學或臺灣大學生物產業機電工程學系官方發布之 Citation Style。
若本 CSL 與系所最新論文格式規範有所衝突：
> **請以系所官方最新規定為準。**

