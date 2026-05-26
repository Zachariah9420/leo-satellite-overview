# LEO 衛星簡報 — 投影片內文初稿

**主題**：The Internet in the Sky — LEO 衛星通訊：當基地台搬上太空
**課程**：行動與無線系統概論 2026 Spring
**時長**：15 分鐘 / 17 張投影片
**風格**：黑底 Apple keynote 風、中英混模

---

## Slide 1 — Cover

**主標**：The Internet in the Sky
**副標**：當基地台搬上太空 — LEO 衛星通訊
**底部**：行動與無線系統概論 2026 Spring｜學生姓名｜學號
**視覺**：地球從太空視角 + 一圈 LEO constellation 線條（橘色光點），右下角小衛星 icon

**口播**：「大家好，今天我要帶大家從地面飛到 350 公里高的太空，看看一個正在改變網路版圖的技術 — LEO 低軌道衛星通訊。」

---

## Slide 2 — Hook：你今天用過衛星了嗎？

**主標**：你今天用過衛星了嗎？
**三欄並列（圖+一行字）**：
- 📱 **iPhone 14+ Emergency SOS** — 沒訊號時，靠衛星發 SOS
- 🇺🇦 **烏俄戰場** — Starlink 終端成為前線通訊命脈
- 🏫 **偏鄉學校** — Starlink 把網路帶到光纖到不了的地方

**底部一行**：This is not sci-fi. This is **now**.

**口播**：「不知不覺中，衛星已經滲透進我們的日常。iPhone 的 SOS、戰場上的通訊、偏鄉的教育網路 — 背後都是低軌衛星在運作。」

---

## Slide 3 — 為什麼需要衛星網路？

**主標**：Why satellites? Why now?
**重點數字（大字）**：
- **2.6 Billion** 全球至今仍無穩定網路存取（ITU 2023）
- **30%** 地球表面無 cellular 覆蓋（海洋、極地、沙漠）

**條列**：
- 地面建設受地形限制（山區、海洋、沙漠）
- 海底電纜易被破壞（台灣 2023 馬祖斷纜事件）
- 偏鄉布建成本回收期長

**結論句**：If we can't build down, we build up. 👆

**口播**：「為什麼要把網路搬上太空？因為地球上還有 2/3 的地方沒有穩定網路。地形、海洋、成本，都讓地面基地台到不了。」

---

## Slide 4 — GEO vs MEO vs LEO

**主標**：軌道高度決定一切
**比較表**：

| 類型 | 高度 | 延遲 (RTT) | 覆蓋一顆 | 代表 |
|------|------|-----------|---------|------|
| **GEO** | 35,786 km | ~600 ms | 1/3 地球 | 衛星電視 |
| **MEO** | 2,000–35,786 km | ~125 ms | 大範圍 | GPS |
| **LEO** | 160–2,000 km | **25–60 ms** | 小（需密集） | Starlink |

**視覺**：地球橫剖面 + 三層軌道環（不同色），箭頭標示高度

**口播**：「衛星不是新東西。但 LEO 低軌衛星的延遲只有 25 到 60 毫秒，跟地面 4G/5G 同一個量級 — 這是 LEO 跟傳統 GEO 衛星最大的差別。」

---

## Slide 5 — LEO 為什麼現在才紅？

**主標**：The Perfect Storm — 三大要素到位
**三欄**：
- 🚀 **可回收火箭** — SpaceX Falcon 9 讓發射成本降 **~10x**
- 🛰️ **衛星量產** — Starlink v2 ~ 800 kg，單次 batch 部署 22+ 顆
- 📡 **用戶終端降價** — 從 1990s Iridium 的 \$3,000 → Starlink \$349

**時間軸（底部）**：
1990s Iridium 倒閉 ❌ → 2015 SpaceX 提案 → 2019 首發 → **2026: 10,296 顆在軌**

**口播**：「為什麼 1990 年代 Iridium 倒閉，但 Starlink 成功？三件事改變了：火箭可回收、衛星量產化、用戶終端便宜十倍。」

