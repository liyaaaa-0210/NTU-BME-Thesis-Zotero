# NTU BME Thesis Zotero CSL

臺灣大學生物產業機電工程學系碩博士論文 Zotero 引用格式之非官方 CSL。

> ⚠️ 本專案並非臺大生機系官方發布之引用格式。實際論文格式仍應以系所最新規定為準。

## 功能

- 臺大生機系 Author–Year 引用格式
- 中文、日文、英文文獻排序
- 中文文獻使用中文標點
- 英文文獻使用英文標點
- 支援人工指定中文姓氏筆畫排序
- Zotero 可直接安裝 `.csl`

## Zotero Language 設定

請在 Zotero 中統一設定文獻語言：

| 文獻語言 | Language |
|---|---|
| 中文 | `zh-TW` |
| 日文 | `ja` |
| 英文 | `en-US` |

此設定用於中、日、英文文獻的分組與排序。

## 中文姓氏筆畫排序

臺大生機系規定中文參考文獻依作者姓氏筆畫排列。

由於 Zotero / CSL 無法可靠地自動判斷繁體中文姓氏筆畫順序，本 CSL 使用 Zotero `Extra` 欄位中的 `Annote` 作為人工排序鍵。

例如：

```text
Language: zh-TW

Extra 欄位填上   Annote: 001
                Annote: 002
                Annote: 003等
依此類推 自行照順序排列
