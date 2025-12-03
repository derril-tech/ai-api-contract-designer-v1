# 🔮 API Contract Designer
**Powered by AutoGen + OpenAI**


🌐 **[View Live Application](https://ai-api-contract-designer.vercel.app/)**

> **Transform product ideas into production-ready API contracts instantly. Describe your app, and watch 5 AI agents collaborate to design endpoints, schemas, and OpenAPI specs—in seconds.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-15-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB.svg)](https://react.dev/)
[![AutoGen](https://img.shields.io/badge/AutoGen-Multi--Agent-purple.svg)](https://microsoft.github.io/autogen/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ What It Does

API Contract Designer is an intelligent API architecture platform that uses a **multi-agent AutoGen workflow** to:

1. **Analyze Your Product** — Extract features, entities, and operations from plain-English descriptions
2. **Design RESTful APIs** — Generate endpoints following industry best practices
3. **Write OpenAPI Specs** — Create complete OpenAPI 3.1.0 YAML specifications
4. **Review & Refine** — Apply security patterns, error conventions, and polish

All in a single, beautiful interface with real-time agent progress visualization.

---

## 🎯 Core Features

### 🤖 **5-Agent AI Pipeline**
- **ProductAnalystAgent** — Extracts use cases and business domains
- **APIDesignerAgent** — Proposes endpoints and HTTP methods
- **OpenAPIWriterAgent** — Generates OpenAPI 3.1.0 contracts
- **ReviewerAgent** — Checks consistency and naming conventions
- **RefinerAgent** — Applies feedback and final polish

### 📊 **Rich Output**
- **Endpoint Gallery** — Visual cards for each API route with method badges
- **YAML Syntax Highlighting** — Professional code display with line numbers
- **Error Conventions** — Collapsible panel with 4xx/5xx standards
- **Security Notes** — Authentication, rate limiting recommendations

### 🎨 **Modern UI/UX**
- **Single-Page Architecture** — Smooth state-driven transitions
- **Dark/Light Mode** — Beautiful theme with system preference support
- **Mobile-First** — Responsive design with tab navigation on mobile
- **Toast Notifications** — Instant feedback for all actions

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🎯 **Agent Pipeline** | Live visualization of 5 agents working |
| 📝 **Contract Templates** | 6 pre-built API patterns to jumpstart |
| 📋 **Copy as cURL** | One-click endpoint copying |
| ⬇️ **Export YAML/JSON** | Download contracts for your project |
| 🔗 **Share via URL** | Generate shareable links |
| ⌨️ **Keyboard Shortcuts** | 6 power-user shortcuts |
| 💾 **Save to Dashboard** | Persist contracts to Supabase |
| 📂 **Project History** | View and manage saved contracts |
| 🎨 **Theme Toggle** | Light, dark, and system modes |
| 📱 **Mobile Tabs** | Touch-friendly panel navigation |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 15** | React 19 with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling |
| **shadcn/ui** | Beautiful component library |
| **Sonner** | Toast notifications |
| **Prism React Renderer** | Syntax highlighting |
| **Lucide Icons** | Modern icon set |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance Python API |
| **AutoGen** | Multi-agent AI orchestration |
| **OpenAI GPT-4** | Intelligent API design |
| **Pydantic v2** | Data validation |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL persistence |
| **Upstash Redis** | Job queue & caching |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting |
| **Railway** | Backend API |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INPUT                               │
│              "A todo app with tasks and categories"         │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                  AUTOGEN PIPELINE                           │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │   Product    │  │     API      │  │   OpenAPI    │      │
│  │   Analyst    │──│   Designer   │──│   Writer     │      │
│  │  (GPT-4)     │  │   (GPT-4)    │  │   (GPT-4)    │      │
│  └──────────────┘  └──────────────┘  └──────┬───────┘      │
│                                             │               │
│         ┌───────────────┐          ┌────────▼────────┐     │
│         │   Reviewer    │◄─────────│    Refiner      │     │
│         │   (GPT-4)     │          │    (GPT-4)      │     │
│         └───────────────┘          └────────┬────────┘     │
└─────────────────────────────────────────────┼───────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────┐
│                       OUTPUT                                │
│  • 5-15 RESTful Endpoints                                   │
│  • 3-5 Data Models with fields                              │
│  • Error Conventions (400, 401, 404, 500)                   │
│  • Security Recommendations                                 │
│  • Complete OpenAPI 3.1.0 YAML                              │
└─────────────────────────────────────────────────────────────┘
```

---

## 📖 User Guide

### Getting Started

1. **Describe Your Product** — Enter a plain-English description of your app idea
2. **Or Choose a Template** — Pick from 6 pre-built API patterns
3. **Run the Agents** — Watch 5 AI agents collaborate in real-time
4. **Explore Results** — Browse endpoints, copy cURL commands, view YAML
5. **Save or Export** — Persist to dashboard or download files

### Understanding Your Results

| Section | What It Shows |
|---------|---------------|
| **Endpoints** | RESTful routes with method badges (GET, POST, PUT, DELETE) |
| **OpenAPI YAML** | Complete specification ready for code generation |
| **Error Conventions** | Standard HTTP error responses (400, 401, 403, 404, 500) |
| **Security Notes** | Authentication and rate limiting recommendations |

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Enter` | Run agents |
| `Ctrl + Shift + C` | Copy YAML |
| `Ctrl + Shift + E` | Export YAML file |
| `Ctrl + Shift + S` | Generate share link |
| `Escape` | Reset workspace |
| `?` | Toggle shortcuts help |

### Contract Templates

| Template | Description |
|----------|-------------|
| 🛒 **E-commerce** | Products, cart, checkout, orders |
| 🔐 **Authentication** | Users, sessions, OAuth, MFA |
| ✅ **Task Management** | Projects, tasks, teams, comments |
| 📱 **Social Media** | Posts, followers, feeds, notifications |
| 🤖 **AI/ML** | Models, predictions, training jobs |
| 🏠 **IoT** | Devices, sensors, telemetry, commands |

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface
- 🌙 **Dark Mode** — Easy on the eyes
- 🖥️ **System** — Follows OS preference

### Mobile Experience
- 📱 **Tab Navigation** — Switch between Input, Endpoints, and YAML panels
- 👆 **Touch-Friendly** — Copy buttons always visible, 44px+ touch targets
- 🔄 **Auto-Switch** — Automatically shows results when generation completes

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Contract Generation | ~15-30 seconds |
| Frontend Bundle | ~170 kB |
| Lighthouse Score | 90+ |
| Mobile Ready | ✅ Yes |

---

## 🛡️ Security

- ✅ No product data stored permanently (ephemeral processing)
- ✅ API rate limiting
- ✅ CORS protection for API endpoints
- ✅ Environment variables for all secrets
- ✅ Input sanitization and validation
- ✅ Supabase Row-Level Security ready

---

## 👨‍💻 Creator

**Derril Filemon**

[![GitHub](https://img.shields.io/badge/GitHub-derril--tech-black.svg?logo=github)](https://github.com/derril-tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue.svg?logo=linkedin)](https://www.linkedin.com/in/derril-filemon-a31715319)

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — AutoGen multi-agent workflows, OpenAI GPT-4
- ⚛️ **Modern React** — Next.js 15, React 19, Server Components
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic
- 🎨 **UI/UX Design** — Responsive design, animations, accessibility
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔧 **DevOps** — CI/CD, environment management, monorepo structure

---

## 🙏 Acknowledgments

- **[AutoGen](https://microsoft.github.io/autogen/)** — Multi-agent orchestration
- **[OpenAI](https://openai.com/)** — GPT-4 API
- **[Supabase](https://supabase.com/)** — Database & persistence
- **[Upstash](https://upstash.com/)** — Redis caching
- **[Railway](https://railway.app/)** — Backend deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful components
- **[Sonner](https://sonner.emilkowal.ski/)** — Toast notifications

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

[Live Demo](https://ai-api-contract-designer.vercel.app/)

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
