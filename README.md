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
                Annote: 003 等

依此類推 自行照順序排列
```
## 文中引用

一般括號式引用：

```text
(Smith, 2020)
(Smith and Wang, 2020)
(Smith et al., 2020)
```
敘述式引用：

```text
Smith (2020)
Smith and Wang (2020)
Smith et al. (2020)
```
## 中文與英文參考文獻

中文文獻範例：

> 田秉才、陳世銘、馮丁樹。1989。檸檬顏色選別裝置之研製。農業工程學報 35(4): 73-82。

英文文獻範例：

> Anderson, G. T., C. V. Renard, L. M. Strein, E. C. Cayo, and M. M. Mervin. 1998. Article title. Applied Eng. in Agric. 23(2): 34-42.

中文與英文文獻會依各自格式使用不同標點。

## Based on

This CSL style was modified from the Citation Style Language (CSL) style for the American Society of Agricultural and Biological Engineers (ASABE) and adapted for NTU BME thesis formatting requirements.

Original attribution and licensing information are retained in the CSL file.

## Disclaimer

This is an unofficial community-maintained CSL style and is not officially provided or endorsed by National Taiwan University or the Department of Bio-Industrial Mechatronics Engineering.

If this CSL conflicts with the latest departmental thesis regulations, the official regulations shall prevail.
