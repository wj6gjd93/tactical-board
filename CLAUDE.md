# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 專案概述

籃球戰術板 Web 應用，純 HTML + CSS + JavaScript 實作，無任何框架或外部依賴。目標是可在移動端直接使用的單一 HTML 檔案應用。

## 執行方式

直接用瀏覽器開啟 `index.html`，無需建置流程或伺服器。

## 功能規格

- **球場**：半場 / 全場可切換
- **球員**：可拖曳新增、移除，可拖曳定位，攻守雙方使用不同顏色，自動賦予球員號碼 1 - 5
- **移動端**：支援 touch events，響應式版面

## 技術架構

- 所有繪圖使用 **Canvas 2D API**
- 球員以可拖曳的 Canvas 物件實作（非 DOM 元素）
- Touch events 映射至對應的 Mouse events 以統一觸控與滑鼠操作
- 單一 `index.html` 包含全部 HTML、CSS、JS
