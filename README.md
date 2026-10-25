# Hi, I'm Andy 👋

**Senior Software Development Engineer in Test (SDET) · Quality Engineering · AI-assisted Testing**

我專注在 **Test Automation、Test Infrastructure、CI Reliability 與 AI-assisted Quality Engineering**。

比起單純增加測試案例，我更在意如何把測試系統做得 **可維護、可觀測、可重現、能安全失敗，也能降低人工維護成本**。近期的重點是把 LLM 放進測試維護流程，但保留 deterministic validation 與 human review，讓 AI 成為工程系統中的 proposal engine，而不是黑箱決策者。

## 🔍 Current Focus

- **E2E Automation** — Playwright, Selenium, Appium, Page Object Model
- **Test Framework Engineering** — Pytest, fixtures, parametrization, parallel execution, test isolation
- **CI/CD & Reliability** — GitHub Actions, Jenkins, Docker, failure evidence, flaky-test reduction
- **API & Data Validation** — Requests, REST API testing, MySQL / PostgreSQL
- **AI-assisted Testing** — structured LLM output, evidence-driven diagnosis, retry / fallback, deterministic safety gates
- **Quality Engineering** — maintainability, observability, responsibility boundaries, safe automation

## 🚀 Featured Projects

### 🤖 [AI 輔助自癒 Playwright E2E 測試系統](https://github.com/Andy-CH-BO-AN/playwright-self-healing-tests)

這是一套用來降低 UI 自動化維護成本的 Playwright E2E 自癒系統。當排程 CI 因 locator drift 失敗時，系統會自動收集失敗證據、找出相關 Page Object，交由 Gemini 產生範圍受限的修復建議，再經過 deterministic safety validation 與完整 regression 驗證，最後開出 **Draft PR 交由人工 review**。

```text
Scheduled E2E failure
        ↓
JSON / DOM / test evidence
        ↓
AST + traceback 找出相關 Page Object
        ↓
Gemini structured repair proposal
        ↓
mechanical safety validation
        ↓
完整 Docker E2E regression
        ↓
Draft PR → human review
```

主要工程設計：

- AI 只能提議修改 `pages/**/*.py`，限制修復範圍
- 使用 exact literal replacement 與 static checks 阻擋不安全 patch
- 最多進行 3 輪修復，每輪 regression 失敗後重新蒐集最新 evidence
- 前段已成功的修復可以保留，透過 Partial Repair 交由工程師接手
- GitHub Actions 串起 nightly monitoring、self-healing、regression 與 Draft PR publication

**Stack:** Python · Playwright · Pytest · pytest-xdist · Gemini · Pydantic · Ruff · Docker · GitHub Actions

---

### 🏃 [AI Running Coach](https://github.com/Andy-CH-BO-AN/AI-running-coach)

Garmin activity data → deterministic preprocessing → AI coaching → PostgreSQL / Neon → Dashboard / LINE notification.

這個專案的重點不是單純呼叫 LLM，而是把 **facts、AI interpretation、persistence、notification 與 failure policy** 拆成可驗證的 pipeline，包含 retry、fallback、scheduled workflow 與資料一致性處理。

---

### ⚔️ [SagaBurst 3D Game](https://github.com/Andy-CH-BO-AN/SagaBurst-3D-Game)

**SagaBurst** 是我開發的 Viking vs Roman **3D 動作與戰術指揮遊戲**，支援瀏覽器及 Windows / macOS 桌面版。玩家可以自訂最高 **200 vs 200 AI 大型戰場**，配置步兵、弓兵、標槍兵、騎兵與騎射兵，親自上陣、指揮列陣與衝鋒，或切換觀戰模式欣賞 AI 軍隊交戰。

除了 **Custom Battle**，還有 **Training Ground**、Roman / Viking 各九關的 **Defense Campaign**，以及可持續存檔的 **Career Mode**：從 Recruit 一路晉升 Commander，累積軍功、升級技能與裝備、招募私人部隊，指揮守城、攻城與各種軍事任務。坐騎包含馬、黑貓、柯基，還能騎乘巨鷹 **xongkoro** 在空中作戰。

**Play:** [Browser](https://andy-ch-bo-an.github.io/SagaBurst-3D-Game/) · [Windows / macOS Downloads](https://github.com/Andy-CH-BO-AN/SagaBurst-3D-Game/releases/latest)

**Stack:** TypeScript · Three.js · Vite · Vitest · Playwright · WebGL

---

### 🧪 [Stylish Automation Test Framework](https://github.com/Andy-CH-BO-AN/Automation-Test-Project-Stylish)

完整的 Pytest automation project，整合：

**Web UI → REST API → MySQL validation → parallel execution → Allure reporting**

包含 Page Object、API Object、DB helper、fixture lifecycle、xdist credential isolation 與 test-data driven flow。

## 🛠️ Tech Stack

`Python` · `Pytest` · `Playwright` · `Selenium` · `Appium` · `Requests` · `Docker` · `GitHub Actions` · `Jenkins` · `Ruff` · `Allure` · `PostgreSQL` · `MySQL` · `Gemini / LLM`

## 🧭 Engineering Direction

```text
manual / repetitive work
        ↓
automation
        ↓
reliable workflow
        ↓
observable + testable system
        ↓
AI where it actually adds value
```

我喜歡做的事情通常圍繞同一個方向：**把原本需要工程師一直盯、一直重複處理的品質工作，逐步變成可靠、可驗證，而且有清楚安全邊界的工程系統。**
