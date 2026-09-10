# 自然科 Kahoot 多元評量設計師

這是一套給國小自然科教師使用的 Agent Skill，適合單元教學、期中考與期末考複習，可設計前測、形成性評量、後測與 Kahoot 題庫。

## 主要功能

- 先以文字確認年級、單元、學習重點與評量用途
- 以複選清單選擇題型與輸出格式
- 設計單選、是非、多選、資料判讀、實驗與情境應用題
- 加入合理誘答，診斷學生迷思概念
- 執行評量品質驗證與自然科學查證
- 產生 Kahoot 官方 `.xlsx` 匯入題庫與教師版檔案
- 取得作答報告後分析答對率、難度、鑑別度與錯誤選項

## 檔案結構

```text
natural-science-kahoot-assessment/
├── SKILL.md
├── README.md
└── agents/
    └── openai.yaml
```

## 在 Codex 使用

將整個資料夾放入 Codex 的 skills 目錄，重新載入技能後即可使用：

```text
$natural-science-kahoot-assessment
```

## 在其他 AI Agent 使用

若代理支援 Agent Skills，保留 `SKILL.md` 與 `agents/openai.yaml` 即可。若不支援技能目錄，可將 `SKILL.md` 的內容放入該代理的 system prompt、project rules 或 agent instructions。

## Kahoot 格式提醒

`.xlsx` 是 Kahoot 試算表題庫匯入格式。是非題會以「是／否」兩個選項呈現，多選題則使用 `Correct answer(s)` 欄位記錄多個答案編號。PDF、PowerPoint、Google Slides、URL 等屬於 Kahoot AI 產題素材或同步來源，不等同於試算表直接匯入。

## 分享到 GitHub

可將本資料夾上傳至公開或私人 GitHub repository。建議保留此資料夾名稱，方便日後安裝與版本更新。

```bash
git add natural-science-kahoot-assessment
git commit -m "Add natural science Kahoot assessment skill"
git push
```

本技能不包含 API 金鑰或個人資料。
