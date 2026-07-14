# 🧧 如意 · 后台管理系统 (RuyiGinReactAdmin)

<p align="center">
  <img src="https://img.shields.io/badge/React-18-4DABF7?logo=react" alt="React 18" />
  <img src="https://img.shields.io/badge/Gin-Go-22B8CF?logo=go" alt="Gin" />
  <img src="https://img.shields.io/badge/Theme-如意国风科技蓝-D4A853" alt="Theme" />
  <img src="https://img.shields.io/badge/Status-前端MVP完成-51CF66" alt="Status" />
</p>

<p align="center">
  <b>吉祥如意 · 万事如意</b>
  <br/>
  基于 Go (Gin) + React 的现代化后台管理系统
  <br/>
  融合中国风美学与前沿 Web 视觉技术
</p>

---

## 🎨 设计理念：如意国风科技蓝

将中国传统美学（金色点缀、云纹意境）与 2025 年最前沿的 Web UI 技术深度融合：

| 技术 | 应用 |
|------|------|
| **Glassmorphism 玻璃拟态** | Header / Sidebar / 卡片 / 面板全链路毛玻璃 |
| **3D Mouse Tilt** | 统计卡片实时跟踪鼠标，perspective 动态倾斜 |
| **@property 动态光晕** | conic-gradient 边框无限旋转发光动画 |
| **Dynamic Gradients** | 3 个浮动光斑 + 40px 科技网格底纹 |
| **Micro-textures** | SVG 噪点 + 扫描线纹理叠加 |

### 🎯 配色体系

| 色值 | 名称 | 用途 |
|------|------|------|
| `#060B18` | 深空黑蓝 | 全局背景 |
| `#4DABF7` | 科技蓝 | 主强调色、发光 |
| `#22B8CF` | 科技青 | 辅强调色、渐变 |
| `#D4A853` | 如意金 | 国风点缀 |
| `#7950F2` | 星云紫 | 对比色 |

---

## 🖥️ 布局规范

```
┌──────────────────────────────────────────────┐
│  Header  (60px · 固定顶部 · 玻璃拟态)         │
├────────┬─────────────────────────────────────┤
│Sidebar │  Content                            │
│ 220px  │  自适应宽高                           │
│固定左侧 │  overflow-y: auto                   │
│玻璃拟态 │                                     │
│        │                                     │
├────────┴─────────────────────────────────────┤
│       100vw × 100vh  撑满全屏                  │
└──────────────────────────────────────────────┘
```

> ⚠️ **铁律**：此布局为本项目强制规范，任何偏离必须先确认。

---

## 📂 项目结构

```
RuyiGinReactAdmin/
├── backend/                # Go (Gin) 后端（待开发）
├── frontend/
│   └── index.html          # React 前端（单文件，开箱即用）
├── README.md
└── .gitignore
```

---

## 🚀 快速开始

### 前端（当前可运行）

```bash
# 无需安装任何依赖！
# 直接用浏览器打开即可
start E:\web\RuyiGinReactAdmin\frontend\index.html

# 或者用任意 HTTP 服务
# python -m http.server 3000 -d frontend
```

> 前端采用 React 18 CDN + Babel Standalone，零构建、零依赖、零安装。

### 后端（计划中）

```bash
cd backend
go mod init ruyi-gin-react-admin
go run main.go
```

---

## ✨ 已实现功能

### Dashboard 首页

| 模块 | 内容 |
|------|------|
| 📊 统计卡片 ×4 | 用户总数 / 订单总量 / 本月营收 / 今日访问 |
| 📈 数据图表 | 3D 立体渐变柱状图（周访问趋势） |
| 📋 订单表格 | 最近 5 笔订单（状态标签 + hover 高亮） |
| ⚡ 快速操作 | 新建订单 / 添加用户 / 数据报表 / 系统设置 |
| 📌 系统公告 | 发光圆点 + 公告列表 |

### 导航菜单

- **核心功能**：工作台 / 数据分析 / 订单管理
- **系统管理**：用户管理 / 角色权限 / 系统设置
- **其他**：操作日志 / 消息中心

### 交互特性

- 🖱️ 统计卡片 3D 鼠标跟踪倾斜
- 🌟 @property 动态光晕旋转边框
- 🪟 全局玻璃拟态毛玻璃质感
- 🌊 动态渐变光斑背景动画
- ✨ 菜单激活态蓝色发光指示条
- 📱 响应式适配（≤768px 自动隐藏侧栏）

---

## 🛠️ 技术栈

| 层 | 技术 | 状态 |
|----|------|------|
| 前端 | React 18 (CDN) + Babel Standalone | ✅ MVP 完成 |
| 样式 | Pure CSS (CSS Variables + @property + 3D Transforms) | ✅ |
| 数据 | Mock 模式（无后端依赖） | ✅ |
| 后端 | Go + Gin Framework | ⏳ 待开发 |
| 数据库 | 待定 | ⏳ |

---

## 🌿 Git 工作流

```bash
# 分支策略
main    ← 稳定版本（待创建）
dev     ← 开发主分支（当前）
feat/*  ← 功能分支
```

### 当前提交历史

```
2d9bb03 专家增强 - @property动态光晕边框 + 3D鼠标倾斜 + 玻璃saturate + 噪点纹理
188643d 主题升级v2 - 玻璃拟态+3D动画+动态渐变+科技感暗色主题
8b3894b 初始化前端 - 如意国风科技蓝主题后台管理首页
```

---

## 🧠 AI 共享记忆

本项目采用**多 AI 共享记忆**机制：

```
E:\RuyiTypora\如意\记忆\
├── 用户档案.md        ← 用户身份与偏好
├── 如意管理系统.md    ← 本项目完整规格
├── 交互规范.md        ← AI 行为准则
└── 共享记忆说明.md    ← 使用规则
```

所有 AI 助手（如意 / Claude / Codex / Gemini）均可读写此目录，确保认知一致。

---

## 📝 License

MIT

---

<p align="center">
  <sub>Made with ❤️ by 如意 · 吉祥如意，万事如意</sub>
</p>
