# Hi, I'm Andy 👋

**Senior Software Development Engineer in Test (SDET)**

## 測試自動化

### [Playwright E2E 測試自癒](https://github.com/Andy-CH-BO-AN/playwright-self-healing-tests)

排程測試因 UI locator 變動而失敗時，Gemini 根據失敗證據提出修正。系統只允許修改 Page Object，並在 Docker 跑完整 E2E 回歸，再開 Draft PR 供人工審查。

[看實際修復 PR #36](https://github.com/Andy-CH-BO-AN/playwright-self-healing-tests/pull/36)

### [Appium Android E2E 測試](https://github.com/Andy-CH-BO-AN/appium-agentic-self-healing-tests)

用 Appium 和 pytest 在 Android Emulator 上測試商品詳情、購物車與結帳。測試失敗時會自動收集截圖、UI hierarchy 和結構化錯誤資訊。

[看 Android E2E 測試案例](https://github.com/Andy-CH-BO-AN/appium-agentic-self-healing-tests/tree/main/tests/e2e)

## 其他作品

### [SagaBurst 3D Game](https://github.com/Andy-CH-BO-AN/SagaBurst-3D-Game)

來指揮維京或羅馬軍隊，自訂最高 **300 vs 300** 的戰場，親自上陣或在觀戰模式看兩軍交戰。也可以從新兵開始玩生涯模式，升到指揮官、招募自己的部隊，或騎上巨鷹參戰。

[瀏覽器直接玩](https://andy-ch-bo-an.github.io/SagaBurst-3D-Game/) · [下載 Windows／macOS 版](https://github.com/Andy-CH-BO-AN/SagaBurst-3D-Game/releases/latest)

### [AI Running Coach](https://github.com/Andy-CH-BO-AN/AI-running-coach)

用 Python 計算 Garmin 活動的訓練量與強度，再由 Gemini 解讀並提供建議。可以在 Dashboard 查看訓練回顧，也能透過 LINE 接收通知。
