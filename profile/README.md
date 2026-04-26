# MetaCAD

**Browser-native maritime CAD.** Rust → WASM. No install. Inspector-grade math.

Live product → **[metacad.io](https://metacad.io)**

---

## What we build

MetaCAD is the first maritime CAD that runs entirely in your browser — 14 modules, 113+ calculators, all backed by a Rust core compiled to WebAssembly with WebGPU acceleration for Monte-Carlo dynamics.

We replace $15K–$30K Windows-only seats (NAPA, GHS, Cargomax, Paramarine) with a free tier that any class society inspector, surveyor, or chief engineer can open in 30 seconds.

Modules cover **stability** (GZ curves, intact + damage, weather criterion, second-generation IS), **loading & ballast** (LP-optimised stowage, trim, free-surface, longitudinal strength, 3-DOF MC), **emissions compliance** (CII, EU ETS, FuelEU, bulk fleet), **MFM bunker reconciliation** (MPA SS 660 + TR 48), **scantlings** (ISO 12215-5), **draft survey**, **PSC**, **hull design**, and an **AI Copilot** with 35 specialised maritime agents.

## Why now

- **FuelEU Maritime** first surrender cycle: January 2026 — fleets mid-audit right now.
- **MPA Singapore SS 660** mandatory for all bunker deliveries from Q1 2026.
- **EU ETS Phase 2** — 75% allowances 2026 → 100% 2027.
- **WebGPU + Rust → WASM** crossed mainstream-browser maturity in 2024.

## Public repositories

| Repo | What |
|---|---|
| [`benchmarks`](https://github.com/metacadio/benchmarks) | Reproducible validation cases — ONRT capsize MC, KVLCC2 GZ-curve, CII bulk fleet wall-clock. Open-core: fixtures + expected outputs only; runtime is in the closed-source WASM core. |

More repos open as Phase 0 validation milestones land.

## Stack

**Rust core →** [`vesselcalc-wasm`] (closed-source, 208/208 cargo tests, 10 modules, 3,500+ LOC).
**Web →** Next.js + TypeScript ([metacad.io](https://metacad.io), 500/500 vitest tests, ~45 routes).
**WebGPU shaders →** ocean spectrum (5 wgsl) + Monte-Carlo dynamics (3 wgsl).
**AI Copilot →** BYOK on user's OpenAI / Anthropic / OpenRouter key — we do not ship inference.

## Get in touch

- **Email** — mmotorin@gmail.com
- **Telegram** — [@metacad_support](https://t.me/metacad_support)
- **Founder** — Dmitriy Motorin · [linkedin.com/in/dmotorin](https://www.linkedin.com/in/dmotorin/) · MS Engineering (Naval Architecture), St. Petersburg State Marine Technical University, 2005

We're raising a $300K SAFE round (post-money cap $5M) to fund Singapore validation runway. If you're a maritime / deeptech / climate VC, scout, angel, or class-society partner — reach out.
