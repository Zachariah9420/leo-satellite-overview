# 🛰 The Internet in the Sky

**LEO 低軌道衛星通訊 — 當基地台搬上太空**

> 行動與無線系統概論 · 2026 Spring · 期末調查報告

一份 17 張投影片的單檔 HTML 簡報，介紹 LEO 衛星網路（以 Starlink 為主案例），涵蓋系統架構、Massive MIMO 物理層挑戰、sCSI 解法、真實量測，以及 6G 非地面網路（NTN）的應用與前沿研究。

---

## 🚀 線上觀看

> 📺 **[啟動簡報](https://Zachariah9420.github.io/leo-satellite-overview/)**

> 🎬 **YouTube 影片版：** 

按 `→` 鍵 / 空白鍵翻頁；`F11` 全螢幕；`Esc` 跳出。

---

## 📋 涵蓋主題

| # | Slide | 內容 |
|---|---|---|
| 1 | Cover | 標題 |
| 2 | Hook | 你今天用過衛星了嗎? |
| 3 | Motivation | 為什麼需要天上的網路 |
| 4 | Orbits | GEO vs MEO vs LEO 比較 |
| 5 | Perfect Storm | LEO 為什麼現在才紅 |
| 6 | Architecture | Starlink end-to-end 系統 |
| 7 | Scale | 10,296 顆衛星的規模 |
| 8 | Cellular vs LEO | 基地台會跑！ |
| 9 | Massive MIMO | 多天線多波束 |
| 10 | MIMO Challenges | Doppler & iCSI 拿不到 |
| 11 | sCSI Solution | 統計通道資訊 |
| 12 | Measurements | Starlink 真實效能 |
| 13 | Environment | Killer 數據：LEO vs GEO 雨衰 |
| 14 | Applications | 6 大場景 + 6G NTN |
| 15 | Frontier | 2025 前沿研究 |
| 16 | Summary | 收尾三件事 |
| 17 | References | 13 篇參考文獻 |

---

## 🛠 技術細節

- 單檔 HTML（CSS / JS 全部 inline，雙擊即開）
- 解析度 1920×1080，黑底 Apple Keynote 風
- 使用原生 Web Components (`<deck-stage>`)
- SVG 自繪所有架構圖、軌道圖、波形圖
- 內嵌 speaker notes JSON

---

## 📚 主要參考文獻

1. Ma, S. et al. *Network Characteristics of LEO Satellite Constellations: A Starlink-Based Measurement from End Users.* **IEEE INFOCOM 2023.**
2. You, L. et al. *Massive MIMO Transmission for LEO Satellite Communications.* **IEEE JSAC**, vol. 38, no. 8, 2020.
3. Su, Y. et al. *Broadband LEO Satellite Communications: Architectures and Key Technologies.* **IEEE Wireless Communications**, 2019.

### 補充研究（2024–2026）

4. Brashears, T. *Achieving 99% link uptime on 100G space laser ISLs.* SPIE FSLC XXXVI 2024.
5. Garcia, J. et al. *A Detailed Characterization of Starlink One-way Delay.* LEO-NET Workshop 2025.
6. Bülo, M. et al. *Crowdsourced Starlink Performance Measurements.* IEEE ICC 2024.
7. Shukur, H. et al. *Latency Performance of LEO Starlink vs SES-12 GEO under Tropical Rainfall.* IIUM Eng. J. 2025.
8. Ullah, M. A. et al. *A First Look at Starlink In-Flight Performance.* ComComAp 2025.
9. Dong, Q. et al. *Statistical CSI-Based Beamspace Transmission for Massive MIMO LEO.* Entropy 2025.
10. Li, Q. et al. *Holographic Metasurface-Based Beamforming for Multi-Altitude LEO.* IEEE TWC 2025.
11. Baena, E. et al. *Space-O-RAN: Enabling Intelligent, Open NTNs in 6G.* IEEE Comm. Mag. 2025.
12. Jamshed, M. A. et al. *A Tutorial on Non-Terrestrial Networks: Towards Global 6G Connectivity.* arXiv/IEEE 2024.

---

## 📁 專案結構

```
leo-satellite-overview/
├── index.html                  # 簡報主檔（單檔自包含）
├── README.md
├── docs/
│   ├── slide_content.md        # 每頁內文 markdown
│   └── youtube_chapters.txt    # YouTube 章節時間戳
└── subtitles/
    └── subtitles_zh-tw.srt     # 繁體中文字幕（影片用）
```

---

## 👤 作者

**劉彥志** · 113368502
🏫 國立臺北科技大學 電子系
📅 行動與無線系統概論 2026 Spring
👨‍🏫 授課教師：陳彥安 教授

---

## 📜 授權

本作品為課程作業，僅供學術參考。投影片內容引用之圖示與數據各歸原始出處所有。

---

