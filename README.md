# Balázs Margitai

**Full-stack developer** · Debrecen, Hungary

Two years building software professionally. Today I build internal web
applications at the **University of Debrecen, Faculty of Informatics**; a
monitoring system and a course management platform among them. Before that I
co-founded **Skillion**, an AI EdTech product, and took it from idea to a live
service.

> It reached **~10,000 registered users** and **hundreds of paying subscribers** during that time.

Right now I'm moving toward **AI engineering**: LLM integration is the part of the
stack I want to own, not just consume.

![Professional since 2024](https://img.shields.io/badge/professional_since-2024-0969DA?style=flat-square)
![Focus: full-stack and LLM integration](https://img.shields.io/badge/focus-full--stack_%2B_LLM_integration-8250DF?style=flat-square)
![Open to new roles](https://img.shields.io/badge/status-open_to_new_roles-2EA043?style=flat-square)

[![Connect on LinkedIn](https://img.shields.io/badge/LinkedIn-margitai--balazs--cs-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/margitai-balazs-cs)
[![Email me](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:balazsmargitai@gmail.com)

---

## Selected work

### [Rebrickable API Manager](https://github.com/mbalazs03/rebrickable-api-manager)

[![CI status](https://github.com/mbalazs03/rebrickable-api-manager/actions/workflows/ci.yml/badge.svg)](https://github.com/mbalazs03/rebrickable-api-manager/actions/workflows/ci.yml)

*Java 21 · Spring Boot 3.2 · MongoDB 7 · React 19*
 
Answers "what can I build right now from the bricks I already own?" Owned sets
are merged into one part inventory, then catalogue sets are scored against it and
ranked by completion.
 
**The hard part:** quantities decide it, not membership. Three 2×4 bricks do not
cover a requirement for eight, so every part contributes `min(owned, required)`.
The upstream API allows one request per second, so the client paces itself, and
the paging calls go through a retry wrapper that honours the server's
`Retry-After` interval instead of guessing a backoff. Part lists are cached per
set, which keeps one page of results from costing hundreds of calls.

### [Taskify](https://github.com/mbalazs03/taskify)

[![CI status](https://github.com/mbalazs03/taskify/actions/workflows/ci.yml/badge.svg)](https://github.com/mbalazs03/taskify/actions/workflows/ci.yml)

*Java 21 · Spring Boot · React · PostgreSQL · Docker*
 
Task manager with JWT authentication, role-based access control and an admin
dashboard.
 
**The hard part:** the admin surface is guarded twice over. The URL pattern is
locked to the ADMIN role in the security config, and the controller carries its
own `@PreAuthorize` so the endpoints stay protected even if a route rule is ever
edited. Sessions are stateless, and role changes are checked against an allowlist
rather than written straight from the request body.

---

## Stack

|**Area**|**Tools**|
|---|---|
| **Languages** | TypeScript · JavaScript · Java · Python · C# · SQL |
| **Frontend** | React · Next.js · React Native · Expo · Tailwind · Radix UI · Vite |
| **Backend** | Spring Boot · Flask · FastAPI · Node.js · Express · REST |
| **Data** | PostgreSQL · MongoDB · MySQL |
| **AI** | Claude Code · Cursor · MCP · LLM APIs |
| **Delivery** | Docker · GitHub Actions · Azure · Nginx · Maven · JUnit · Vitest |

I work AI-native day to day: Claude Code, Cursor and MCPs are part of the
toolchain. Data Science MSc in progress at the University
of Debrecen.

---

## Certifications

**6 verified:** NVIDIA, Azure ×2, Java, Python, Databases

[![NVIDIA Generative AI with Diffusion Models](https://img.shields.io/badge/NVIDIA-Generative_AI_with_Diffusion_Models-76B900?style=flat-square&logo=nvidia&logoColor=white)](https://learn.nvidia.com/certificates?id=MFLM5iobQlKuCT6q6oJt3g)
[![AZ-900 Azure Fundamentals](https://img.shields.io/badge/AZ--900-Azure_Fundamentals-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)](https://www.credly.com/badges/f04be3f7-6f97-4b4f-a831-699d0418fb24/public_url)
[![DP-900 Azure Data Fundamentals](https://img.shields.io/badge/DP--900-Azure_Data_Fundamentals-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)](https://www.credly.com/badges/6eacebbf-aa12-448c-827a-bed140901347/public_url)
[![IT Specialist Java](https://img.shields.io/badge/IT_Specialist-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://www.credly.com/badges/301dd53b-dc9e-4736-98cd-99125f3309ea/public_url)
[![IT Specialist Python](https://img.shields.io/badge/IT_Specialist-Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.credly.com/badges/223d4d77-6cb6-4ffc-ba24-70e56aeda81c/public_url)
[![IT Specialist Databases](https://img.shields.io/badge/IT_Specialist-Databases-4479A1?style=flat-square&logo=postgresql&logoColor=white)](https://www.credly.com/badges/61a852ea-dca0-404b-b3aa-1aec5ecd7e15/public_url)

Every badge links to its verification page.

---
