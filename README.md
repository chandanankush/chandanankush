# Hi, I'm Chandan 🙏

I build things that talk to each other — iOS and macOS apps, the networks underneath them, and lately the models sitting on top. I'm an Engineering Manager at Paytm Payments Bank, leading Web, Android, iOS, and internal UI engineering across five teams; before that, ~15 years shipping mobile and full-stack software, including consumer-facing work on Paytm and J.P. Morgan Markets/Execute. Swift and networking are my core; everything else is whatever the problem needs.

I'm a mobile engineer by trade and a homelab person by hobby, which means half my repos are Swift packages and the other half are Python or Flask services running on boxes under my desk.

## What I'm working on

- **AIResume** *(private)* — An AI-queryable portfolio site with a from-scratch RAG SDK behind it — chunking, embeddings, vector store, retrieval, reranking, confidence gating — running entirely on self-hosted local models (LM Studio, gemma-4-e4b for chat, bge-m3 for embeddings) so there's no cloud inference cost. It has its own eval harness (frozen manifests, section@1/3 metrics) so I can catch regressions honestly instead of just shipping. Live at [chandan.mopplications.com](https://chandan.mopplications.com/).
- **bank_statement-parser** *(private)* — A multi-tenant service that turns inconsistent Indian bank/credit-card PDF statements into structured, categorized data, with Postgres row-level security keeping each tenant's numbers isolated from every other. Mostly a lesson in how many ways a table can be not-a-table. Live at [txparse.mopplications.com/](https://txparse.mopplications.com/).
- **A GitHub Copilot adoption dashboard** *(private)* — Streamlit analytics for engineering leadership: acceptance rates, per-engineer activity, model-usage breakdown, built to answer "is this actually helping" with numbers instead of vibes.
- **A fail-closed SSH access-window tool** *(private)* — A menu-bar utility for my home server that keeps SSH closed by default and opens a time-bounded, auditable window via fresh macOS authorization — with an independent expiry enforcer that closes it again even if the menu app itself is compromised. The interesting part was writing the actual threat model, not the Swift.
- **AccessibilitySDK** *(private)* — An in-app SDK + Mac scanner pair that walks a running app's live accessibility tree over a local WebSocket and scores it against WCAG rules, including a proper pixel-sampled contrast check — no App Store review or cable required.
- **[dev-tools](https://github.com/chandanankush/dev-tools)** — A growing, self-hosted grid of developer utilities on Next.js 16 with a strict nonce-based CSP and SSRF-safe URL handling. Deployed to a Raspberry Pi via a Jenkins pipeline I built for it.

## Things you can actually use

| | |
|---|---|
| **[LGLogger](https://github.com/chandanankush/LGLogger)** | Dependency-free iOS logging. `print()`-style calls, per-module/per-level filtering, on-disk persistence, one-tap email/HTTP upload, and a floating in-app viewer — with a real test suite and CI behind it. |
| **[lan-devices](https://github.com/chandanankush/lan-devices)** | A SwiftUI macOS app for discovering and managing the SSH-accessible machines on your LAN — Bonjour discovery, TCP reachability checks, and remote shutdown/restart, because `~/.ssh/config` is not a UI. |
| **[dev-tools](https://github.com/chandanankush/dev-tools)** | Self-hosted developer-utility grid, Next.js 16 + strict CSP, shipped as a multi-stage Docker image. |
| **[statix](https://github.com/chandanankush/statix)** | A FastAPI agent + Flask/SQLite server for monitoring CPU, memory, disk, and network across every machine in the homelab, published as a multi-arch Docker image. |
| **[CAAlertView](https://github.com/chandanankush/CAAlertView)** | An anchored SwiftUI selection popover — a 2013 UIKit control rebuilt for SwiftUI, arrow and all, with an iOS-version fallback for the pre-popover era. |
| **[TextToQR](https://github.com/chandanankush/TextToQR)** | A local macOS QR generator with a managed text library, import/export included. Swift, no ceremony. |

## Tech stack

![Swift](https://img.shields.io/badge/-Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/-SwiftUI-0071E3?style=flat-square&logo=swift&logoColor=white)
![Objective-C](https://img.shields.io/badge/-Objective--C-438EFF?style=flat-square&logo=apple&logoColor=white)
![Kotlin](https://img.shields.io/badge/-Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

Plus the parts that don't have a nice logo: URLSession, TCP reachability checks and Bonjour discovery, socket-based protocols (built one for a HIPAA-compliant hospital app early in my career), server-side URL validation against SSRF, Swift Package Manager, SwiftData/Core Data, WidgetKit, Authorization Services and XPC on macOS, self-hosted RAG and retrieval-eval tuning, and a home server that has survived more rebuilds than it should have.

## GitHub stats

![Metrics](./github-metrics.svg)

## Connect with me

[![Website](https://img.shields.io/badge/-chandan.mopplications.com-FF5722?style=flat-square&logo=googlechrome&logoColor=white)](https://chandan.mopplications.com/)
[![LinkedIn](https://img.shields.io/badge/-Chandan_Singh-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/chandan-singh-mobileengineer)
[![Email](https://img.shields.io/badge/-chandan.ankush@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:chandan.ankush@gmail.com)

Open to EM / Staff / Principal conversations in fintech and AI-first product teams — feel free to reach out.
