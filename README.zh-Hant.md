# 語音輸入 (VoiceInput)

[English](README.md) · **繁體中文** · [日本語](README.ja.md)

**Mac 與 Windows 上的離線語音輸入** —— 按熱鍵說話，文字直接出現在任何 App 的游標處。本機 Whisper 辨識，支援 **60+ 語言**、**100% 離線**，語音永不離開你的電腦。**中日韓**準確度同類少見的好。

這個 repo 用來放**公開發版**。

## 下載

到 **[Releases](../../releases)** 下載最新版本：

| 平台 | 檔案 | 說明 |
|---|---|---|
| macOS | `VoiceInput-x.y.zip` | 首次啟動時下載模型（約 574MB） |
| Windows | `VoiceInput-x.y.z-setup.exe` | 已內含模型，裝完即可離線使用 |

## 安裝 — macOS

1. 下載並解壓 → 把 **VoiceInput.app** 拖到「應用程式」資料夾
2. 開啟（已用 Apple Developer ID 簽章 + 公證，不會被 Gatekeeper 擋）
3. 依首次引導：下載辨識模型、授權「麥克風」與「輔助使用」
4. 在任何 App 按熱鍵說話，文字就會插入游標處

## 安裝 — Windows

1. 執行 `VoiceInput-x.y.z-setup.exe`，不需要系統管理員權限
2. 程式常駐在系統匣，輕點 **Left Ctrl** 開始說話，再輕點一次結束
3. 系統匣圖示按右鍵可開啟設定、檔案轉錄與授權

不需要另外安裝任何東西：辨識模型與必要的函式庫都已包含在內。
GPU 加速走 **Vulkan**，執行環境由顯示卡驅動程式提供，NVIDIA、AMD、Intel 都用同一份程式。
若驅動不支援 Vulkan，會自動退回 CPU 辨識，功能一樣但速度慢很多。

> Windows 版**尚未程式碼簽章**，首次執行時 SmartScreen 會跳出警告，
> 請點「其他資訊 → 仍要執行」。簽章會在之後的版本補上。

## 系統需求

| | macOS | Windows |
|---|---|---|
| 作業系統 | macOS 14 以上 | Windows 10 以上（64 位元） |
| 建議 | Apple Silicon（M 系列） | 顯示卡驅動保持更新 |
| 磁碟空間 | 模型約 600MB | 約 700MB |

## 特色

- 本機 Whisper（large-v3-turbo），多語精準
- 100% 離線、隱私無虞
- 插字進任何 App · CJK 排版優化（中英空格、標點、簡繁）
- 中文標點自動還原
- 自訂詞庫 · 糾錯學習 · 雙語快切
- 音訊／影片檔轉錄為純文字或 SRT 字幕
- 介面語言：繁中 / 簡中 / 日文 / 英文

一組授權 **Mac 與 Windows 通用**，裝置數兩平台合計計算。

---

© 2026 momosoft · 由 Whisper 驅動，100% 本機執行