---

## Slide 6 — Starlink 系統架構（Paper 3 + SpaceX 2024）

**主標**：Starlink Architecture — End-to-End
**視覺（核心圖）**：橫向流程圖
```
[用戶終端 UT] ⇄ [LEO 衛星] ⇄ [ISL 衛星間光鏈路] ⇄ [Ground Gateway] ⇄ [PoP] ⇄ [Internet]
```

**條列說明**：
- **UT (User Terminal)**：相位陣列天線盤
- **ISL (Inter-Satellite Link)**：v1.5+ 衛星具備雷射光鏈路
- **Walker constellation**：星座採 Walker Delta 設計（Paper 3）
- **混合波束覆蓋**：寬波束 + 點波束（Paper 3）

**🔥 SpaceX 官方數據（Brashears 2024）**：
- 已部署 **5,000+ 雷射光通訊終端**
- 每條鏈路 **100 Gbps**
- 鏈路 uptime **99%**

**Cite**：Su et al., IEEE Wireless Comm 2019｜Brashears, SPIE Free-Space Laser Comm XXXVI 2024

**口播**：「Starlink 不是只有衛星 — 它是一整套系統。SpaceX 自家工程師 2024 年發表的數據顯示：他們已經部署超過 5000 個雷射光終端，每條鏈路 100Gbps，可用率 99% — 這是太空中規模最大的光通訊網路。」

---

## Slide 7 — 規模震撼

**主標**：By the Numbers (May 2026)
**四大數字（大字）**：
- **10,296** 顆衛星在軌
- **11,529** 累計發射
- **~4 Million** 全球用戶
- **70+** 個國家服務中（包含 🇹🇼）

**視覺**：右側顯示 Starlink 軌道密度動畫截圖

**口播**：「這個規模 5 年前無法想像。現在 SpaceX 平均每週發射一次，每次 22 顆。台灣也是服務國之一。」

---

## Slide 8 — Cellular vs LEO（接 lec11）⭐

**主標**：上週老師教的 Cellular，跟天上的 LEO 有什麼差別？
**左右對比**：

| 維度 | **Terrestrial Cellular** | **LEO Satellite** |
|------|-------------------------|-------------------|
| 基地台 | 地面固定 BS | LEO 衛星（移動中）|
| 細胞 | Hexagonal cell（lec11） | Satellite footprint（橢圓）|
| Handover | 數分鐘一次（人移動）| **每 ~15 秒一次**（衛星移動！）|
| 衛星速度 | 0 | **7.5 km/s** |
| 都卜勒效應 | 可忽略 | **嚴重**（後面詳談）|

**重點橘字**：基地台會跑！這帶來全新挑戰。

**🔬 證據**：Garcia 2025 用 10 天收集 **5 億個 probe 封包**，量化證實了 Starlink 每 15 秒的 reconfiguration 週期。

**Cite**：Garcia et al., LEO-NET Workshop 2025

**口播**：「老師上週教 cellular 時，基地台是站好不動的。在 LEO 完全反過來 — 衛星以每秒 7.5 公里高速飛行，每 15 秒你就要 handover 一次。2025 年 Garcia 等人用 5 億個封包證實了這個 15 秒週期。這帶來兩個關鍵問題：handover 頻繁、都卜勒嚴重。」

---

## Slide 9 — 核心技術：Massive MIMO 是什麼？

**主標**：Massive MIMO — 一顆衛星同時服務很多人
**視覺**：左圖一根天線打一個信號 vs 右圖多天線陣列打多個 beam（多色波束）

**條列**：
- **MIMO** = Multiple-Input Multiple-Output
- 多根天線 → **同時形成多個波束**（beamforming）
- 每個波束服務不同用戶 → **頻譜利用率大幅提升**
- 4G/5G 地面已標配；衛星才剛開始

**重點**：More antennas, more users, more capacity. 同一個頻段服務多人。

