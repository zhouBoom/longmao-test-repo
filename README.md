# 🚀 Prompt2Repo 准入考核 (Entrance Challenge)

## 📌 考核背景
本项目寻找具备 **"AI Native" (Vibe Coding)** 能力的资深工程师。我们需要你展示如何利用 **Cursor / Trae / Claude Code** 等 AI 工具，快速构建**工程化标准**的应用。

> **核心考核点**：
> 1. **AI 驾驭能力**：不仅是生成代码，而是生成架构、调试 Bug、优化工程。
> 2. **Docker 交付标准**：强制容器化交付，拒绝“在我本地能跑”的代码。
> 3. **全栈审美**：拒绝简陋 UI，需具备商业级交付意识。

---

## 🎯 题目菜单 (任选其一)

请根据你的技术栈，从以下 5 个题目中**任选 1 个**完成。

### 🅰️ 纯前端：动态主题仪表盘 (SaaS Dashboard)
* **目标**：构建一个销售数据看板，支持 Light/Dark 主题切换。
* **技术**：React/Vue + Echarts/Recharts + **Tailwind/AntD (必选)**。
* **交付**：将前端静态资源或服务容器化，实现一键启动。

### 🅱️ 纯后端：短链接生成服务 (URL Shortener)
* **目标**：实现长链接转短链接的 REST API (POST/GET)，含重定向逻辑。
* **技术**：Python/Go/Java/Node + Redis/SQLite。
* **交付**：API 服务与数据库均需 Docker 化。

### 🅾️ 全栈：看板任务管理 (Kanban Board) —— ⭐ 推荐
* **目标**：实现类似 Trello 的任务拖拽 (Todo/Doing/Done) 及数据同步。
* **技术**：Web 前端 + 后端 API + 数据库。
* **交付**：前后端及数据库必须通过 `docker compose` 一键联调。

### 🅳 跨平台/小程序：咖啡点单 (Coffee Order App)
* **目标**：模拟点单流程（商品列表、规格选择、购物车）。
* **技术**：Uni-app / Taro / Flutter / 微信原生。
* **交付**：**客户端代码本地运行** + **后端 API/DB 必须 Docker 化**。

### 🅴 原生移动端：健身计时器 (Fitness Timer)
* **目标**：HIIT 倒计时工具，支持后台运行和声音提示。
* **技术**：Swift / Kotlin / React Native。
* **交付**：**App 代码本地运行** + **后端 API/DB 必须 Docker 化**。

---

## 📦 统一交付标准 (Unified Delivery Standard)

本项目强制要求 **Docker 化交付**。请根据你选择的题目类型，遵守以下目录结构和规范：

### 1. 针对 Web / 全栈 / 纯后端 (Type A, B, C)
你的仓库必须包含完整的前后端容器配置。
* **结构示例**：
  ```text
  ├── frontend/ (含 Dockerfile)
  ├── backend/  (含 Dockerfile)
  └── docker-compose.yml  <-- 必须包含，负责启动所有服务