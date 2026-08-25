<div align="center">

# Hervé "Kamanga" Muludiki

### Software Craftsman · Craft + AI Coach · Full Stack Developer

*Taking back control of your code, in the age of AI.*

[![Website](https://img.shields.io/badge/Website-kamanga.fr-0A0A0A?style=for-the-badge&logo=safari&logoColor=white)](https://kamanga.fr)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-kamangacode-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kamangacode)
[![YouTube](https://img.shields.io/badge/YouTube-@kamangacode-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@kamangacode)
[![X](https://img.shields.io/badge/X-@kamangacode-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/kamangacode)
[![Email](https://img.shields.io/badge/Email-herve@kamanga.fr-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:herve@kamanga.fr)

[🇫🇷 Français](README.md) · **🇬🇧 English**

</div>

---

## About

I help engineering teams and their managers **take back control of their systems**. 25 years in the field as a tech lead, fractional CTO and technical coach inside large organizations (BNP Paribas, Crédit Agricole, Canal+, Agirc-Arrco, Société Générale, JCDecaux, Air France).

Today my work is focused on a single axis:

- **[Craft + AI Coach](https://www.kamanga.fr/)**: transforming engineering culture (Clean Architecture, DDD, TDD, pair programming, software quality) and governing AI inside the development cycle (shared guardrails, security of generated code, controlled cost)

### AI Craft, my current conviction

> *The art of using AI to build well-made applications, on a tightly controlled budget.*

AI speeds up production. It does not replace judgment. The teams that come out of this transition ahead are the ones that understand what they are building. That is exactly where I work.

---

## Current projects

### Conduit Full Stack

A real full-stack TypeScript project, run like a production system: an `api` + `web` +
`shared` monorepo in NestJS, Next.js and Zod, implementing the
[RealWorld](https://realworld-docs.netlify.app/) spec (code name *Conduit*, a Medium clone
with articles, comments, favorites and author following).

[![conduit-fullstack](https://img.shields.io/badge/GitHub-conduit--fullstack-0A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kamangacode/conduit-fullstack)

**What is at stake.** What separates a project that lasts ten years from one that becomes
unmanageable at 18 months is almost never the talent of the team: it is the frame put in
place on day one. The problem is that this frame does not fit in slides. It is read in the
files.

**Why it exists.** To make that frame concrete and verifiable. Since the functional scope is
frozen by the RealWorld spec, the *what* is already decided: only the *how* is left, and
that is exactly what this repository exposes. It is also the executable implementation of
[Le Référentiel Craft](https://www.kamanga.fr/referentiel-craft), my 25 years of practice
condensed into 100 practices across 21 phases.

**My methodology.** Every increment follows the same path and leaves a trace at each step:
frame it (PRD, explicit out of scope), specify it (versioned requirements with their
acceptance criteria), decide (immutable ADRs), implement (code and tests in the same unit,
on a branch cut from `staging`), review and ship (review in Conventional Comments, promotion
from `staging` to `main`). Interrupted work can be picked up without rebuilding the context
from memory.

**What this project demonstrates:**

- **Hexagonal architecture**: ports in the domain, adapters in the infrastructure, a pure domain without a single NestJS or Prisma import.
- **DDD and Clean Architecture**: bounded contexts, an immutable aggregate root, validated value objects, the dependency rule held across 4 layers.
- **One single shared model**: the Zod schema is the only definition, the TypeScript type is inferred from it. Front and back consistency becomes a compile-time dependency instead of a contract to keep in sync.
- **Testing strategy**: the official RealWorld conformance suite vendored at a pinned SHA (128 Playwright tests, never edited), coverage required per layer, and a guard against a green but empty run.
- **Tooled quality**: Biome, cognitive complexity blocking in CI, dependency-cruiser on hexagonal boundaries, knip on dead code.
- **Requirements as code**: versioned requirements, schema-validated frontmatter, requirements-to-tests traceability matrix generated in CI.
- **Security by design**: fail-fast environment validation at boot, anti-IDOR filtered in SQL, server-side authority on authorship, secrets kept out of the repository, documented threat model.
- **Documentation as code**: immutable ADRs with an automated gate, guides, standards, all in versioned Markdown.
- **Delivery**: Conventional Commits, `feature` to `staging` to `main` by promotion, merge commit and never squash.
- **Agentic workflow and SDLC**: the tooled cycle I use daily, under human gates.

> **This repository is meant to be read, not just cloned.** Every guardrail is a real,
> commented file, readable without additional context. Open one at random.
>
> [**→ Explore conduit-fullstack**](https://github.com/kamangacode/conduit-fullstack) · [**→ Discover Le Référentiel Craft**](https://www.kamanga.fr/referentiel-craft)

### CRM Coaching

A SaaS application for professional coaches (Next.js 16, NestJS 11, Prisma, hexagonal architecture, embedded AI). Written 100% in AI Craft.

<p align="center">
  <img src="ressources/crm-cosching-lead.png" alt="CRM Coaching lead view preview" width="800" />
</p>

### Others

- **[kamanga.fr blog](https://kamanga.fr/blog)**: software craftsmanship and AI Craft, made accessible.
- **YouTube channel [@kamangacode](https://youtube.com/@kamangacode)**: tutorials, field feedback, modern engineering practices taken apart.

---

## What I believe, no compromise

- **Software quality** is a business decision, not a technical option.
- **Technical debt** is financial debt. It has a real, measurable cost.
- **Craftsmanship** is a guardrail, not a dogma.
- **AI** raises the urgency of human judgment, it does not remove it.
- A good **transformation** makes teams autonomous, not dependent on the consultant.

---

## Tech Stack

### AI and Agents

![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor-000000?style=for-the-badge&logo=cursor&logoColor=white)

### Frontend and Full Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_16-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn/ui-000000?style=for-the-badge&logo=shadcnui&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=for-the-badge&logo=react&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)

### Backend and Data

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS_11-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Java](https://img.shields.io/badge/Java_25-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma_7-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3068B7?style=for-the-badge&logo=zod&logoColor=white)
![Better Auth](https://img.shields.io/badge/Better_Auth-000000?style=for-the-badge&logo=auth0&logoColor=white)

### Testing and Quality

![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Cucumber](https://img.shields.io/badge/Cucumber-23D96C?style=for-the-badge&logo=cucumber&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white)
![Biome](https://img.shields.io/badge/Biome-60A5FA?style=for-the-badge&logo=biome&logoColor=white)

### DevOps and Infrastructure

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white)

### Architecture and Methodologies

![Hexagonal](https://img.shields.io/badge/Hexagonal_Architecture-1A1A1A?style=for-the-badge)
![DDD](https://img.shields.io/badge/DDD-1A1A1A?style=for-the-badge)
![Clean Architecture](https://img.shields.io/badge/Clean_Architecture-1A1A1A?style=for-the-badge)
![TDD](https://img.shields.io/badge/TDD-1A1A1A?style=for-the-badge)
![BDD](https://img.shields.io/badge/BDD-1A1A1A?style=for-the-badge)
![SOLID](https://img.shields.io/badge/SOLID-1A1A1A?style=for-the-badge)
![Microservices](https://img.shields.io/badge/Microservices-1A1A1A?style=for-the-badge)
![Pair Programming](https://img.shields.io/badge/Pair_Programming-1A1A1A?style=for-the-badge)
![Scrum](https://img.shields.io/badge/Scrum-1A1A1A?style=for-the-badge)
![SAFe](https://img.shields.io/badge/SAFe-1A1A1A?style=for-the-badge)

### Compliance and regulation

![GDPR](https://img.shields.io/badge/GDPR-1E3A8A?style=for-the-badge)

---

## Certifications and education

| Year | Type | Title |
|-----:|------|-------|
| 2023 | Certification | Manager Certification (Ecole 109) |
| 2023 | Education | **Executive MBA** in IT Management and Entrepreneurship (Epitech Executive, Paris) |
| 2023 | Education | **Information Systems Management** (IB Cegos, Paris): IT master plan, digital transformation, governance, financial performance, risk management, agile methods |
| 2021 | Certification | Certified Scrum Master (Scrum Alliance) |
| 2021 | Certification | Practitioner Coach (Coach Académie, Paris) |
| 2008 | Education | **Master's degree** in IT, networks and telecom engineering, banking information systems track (M2IRT, ITIN / CCI Versailles) |
| 2007 | Education | **Master 1**, IT project management, information systems engineering track (ITIN) |
| 2004 | Education | **BTS Informatique de Gestion** (two-year IT degree), enterprise network administration track (E.C.T.E.I, Groupe ECE, Montreuil) |
| 2002 | Education | **Baccalauréat Scientifique** (French science high school diploma), engineering sciences track (Lycée La Tourelle, Sarcelles) |

---

## Latest articles

I publish regularly on [kamanga.fr/blog](https://kamanga.fr/blog): field feedback, engineering practices taken apart, AI Craft, technical governance. **Posts are written in French**; the titles below are translated for reference.

| Date | Category | Article |
|------|----------|---------|
| 2026-06-17 | Technical debt | [The craft toolkit that keeps an app from dying at 18 months](https://kamanga.fr/fr/dette-technique/boite-a-outils-craft-app-durable) |
| 2026-06-10 | Technical debt | [Cognitive complexity: the lock that keeps debt from coming back](https://kamanga.fr/fr/dette-technique/verrou-complexite-cognitive-code-ia) |
| 2026-05-25 | Technical debt | [5 reasons why your app dies at 18 months](https://kamanga.fr/fr/dette-technique/5-raisons-app-meurt-18-mois) |
| 2026-05-19 | AI | [Who owns the production bug: you or Claude?](https://kamanga.fr/fr/intelligence-artificielle/a-qui-appartient-le-bug-ia) |
| 2026-05-16 | AI | [10x more PRs is not 10x more value shipped: the 4 metrics that lie](https://kamanga.fr/fr/intelligence-artificielle/illusion-productivite-10x-pr) |
| 2026-05-13 | AI | [The Claude code that "works" is often the one that costs you the most](https://kamanga.fr/fr/intelligence-artificielle/faux-ami-code-claude-coute-cher) |
| 2026-05-10 | AI | [All tests green, and three days later it breaks in production](https://kamanga.fr/fr/intelligence-artificielle/code-claude-tests-passent-plante-prod) |
| 2026-05-01 | Technical debt | [Dependabot: setting up your silent teammate against dependency debt](https://kamanga.fr/fr/dette-technique/dependabot-craft-gestion-dependances) |

[**→ See all posts**](https://kamanga.fr/blog)

---

## GitHub stats

<div align="center">

![Profile views](https://komarev.com/ghpvc/?username=kamangacode&style=for-the-badge&color=1A1A2E&label=PROFILE+VIEWS)
![Followers](https://img.shields.io/github/followers/kamangacode?style=for-the-badge&color=1A1A2E&label=FOLLOWERS)
![Stars](https://img.shields.io/github/stars/kamangacode?style=for-the-badge&color=1A1A2E&label=STARS&affiliations=OWNER)
![Repos](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=1A1A2E&label=PUBLIC%20REPOS&query=public_repos&url=https%3A%2F%2Fapi.github.com%2Fusers%2Fkamangacode)

</div>

---

<div align="center">

### Does any of this sound like your situation?

**Let's talk.** No pitch. No sales. 30 minutes to ask the right questions and identify one or two leads.

[**→ Book a call**](https://app.kamanga.fr/forms/discovery-call) · [**→ Follow me on LinkedIn**](https://linkedin.com/in/kamangacode)

</div>
