# Hi, I'm Vinícius Arruda 👋

Software Engineer based in São Paulo 🇧🇷, currently building fintech and crypto products at **[Trace Finance](https://www.trace.finance)** with a globally distributed team.

I care about clean architecture, reusable systems, and shipping things people actually use. I like Anime, gaming, toy photography, baseball and NBA

---

### 🚀 What I'm building

- ⚔️ **[TBHelper](https://tbherohelper.com)** — wiki + real-time DPS meter for the game *Task Bar Hero*.
- 🛒 **Open-source e-commerce monorepo** — a reusable foundation for new sellers to launch and scale their shops. Issues and PRs welcome.
- 💼 Day-to-day: fintech & crypto platforms at Trace Finance.
- 📚 Always exploring: edge databases (ElectricSQL), local-first apps, and DX tooling.

---

### 🤖 Working with AI

I'm deep into AI-assisted development — **Claude Code** is part of my daily workflow.

- Building **custom agents, slash commands, and hooks** to automate planning, reviewing, and scaffolding.
- Designing **multi-agent code review** (specialist reviewers for security, conventions, logic, tests) to raise the floor on PR quality.
- Sharing what works (and what doesn't) — prompt design, agent orchestration, and where AI still falls short in real codebases.

If you're building tooling around Claude Code, the Anthropic SDK, or agent workflows, I'd love to compare notes.

#### 🧩 Lins Flow — visual orchestration for AI agents

I'm building an AI project called **Lins Flow** — a desktop app where you compose **multi-step AI workflows on a node-based canvas**, instead of writing prompts ad-hoc.

You drop blocks on a board — **triggers**, **pipelines**, **artifacts**, **repositories**, **agent pools**, **context** — connect them with edges, and each pipeline runs Claude Code locally with the skills, agents, and context you wired in. Outputs flow downstream as typed artifacts (subtasks, code, PRs, reviews), so a real feature can be expressed as `Plan → Execute → Review → PR`, parallelized across subtasks, and re-run from any failed step.

Under the hood:
- ⚛️ **Electron + React 19** renderer with **XY Flow**
- ⚡ **Fastify + PostgreSQL + ElectricSQL** backend with WAL-streamed local-first sync
- 🔌 **TanStack DB + Socket.IO** for optimistic writes and ACK-required mutations
- 🧠 **Local Claude CLI execution** via `node-pty`, with an MCP server bridging tool calls back into the app

It's a real engineering exercise in **local-first architecture, multi-user realtime sync, and DAG-based execution** — the kind of system where a single SSOT decision in the wrong place ripples for weeks.

#### ⚔️ TBHelper — wiki + DPS meter for Task Bar Hero

**[tbherohelper.com](https://tbherohelper.com)** is a full product I built for the game *Task Bar Hero*: a datamined wiki (items, builds, monsters, leaderboards) plus a desktop **DPS meter overlay** that reads the game's memory in real time.

- 🌐 **Wiki:** TanStack Start (React 19) + Vite SSR, Tailwind v4, Supabase (auth + Postgres with RLS), crawlable in **16 languages** with hreflang
- 🛰️ **API:** Hono on Node.js (Railway) — leaderboards, run ingest, Discord integration
- 🖥️ **Meter:** Electron overlay + Python memory-reader sidecar (`ReadProcessMemory` + IL2CPP class resolution) tracking DPS, gold, deaths/revives and chest drops per run — [public releases](https://github.com/mad-labs-org/tbh-meter-releases)
- 🚀 **Release pipeline:** tag-driven conventional-commit versioning with a 3-stage RC flow (stage → draft release → promote) and side-by-side RC installs
- 🧪 Reverse-engineering work: IL2CPP metadata resolution (~9x faster cold start via RVA + TypeInfoTable), `.es3` save decryption, CSV TextAsset datamining

### 🧰 Frontend toolkit

What I reach for when starting or scaling a frontend project today:

- **Languages:** TypeScript, JavaScript, Kotlin
- **Frameworks:** Next.js, React, React Native, TanStack Start, Electron
- **State & data:** Zustand, TanStack
- **Forms & validation:** React Hook Form, Zod, Yup
- **Styling:** Tailwind CSS, styled-components, PandaCss, Stitches, Design Systems
- **i18n:** next-i18next
- **Auth:** NextAuth.js, JWT, OAuth
- **Testing:** Jest, Vitest, React Testing Library, Playwright
- **Quality & DX:** ESLint, Prettier, Biome, Husky
- **Monorepo & build:** pnpm workspaces, Turborepo, Vite, esbuild
- **Backend (when needed):** Node.js, NestJS, Express, Fastify, GraphQL, Ktor
- **Databases:** PostgreSQL, SQLite, ElectricSQL, Drizzle ORM, Prisma
- **CI/CD:** GitHub Actions, Vercel, Railway, Docker
- **Observability:** Sentry, Datadog
- **AI tooling:** Claude Code, MCP servers, agent orchestration

---

### 📊 GitHub stats

<p>
  <img height="160" src="https://github-readme-stats-sigma-five.vercel.app/api?username=viniarruda&show_icons=true&hide_border=true&theme=tokyonight" />
  <img height="160" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=viniarruda&layout=compact&hide_border=true&theme=tokyonight" />
</p>

---

### 📄 Resume

- <img src="https://flagcdn.com/20x15/us.png" width="20" alt="🇺🇸" /> [English CV](https://github.com/viniarruda/resume/blob/master/README.en.md)
- <img src="https://flagcdn.com/20x15/br.png" width="20" alt="🇧🇷" /> [Portuguese CV (Português)](https://github.com/viniarruda/resume/blob/master/README.md)

---

### 📫 Find me

- **LinkedIn:** [viniz-arruda](https://www.linkedin.com/in/viniz-arruda)
- **X / Twitter:** [@viniz_arruda](https://twitter.com/viniz_arruda)
- **Email:** [viniarruda.souza@gmail.com](mailto:viniarruda.souza@gmail.com)
- **Stack Overflow:** [profile](https://stackoverflow.com/a/58885314/11896237)
