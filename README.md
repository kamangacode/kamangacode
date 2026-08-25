<div align="center">

# Hervé "Kamanga" Muludiki

### Software Craftsman · Coach Craft + IA · Développeur Full Stack

*Reprendre la maîtrise de son code, à l'ère de l'IA.*

[![Website](https://img.shields.io/badge/Website-kamanga.fr-0A0A0A?style=for-the-badge&logo=safari&logoColor=white)](https://kamanga.fr)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-kamangacode-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kamangacode)
[![YouTube](https://img.shields.io/badge/YouTube-@kamangacode-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@kamangacode)
[![X](https://img.shields.io/badge/X-@kamangacode-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/kamangacode)
[![Email](https://img.shields.io/badge/Email-herve@kamanga.fr-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:herve@kamanga.fr)

**🇫🇷 Français** · [🇬🇧 English](README.en.md)

</div>

---

## À propos

J'aide les équipes techniques et leurs managers à **reprendre la maîtrise de leurs systèmes**. 25 ans de terrain comme tech lead, CTO fractionné et coach technique au sein de grands comptes (BNP Paribas, Crédit Agricole, Canal+, Agirc-Arrco, Société Générale, JCDecaux, Air France).

Aujourd'hui, mon activité est centrée sur un seul axe :

- **[Coach Craft + IA](https://www.kamanga.fr/)** : transformation de la culture d'ingénierie (Clean Architecture, DDD, TDD, pair programming, qualité logicielle) et gouvernance de l'IA dans le cycle de dev (cadre commun, sécurité du code généré, coût maîtrisé)

### Le Craft IA, ma conviction actuelle

> *L'art d'utiliser l'IA pour construire des applications bien faites, avec un budget extrêmement maîtrisé.*

L'IA accélère la production. Elle ne remplace pas le jugement. Les équipes qui sortiront gagnantes de cette transition seront celles qui comprennent ce qu'elles construisent. C'est exactement sur ce terrain que j'interviens.

---

## Projets en cours

### Conduit Full Stack

Un vrai projet full-stack TypeScript, tenu comme un projet de production : monorepo `api` +
`web` + `shared` en NestJS, Next.js et Zod, qui implémente la spec
[RealWorld](https://realworld-docs.netlify.app/) (nom de code *Conduit*, un clone de Medium
avec articles, commentaires, favoris et suivi d'auteurs).

[![conduit-fullstack](https://img.shields.io/badge/GitHub-conduit--fullstack-0A0A0A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kamangacode/conduit-fullstack)

**L'enjeu.** Ce qui sépare un projet qui tient dix ans d'un projet ingérable à 18 mois, ce
n'est presque jamais le talent des équipes : c'est le cadre posé dès le premier jour.
Problème, ce cadre se raconte mal en slides. Il se lit dans les fichiers.

**Le pourquoi.** Rendre ce cadre concret et vérifiable. Le périmètre fonctionnel étant figé
par la spec RealWorld, tout le *quoi* est déjà décidé : reste le *comment*, et c'est
exactement ce que ce dépôt expose. C'est aussi l'implémentation exécutable du
[Référentiel Craft](https://www.kamanga.fr/referentiel-craft), mes 25 ans de pratique
condensés en 100 pratiques sur 21 phases.

**Ma méthodologie.** Chaque incrément suit le même trajet, et laisse une trace à chaque
étape : cadrer (PRD, hors périmètre explicite), spécifier (exigences versionnées avec leurs
critères d'acceptation), décider (ADR immuables), implémenter (le code et ses tests dans la
même unité, sur une branche issue de `staging`), relire et livrer (review en Conventional
Comments, promotion `staging` vers `main`). Un travail interrompu se reprend sans
reconstituer le contexte de tête.

**Ce que je montre dans ce projet :**

- **Architecture hexagonale** : ports dans le domaine, adapters dans l'infrastructure, un domaine pur sans un seul import de NestJS ou de Prisma.
- **DDD et Clean Architecture** : bounded contexts, aggregate root immuable, value objects validés, règle de dépendance tenue sur 4 couches.
- **Un modèle partagé unique** : le schéma Zod est l'unique définition, le type TypeScript en est inféré. La cohérence front/back devient une dépendance de compilation, pas un contrat à synchroniser.
- **Stratégie de tests** : suite de conformité RealWorld vendorée au SHA (128 tests Playwright, jamais éditée), couverture exigée par couche, garde-fou anti run vert et creux.
- **Qualité outillée** : Biome, complexité cognitive bloquante en CI, dependency-cruiser sur les frontières hexagonales, knip sur le code mort.
- **Requirements as code** : exigences versionnées, frontmatter validé par schéma, matrice de traçabilité exigences vers tests générée en CI.
- **Sécurité by design** : validation d'environnement fail-fast au boot, anti-IDOR filtré en SQL, autorité serveur sur l'auteur, secrets hors dépôt, modèle de menace documenté.
- **Documentation as code** : ADR immuables avec gate automatique, guides, standards, tout en Markdown versionné.
- **Livraison** : Conventional Commits, flux `feature` vers `staging` vers `main` par promotion, merge commit jamais squash.
- **Workflow agentique et SDLC** : le cycle outillé que j'utilise au quotidien, sous gates humaines.

> **Ce dépôt est fait pour être lu, pas seulement cloné.** Chaque garde-fou est un vrai
> fichier commenté, lisible sans contexte additionnel. Ouvre-en un au hasard.
>
> [**→ Explorer conduit-fullstack**](https://github.com/kamangacode/conduit-fullstack) · [**→ Découvrir Le Référentiel Craft**](https://www.kamanga.fr/referentiel-craft)

### CRM Coaching

Application SaaS pour coachs professionnels (Next.js 16, NestJS 11, Prisma, architecture hexagonale, IA intégrée). 100% codée en Craft IA.

<p align="center">
  <img src="ressources/crm-cosching-lead.png" alt="Aperçu fiche lead CRM Coaching" width="800" />
</p>

### Autres

- **[Blog kamanga.fr](https://kamanga.fr/blog)** : vulgarisation du software craftsmanship et du Craft IA.
- **Chaîne YouTube [@kamangacode](https://youtube.com/@kamangacode)** : tutos, retours d'expérience, dissection des pratiques d'ingénierie modernes.

---

## Ce que je crois, sans compromis

- La **qualité logicielle** est une décision business, pas une option technique.
- La **dette technique** est une dette financière. Elle a un coût réel, mesurable.
- Le **craftsmanship** est un garde-fou, pas un dogme.
- L'**IA** augmente l'urgence du jugement humain, elle ne l'élimine pas.
- Une bonne **transformation** rend les équipes autonomes, pas dépendantes du consultant.

---

## Tech Stack

### IA et Agents

![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor-000000?style=for-the-badge&logo=cursor&logoColor=white)

### Frontend et Full Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_16-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn/ui-000000?style=for-the-badge&logo=shadcnui&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=for-the-badge&logo=react&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)

### Backend et Data

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS_11-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Java](https://img.shields.io/badge/Java_25-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma_7-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3068B7?style=for-the-badge&logo=zod&logoColor=white)
![Better Auth](https://img.shields.io/badge/Better_Auth-000000?style=for-the-badge&logo=auth0&logoColor=white)

### Tests et Qualité

![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Cucumber](https://img.shields.io/badge/Cucumber-23D96C?style=for-the-badge&logo=cucumber&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white)
![Biome](https://img.shields.io/badge/Biome-60A5FA?style=for-the-badge&logo=biome&logoColor=white)

### DevOps et Infrastructure

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white)

### Architecture et Méthodologies

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

### Conformité et réglementation

![RGPD](https://img.shields.io/badge/RGPD-1E3A8A?style=for-the-badge)

---

## Certification et formation

| Année | Type | Intitulé |
|------:|------|----------|
| 2023 | Certification | Certification de Manager (Ecole 109) |
| 2023 | Formation | **Executive MBA** Management et Entrepreneuriat IT (Epitech Executive, Paris) |
| 2023 | Formation | **Direction des Systèmes d'Information** (IB Cegos, Paris) : plan directeur, transformation numérique, gouvernance, performance financière, gestion des risques, méthodes agiles |
| 2021 | Certification | Certified Scrum Master (Scrum Alliance) |
| 2021 | Certification | Coach Praticien (Coach Académie, Paris) |
| 2008 | Formation | **Master 2** Manager en ingénierie informatique, réseaux et télécoms, option Système d'information bancaire (M2IRT, ITIN / CCI Versailles) |
| 2007 | Formation | **Master 1** Chargé de projets informatique, option Ingénierie des systèmes d'information (ITIN) |
| 2004 | Formation | **BTS Informatique de Gestion**, option Administrateur de réseau local d'entreprise (E.C.T.E.I, Groupe ECE, Montreuil) |
| 2002 | Formation | **Baccalauréat Scientifique**, option Sciences de l'ingénieur (Lycée La Tourelle, Sarcelles) |

---

## Mes derniers articles

Je publie régulièrement sur [kamanga.fr/blog](https://kamanga.fr/blog) : retours terrain, dissection de pratiques d'ingénierie, Craft IA, gouvernance technique.

| Date | Catégorie | Article |
|------|-----------|---------|
| 2026-06-17 | Dette technique | [La boîte à outils craft qui empêche une app de mourir à 18 mois](https://kamanga.fr/fr/dette-technique/boite-a-outils-craft-app-durable) |
| 2026-06-10 | Dette technique | [Complexité cognitive : le verrou qui empêche la dette de revenir](https://kamanga.fr/fr/dette-technique/verrou-complexite-cognitive-code-ia) |
| 2026-05-25 | Dette technique | [5 raisons pour lesquelles votre app meurt à 18 mois](https://kamanga.fr/fr/dette-technique/5-raisons-app-meurt-18-mois) |
| 2026-05-19 | IA | [À qui appartient le bug en prod : toi ou Claude ?](https://kamanga.fr/fr/intelligence-artificielle/a-qui-appartient-le-bug-ia) |
| 2026-05-16 | IA | [10x plus de PR ≠ 10x plus de valeur livrée : les 4 métriques qui mentent](https://kamanga.fr/fr/intelligence-artificielle/illusion-productivite-10x-pr) |
| 2026-05-13 | IA | [Le code Claude « qui marche » est souvent celui qui coûte le plus cher](https://kamanga.fr/fr/intelligence-artificielle/faux-ami-code-claude-coute-cher) |
| 2026-05-10 | IA | [Tous les tests sont verts, et 3 jours plus tard ça plante en prod](https://kamanga.fr/fr/intelligence-artificielle/code-claude-tests-passent-plante-prod) |
| 2026-05-01 | Dette technique | [Dependabot : configurer son coéquipier silencieux contre la dette](https://kamanga.fr/fr/dette-technique/dependabot-craft-gestion-dependances) |

[**→ Voir tous les articles**](https://kamanga.fr/blog)

---

## Stats GitHub

<div align="center">

![Profile views](https://komarev.com/ghpvc/?username=kamangacode&style=for-the-badge&color=1A1A2E&label=PROFILE+VIEWS)
![Followers](https://img.shields.io/github/followers/kamangacode?style=for-the-badge&color=1A1A2E&label=FOLLOWERS)
![Stars](https://img.shields.io/github/stars/kamangacode?style=for-the-badge&color=1A1A2E&label=STARS&affiliations=OWNER)
![Repos](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=1A1A2E&label=PUBLIC%20REPOS&query=public_repos&url=https%3A%2F%2Fapi.github.com%2Fusers%2Fkamangacode)

</div>

---

<div align="center">

### Tu reconnais ta situation dans ce que je décris ?

**On peut parler.** Pas de pitch. Pas de vente. 30 minutes pour poser les bonnes questions et identifier une ou deux pistes.

[**→ Réserver un échange**](https://app.kamanga.fr/forms/discovery-call) · [**→ Me suivre sur LinkedIn**](https://linkedin.com/in/kamangacode)

</div>
