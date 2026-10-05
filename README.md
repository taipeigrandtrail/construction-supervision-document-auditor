# 監造月報及相關文書審核 Skill

`construction-supervision-document-auditor` 是供 Codex 使用的公共工程文件審核 Skill，用於檢核監造月報、監造日報、施工日誌、自主檢查表、防汛檢查、督導紀錄、材料檢試驗文件及照片佐證。

## 功能

- 建立送審文件清冊及日期索引。
- 交叉核對每日工項、進度、天氣與出工人數。
- 檢核防汛及督導頻率、簽章、照片獨立性與材料試驗追溯性。
- 依證據區分符合、不符合、待確認及不適用。
- 對外僅輸出具精確證據的重大缺失。
- 產出 A4 橫式 ODT「監造月報缺失改善表」，包含六欄主表及紅圈圖片附件。

## 安裝

將本儲存庫複製至 Codex skills 目錄：

```text
~/.codex/skills/construction-supervision-document-auditor/
```

或以 Skill Installer 從 GitHub 儲存庫安裝。

## 使用方式

在 Codex 中指定：

```text
使用 $construction-supervision-document-auditor 審核這份監造月報及相關文書。
```

請一併提供需審核的 PDF、DOCX、XLSX 或圖片。原始文件維持唯讀，Skill 僅建立審核成果。

## 審核邊界

- 不因「未看到」即推定不符合；無法確認時列為待確認。
- 不做人臉辨識，不依筆跡推斷簽署人身分。
- 照片相似僅能列為疑似重複，不直接認定造假。
- 未提供契約、圖說或材料規範時，不臆造允收值。
- 最新表格格式應以主管機關正式版本或使用者提供範本為準。

## 儲存庫資料範圍

本儲存庫不包含真實工程月報、簽章、照片、個人資料或審核成品。

## 授權

MIT License。
