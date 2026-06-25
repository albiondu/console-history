# Retrocore Design

## 專案概述
FPGA 復古遊戲主機「RetroCore FPGA」的硬體設計與規畫專案。包含主機規格書、I/O 接口規劃、與市場上現有 FPGA 方案（Analogue 3D、SuperStation One、MiSTer）的對比分析。

## 相關連結
- GitHub Pages: https://albiondu.github.io/console-history/
- NotebookLM: https://notebooklm.google.com/notebook/2faefc57-8b53-4794-8620-7fda69241f2a

## 設計原則
1. 純 FPGA 為核心運算元件，非 PC 零組件堆疊
2. 支援原版卡匣/光碟讀取但保持務實
3. 精簡 OS 專注於遊戲載入
4. 模組化擴充，成本目標 $249

## 關鍵規格
- FPGA: Intel Cyclone 10 GX (220K LE)
- 記憶體: 256MB DDR3 + 128MB 專用 SDRAM
- 輸出: HDMI 2.1 (4K/60) + VGA + TOSLINK
- 控制器: 2× SNAC 原廠控制器埠
- 擴充: 40-pin GPIO 模組連接器
- 功耗: < 40W 被動散熱

## 開發者
Albion Du