**口播**：「Massive MIMO 在 4G/5G 地面是已知技術。簡單講就是：一個基地台用很多天線同時打很多波束，每個波束服務一個用戶，達到頻率重用。」

---

## Slide 10 — LEO 上的 Massive MIMO 為什麼難？（Paper 2 核心 1/2）

**主標**：LEO 把 Massive MIMO 變得超難
**兩大挑戰（橘色標題）**：

### 🌀 挑戰 1：嚴重 Doppler shift
- 衛星 7.5 km/s 高速飛行 → 信號頻率被「拉伸/壓縮」
- 地面 cellular Doppler 可忽略；LEO 完全不行

### 📡 挑戰 2：iCSI 取得困難
- 傳統 Massive MIMO 需要 **instantaneous CSI**（瞬時通道資訊）
- LEO 通道變化太快、來回延遲長 → iCSI 拿到時已過時

**底部橘字結論**：⛔ 傳統地面 Massive MIMO 方法不能直接用

**口播**：「在地面，Massive MIMO 仰賴的『瞬時通道資訊』在 LEO 拿不到 — 因為衛星跑太快、來回延遲太長，等你拿到資訊，通道狀態已經變了。Doppler 效應也讓信號頻率漂移嚴重。」

---

## Slide 11 — sCSI 解法（Paper 2 核心 2/2）

**主標**：解法 — 用統計通道資訊（sCSI）
**核心 idea（中央大字）**：
> 拿不到瞬時 CSI？那就用**統計 CSI**。

**條列**：
- **sCSI (statistical CSI)** = 通道的長時間統計特性
- 不隨衛星位置劇烈變化 → 適合 LEO 高速場景
- 用戶端先做 **Doppler / delay 補償**
- 衛星端用 sCSI 設計低複雜度預編碼（precoding）

**目標**：
- ↑ 下行：最大化 **ASLNR**（Average Signal-to-Leakage-plus-Noise Ratio）
- ↑ 上行：最大化 **ASINR**（Average Signal-to-Interference-plus-Noise Ratio）

**📈 2025 最新進展**：Dong 等人把 sCSI 擴展到 **beamspace 域**，用 WMMSE 進一步降低計算複雜度。

**Cite**：You et al., IEEE JSAC 2020｜Dong et al., Entropy 2025

**口播**：「You 等人 2020 年提出一個很聰明的想法：拿不到瞬時資訊，那就用『統計上會長這樣』的資訊。這個概念到 2025 年還在演進 — Dong 等人最新研究把它延伸到 beamspace 域，計算量更低。配上用戶端的 Doppler 補償，就能用 Massive MIMO 在 LEO 服務多用戶。」

---

## Slide 12 — 真實量測（Paper 1）

**主標**：Starlink 在真實世界跑得怎樣？
**研究方法**：
- 多個 Starlink 終端 × 多地點
- 工具：`iperf3`（吞吐）、`ping`（延遲）、`traceroute`（路由）、串流測試

**主要發現（左右兩欄）**：

| 📊 Throughput | ⏱ Latency |
|---------------|-----------|
| 中位數 100–200 Mbps | 中位數 25–50 ms |
| **變動劇烈** | **週期性尖峰**（handover）|
| 偶發 outage | 偶發 spike 到 200+ ms |

**金句**：Starlink works — but it's **not** a smooth terrestrial fiber.

**🌐 跨研究交叉驗證**：
- **Bülo 2024**（crowdsourced）：170 萬筆量測、309 用戶、29 國 → 數字非常一致
- **Garcia 2025**（精準）：5 億封包證實 15 秒週期性延遲尖峰

**Cite**：Ma et al., IEEE INFOCOM 2023｜Bülo et al., IEEE ICC 2024｜Garcia et al., LEO-NET 2025

**口播**：「Ma 等人 2023 年實測幾個 Starlink 終端發現：throughput 中位數有 100-200 Mbps，但變動很大。這個結論被 2024 年 Bülo 等人的 170 萬筆群眾外包量測完全驗證 — 跨 29 國數據都長一樣。延遲中位數 25-50ms 也不錯，但每 15 秒 handover 一次會造成週期性尖峰。」

