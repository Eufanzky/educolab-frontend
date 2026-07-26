<div align="center">

# 🎓 EduColab — Frontend

**A collaborative learning platform built by a team of four for the Platzi × New Relic Hackathon (May 2023).**

[![Next.js](https://img.shields.io/badge/Next.js-13-black?logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)](https://react.dev/)
[![CSS Modules](https://img.shields.io/badge/CSS_Modules-000000?logo=css3&logoColor=white)](https://github.com/css-modules/css-modules)
[![New Relic](https://img.shields.io/badge/New_Relic-1CE783?logo=newrelic&logoColor=black)](https://newrelic.com/)

</div>

> **This is my fork of [`EduColab/frontend`](https://github.com/EduColab/frontend).**
> It's kept public as a record of my contribution to the project. Full credit for the platform goes to the whole team — see [Team](#-team) below.

---

## 👤 My Role

I was the **second-largest contributor** on this codebase, with **64 commits across 18 merged pull requests**, working on a shared `task → stage → main` branching workflow.

**What I built:**

| Area | Contribution |
|:-----|:-------------|
| 🏘️ **Community section** | Built the community page end to end — layout, sections, styles, and API integration |
| 📝 **Registration & login** | Register page, plus link wiring and flow for the auth pages |
| 📤 **Course upload form** | `FormUploadCourse` — form handling and submission logic |
| 🔌 **API integration** | Wired several pages to the backend via `axios` |
| 🚪 **`NoLogin` component** | Logged-out state and its integration into the community page |
| ℹ️ **About page** | Built the page and its styling |

Working on a four-person team meant regularly rebasing on `upstream/stage` and resolving merge conflicts — a good chunk of the commit log is exactly that.

## 🧱 Tech Stack

- **Next.js 13** with the App Router (`src/app/`)
- **React 18**
- **CSS Modules** — scoped styles co-located per component
- **axios** for API consumption
- **New Relic** APM instrumentation (the hackathon's sponsor challenge)
- **GitHub Actions** CI (`.github/workflows/node.js.yml`)
- Separate `stage` and `production` environment configs

## 📁 Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── community/          # Community hub
│   ├── curso/[id]/         # Course detail (dynamic route)
│   ├── carrera/[id]/       # Career track detail
│   ├── university/[id]/    # University pages
│   ├── login/  register/   # Auth pages
│   └── about/
└── components/             # Component + co-located CSS Module
    ├── CommunitySection/
    ├── CommunityCourses/
    ├── FormUploadCourse/
    ├── LoginForm/
    └── ...
```

## 🚀 Running Locally

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## 👥 Team

Built by [@Duvier-Reinosa](https://github.com/Duvier-Reinosa), [@Eufanzky](https://github.com/Eufanzky), [@castlewhites](https://github.com/castlewhites) and [@UzyOrg](https://github.com/UzyOrg).

Upstream repository: **[EduColab/frontend](https://github.com/EduColab/frontend)**
