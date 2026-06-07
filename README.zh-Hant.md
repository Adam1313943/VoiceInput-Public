# 語音輸入 (VoiceInput) for Mac

[English](README.md) · **繁體中文** · [日本語](README.ja.md)

**Mac 上的離線語音輸入** —— 按熱鍵說話，文字直接出現在任何 App 的游標處。本機 Whisper 辨識，支援 **60+ 語言**、**100% 離線**，語音永不離開你的 Mac。**中日韓**準確度同類少見的好。

這個 repo 用來放**公開發版**。

## 下載

到 **[Releases](../../releases)** 下載最新的 `VoiceInput-x.y.zip`。

## 安裝

1. 下載並解壓 → 把 **VoiceInput.app** 拖到「應用程式」資料夾
2. 開啟（已用 Apple Developer ID 簽章 + 公證，不會被 Gatekeeper 擋）
3. 依首次引導：下載辨識模型、授權「麥克風」與「輔助使用」
4. 在任何 App 按熱鍵說話，文字就會插入游標處

## 系統需求

- macOS 14 以上
- 建議 Apple Silicon（M 系列）以獲得最佳速度
- 首次使用會下載一次辨識模型（約 574MB）

## 特色

- 本機 Whisper（large-v3-turbo），多語精準
- 100% 離線、隱私無虞
- 插字進任何 App · CJK 排版優化（中英空格、標點、簡繁）
- 自訂詞庫 · 糾錯學習 · 雙語快切

---

© 2026 momosoft · 由 Whisper 驅動，100% 本機執行