---

## Slide 13 — 環境因素影響（Paper 1 + Shukur 2025）

**主標**：Starlink 怕什麼？
**五大環境因素（icon + 一行字）**：
- 🏔️ **地形** — 樹木、山遮擋
- ☀️ **太陽風暴** — 影響軌道與信號
- 🌧️ **雨衰** — Ka/Ku 頻段雨衰明顯
- ☁️ **雲層** — 厚雲影響鏈路品質
- 🌡️ **溫度** — 用戶終端高溫時自動降速以散熱

**💥 KILLER 數據（Shukur 2025，熱帶 6 個月實測）**：
| 條件 | **Starlink LEO** | **SES-12 GEO** |
|------|------------------|----------------|
| 暴雨延遲 | **20–100 ms** | **600–3,000 ms** |
| 上行可用率 | **99.6 %** | **94 %** |

**底部橘字**：LEO 不只比 GEO 快 30 倍 — 還更抗惡劣天氣。

**Cite**：Ma et al., IEEE INFOCOM 2023｜Shukur et al., IIUM Engineering Journal 2025

**口播**：「Paper 1 提到環境影響大，但 2025 年 Shukur 等人在熱帶國家做了 6 個月實測，數據更震撼 — 同樣暴雨下，Starlink 延遲 20 到 100 毫秒，傳統 GEO 衛星卻飆到 600 到 3000 毫秒，差了 30 倍！上行可用率 99.6% 對 94%。LEO 不只快，還更抗惡劣天氣。」

---

## Slide 14 — 應用場景

**主標**：Where LEO Wins
**六大場景（3x2 格子）**：
- 🏔️ **偏鄉/山區** — 光纖無法到的地方
- 🌊 **海上** — 漁船、商船、郵輪
- ✈️ **航空** — 商業航班 In-Flight Wi-Fi（**Ullah 2025 實測：64 Mbps median**）
- 🆘 **災難備援** — 地震、海嘯時地面壞了還能用
- ⚔️ **戰場通訊** — 烏俄戰爭實證
- 📱 **D2D 衛星直連** — iPhone 14+ SOS、T-Mobile + Starlink 計畫

**底部橘標**：
🌐 **6G NTN 標準化進行中** — 3GPP **Release 17、18、19** 都已納入 NTN（Jamshed 2024）

**Cite**：Ullah et al., ComComAp 2025｜Jamshed et al., arXiv 2024

**口播**：「LEO 不是要取代光纖，而是補光纖到不了的地方。從偏鄉、海上、商業航班 — 2025 年最新研究實測飛機上單用戶有 64 Mbps；到災區、戰場、iPhone SOS。最關鍵的是 3GPP Release 17 到 19 都已經把 Non-Terrestrial Networks 正式納入 6G 標準。」

---

## Slide 15 — 挑戰與前沿研究方向

**主標**：Not All Sunshine — 挑戰 × 前沿方向
**左半：四大挑戰**：
- 🗑️ **Kessler Syndrome** — 太空垃圾連鎖碰撞風險
- 📻 **頻譜協調** — FCC / ITU 跟 GEO 業者衝突
- 🔭 **天文光害** — 衛星反光影響天文觀測
- 💰 **商業永續** — 高發射成本 vs 用戶 ARPU

**右半：2025 年三大前沿研究方向**：
- 🌀 **Holographic Metasurface 波束成形**（Li 2025, 91 引用）
- 🛰️ **Space-O-RAN**：把 Open RAN 搬上太空（Baena 2025）— 跟老師教的 cellular RAN 接續
- 🤖 **RL/LLM 輔助 handover 決策**（多篇 2024-2026）

**Cite**：Li et al., IEEE TWC 2025｜Baena et al., IEEE Comm Mag 2025

**口播**：「LEO 還有很多沒解決的問題：太空垃圾、頻譜爭奪、天文光害、商業可持續。但同時 2025 年研究前沿也非常熱：全息超表面做波束、把 Open RAN 概念搬上太空、用強化學習做 handover 決策 — 這正是 6G 時代最 hot 的研究方向。」

