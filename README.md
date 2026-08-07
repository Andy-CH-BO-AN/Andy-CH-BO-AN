# Hi, I'm Andy 👋

**Software Development Engineer in Test · Python Engineer · AI-assisted Engineering**

我主要做 **Test Automation / SDET**，也喜歡把自動化從「測試腳本」往更完整的工程系統延伸：API、Database、CI/CD、Docker、資料處理，以及 AI-enabled workflows。

我在意的不只是「測試有沒有跑」，而是 **可維護性、可追溯性、failure handling、test isolation 與清楚的 responsibility boundary**。

## 🧪 Test Automation / SDET

- **Web UI** — Selenium, Appium, Page Object Model
- **API** — Requests, REST API testing, session / auth handling
- **Test Framework** — Pytest, fixture design, parametrization, xdist
- **Database Validation** — MySQL / PostgreSQL cross-validation
- **Reporting** — Allure, screenshots, failure evidence
- **CI/CD** — GitHub Actions, Jenkins, Docker
- **Quality Engineering** — test isolation, flaky-test reduction, deterministic assertions, safe logging

## 🤖 AI Engineering

我把 AI 當成工程系統的一部分，而不是單純 chatbot：

- LLM / Gemini integration
- structured AI output 與 schema validation
- **deterministic facts → AI interpretation** 的資料邊界
- evidence-driven AI output，讓結果可以回頭追查原始資料
- AI pipeline 的 retry / fallback / degraded-mode design
- AI-assisted development：architecture planning、refactoring、review 與 test design

目前主要實作在 **AI Running Coach**：Garmin data 先由 Python 產生 deterministic training facts，再交給 Gemini 做 coaching interpretation，最後串接 PostgreSQL / Neon、Dashboard、LINE notification 與 GitHub Actions scheduled pipeline。

## 🛠️ Tech Stack

`Python` · `Pytest` · `Selenium` · `Appium` · `Requests` · `MySQL` · `PostgreSQL` · `Docker` · `GitHub Actions` · `Jenkins` · `Allure` · `Gemini / LLM`

## 🚀 Featured Projects

### 🏃 [AI Running Coach](https://github.com/Andy-CH-BO-AN/AI-running-coach)

Garmin → deterministic preprocessing → AI coaching → PostgreSQL / Neon → Dashboard / LINE。

重點不只是接 LLM API，而是把 **facts、AI interpretation、persistence、notification 與 cloud failure policy** 拆成可驗證的 pipeline。

### 🧪 [Stylish Automation Test Framework](https://github.com/Andy-CH-BO-AN/Automation-Test-Project-Stylish)

完整的 Pytest automation project，整合：

**Web UI → REST API → MySQL validation → parallel execution → Allure reporting**

包含 Page Object、API Object、DB helper、fixture lifecycle、xdist credential isolation 與 test-data driven flow。

### 🌐 [ACY Registration Automation](https://github.com/Andy-CH-BO-AN/test-acy-register)

Selenium + Pytest 的 multi-step registration E2E automation，包含 file upload、local Chrome 與 Selenium Docker Remote WebDriver。

### 🎮 [Online Rock Paper Scissors](https://github.com/Andy-CH-BO-AN/online-paper-scissors-stone)

Python socket + threading 的雙人連線猜拳程式。後續重構為 length-prefixed JSON protocol、明確 game state 與 thread-safe server flow。

### 🧩 [Computer Part Price](https://github.com/Andy-CH-BO-AN/computer-part-price)

早期 Python side project：從原價屋抓取商品資料，經 BeautifulSoup parsing / normalization 後存入 MongoDB。

`fetch → parse → normalize → persist`

## 🔍 What I enjoy building

```text
repetitive manual work
        ↓
automation
        ↓
reliable workflow
        ↓
observable / testable system
        ↓
AI where it actually adds value
```

我喜歡的方向通常都圍繞同一件事：**把原本需要人一直盯、一直重複做的事情，變成可靠而且能被驗證的系統。**
