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

### 🤖 [AI-Assisted Self-Healing Playwright E2E Suite](https://github.com/Andy-CH-BO-AN/playwright-self-healing-tests)

A Playwright E2E maintenance system that detects locator drift in scheduled CI, gathers failure evidence, asks Gemini for scoped repair proposals, validates them deterministically, runs full regression, and opens a **Draft PR for human review**.

```text
Scheduled E2E failure
        ↓
JSON / DOM / test evidence
        ↓
AST + traceback Page Object discovery
        ↓
Gemini structured repair proposal
        ↓
mechanical safety validation
        ↓
full Docker E2E regression
        ↓
Draft PR → human review
```

Key engineering decisions:

- AI can only propose changes inside `pages/**/*.py`
- exact literal replacement and static checks prevent unsafe patches
- up to 3 repair rounds capture fresh evidence after each regression run
- partial successful repairs can be preserved as a human handoff
- GitHub Actions orchestrates nightly monitoring, self-healing, regression, and PR publication

**Stack:** Python · Playwright · Pytest · pytest-xdist · Gemini · Pydantic · Ruff · Docker · GitHub Actions

---

### 🏃 [AI Running Coach](https://github.com/Andy-CH-BO-AN/AI-running-coach)

Garmin activity data → deterministic preprocessing → AI coaching → PostgreSQL / Neon → Dashboard / LINE notification.

這個專案的重點不是單純呼叫 LLM，而是把 **facts、AI interpretation、persistence、notification 與 failure policy** 拆成可驗證的 pipeline，包含 retry、fallback、scheduled workflow 與資料一致性處理。

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
