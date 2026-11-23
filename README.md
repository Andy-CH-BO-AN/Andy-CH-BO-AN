# Hi, I'm Andy 👋

**Senior Software Development Engineer in Test (SDET) · Quality Engineering**

我有 6 年以上軟體測試與自動化經驗。

## 精選測試專案

### [Playwright E2E 測試自癒](https://github.com/Andy-CH-BO-AN/playwright-self-healing-tests)

排程 CI 偵測到 UI locator drift 後，系統收集失敗證據、定位相關 Page Object，再由 Gemini 提議修正。程式限制修改範圍並驗證 patch，接著在 Docker 跑完整 E2E 回歸。修正以 Draft PR 交由工程師審查。 [看實際修復案例 #36](https://github.com/Andy-CH-BO-AN/playwright-self-healing-tests/pull/36)

### [Appium Android E2E 與自癒基礎](https://github.com/Andy-CH-BO-AN/appium-agentic-self-healing-tests)

以 Appium、UiAutomator2 與 pytest 在 Android Emulator 上驗證商品詳情、購物車與結帳流程。測試失敗時會保留截圖、UI hierarchy 與結構化錯誤資訊，區分 locator timeout 與 assertion failure。下一步是用這些證據做 AI 輔助診斷。

## 其他作品

### [SagaBurst 3D Game](https://github.com/Andy-CH-BO-AN/SagaBurst-3D-Game)

來指揮維京或羅馬軍隊，自訂最高 **300 vs 300** 的戰場，親自上陣或在觀戰模式看兩軍交戰。也可以從新兵開始玩生涯模式，升到指揮官、招募自己的部隊，或騎上巨鷹參戰。

[瀏覽器直接玩](https://andy-ch-bo-an.github.io/SagaBurst-3D-Game/) · [下載 Windows／macOS 版](https://github.com/Andy-CH-BO-AN/SagaBurst-3D-Game/releases/latest)

### [AI Running Coach](https://github.com/Andy-CH-BO-AN/AI-running-coach)

把 Garmin 活動資料整理成可追溯的訓練指標，由 Gemini 解讀近期訓練並產生建議。支援 GitHub Actions 排程、PostgreSQL／Neon 資料儲存、Dashboard 與 LINE 通知。