---

## Slide 16 — 總結 + 跟課程連結

**主標**：今天學到什麼？
**三句話**：
1. **LEO 把地面 cellular 的概念搬上太空** — 但基地台會跑
2. **Massive MIMO + sCSI** 解決 LEO 的 Doppler 與通道資訊問題
3. **真實世界量測**證實 LEO 可用，但對環境敏感

**金句**（最下方大字）：
> 下次你的 iPhone 顯示衛星訊號 — 你已經在用今天學到的技術。

**口播**：「總結三點：LEO 把基地台搬到天上但帶來新挑戰；Massive MIMO 配 sCSI 是核心物理層技術；Starlink 真實效能不錯但怕環境。謝謝大家。」

---

## Slide 17 — References

**主標**：References

**📌 指定主要文獻（3 篇）**
1. Ma, S. et al. *Network Characteristics of LEO Satellite Constellations: A Starlink-Based Measurement from End Users*. **IEEE INFOCOM 2023**.
2. You, L. et al. *Massive MIMO Transmission for LEO Satellite Communications*. **IEEE JSAC**, vol. 38, no. 8, 2020.
3. Su, Y. et al. *Broadband LEO Satellite Communications: Architectures and Key Technologies*. **IEEE Wireless Comm.**, vol. 26, no. 2, 2019.

**🆕 補充：2024-2026 前沿研究**
4. Brashears, T. *Achieving 99% link uptime on 100G space laser ISLs*. **SPIE Free-Space Laser Comm. XXXVI 2024**. （SpaceX 官方）
5. Garcia, J. et al. *A Detailed Characterization of Starlink One-way Delay*. **LEO-NET Workshop 2025**.
6. Bülo, M. et al. *Crowdsourced Starlink Performance Measurements*. **IEEE ICC 2024**.
7. Shukur, H. et al. *Latency Performance Evaluation of LEO Starlink and SES-12 GEO HTS Under Tropical Rainfall*. **IIUM Eng. J. 2025**.
8. Ullah, M. A. et al. *A First Look at Starlink In-Flight Performance*. **ComComAp 2025**.
9. Dong, Q. et al. *Statistical CSI-Based Beamspace Transmission for Massive MIMO LEO*. **Entropy 2025**.
10. Li, Q. et al. *Holographic Metasurface-Based Beamforming for Multi-Altitude LEO Satellite Networks*. **IEEE TWC 2025**.
11. Baena, E. et al. *Space-O-RAN: Enabling Intelligent, Open NTNs in 6G*. **IEEE Comm. Mag. 2025**.
12. Jamshed, M. A. et al. *A Tutorial on Non-Terrestrial Networks: Towards Global 6G Connectivity*. **arXiv / IEEE 2024**.

**🌐 數據來源**
13. Starlink 官方統計 (May 2026) | ITU Facts & Figures 2023 | 3GPP Release 17–19 NTN 標準

---

## ⏱ 時間檢查

15 分鐘 = 900 秒。17 張平均 53 秒/張。
- Hook + Cover（slides 1-2）：60-70 秒
- 背景（3-5）：180 秒
- 架構（6-8）：180 秒
- 技術深度 MIMO（9-11）：240 秒
- 量測（12-13）：150 秒
- 應用+挑戰（14-15）：120 秒
- 收尾（16-17）：30-50 秒

**緩衝**：約 30-60 秒，剛剛好不超時。

---

## 📌 待你確認

請逐頁看內文，有以下任何想法請告訴我：
1. **內容方向** — 哪些 slide 想加深/減淡？
2. **數字準確度** — 有沒有要更新/調整的數據？
3. **個人風格** — 哪些「金句」想換掉或自己重寫？
4. **slide 數** — 是否要砍掉某些 slide 讓報告更鬆？
5. **新增 slide** — 有沒有想補的內容？

確認後我就動工做 .pptx 檔。
