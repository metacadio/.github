<div align="center">

<img src="https://raw.githubusercontent.com/metacadio/.github/main/profile/logo.png" alt="MetaCAD" width="120" height="120" />

# MetaCAD

**Browser-native maritime CAD.** Rust → WASM. No install. Inspector-grade math.

[![Live on metacad.io]([https://img.shields.io/badge/live-metacad.io-0a3b6e?](https://avatars.githubusercontent.com/u/279407054?s=400&u=979b853fbf0c780ef43003fb4af2a72e269f51e2&v=4)logo=safari&logoColor=white)](https://metacad.io)
[![Benchmarks CI](https://github.com/metacadio/benchmarks/actions/workflows/validate.yml/badge.svg)](https://github.com/metacadio/benchmarks/actions/workflows/validate.yml)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

</div>

---

## What we build

MetaCAD is the first maritime CAD that runs entirely in your browser — **14 modules, 113+ calculators**, all backed by a Rust core compiled to WebAssembly with WebGPU acceleration for Monte-Carlo dynamics.

We replace $15K–$30K Windows-only seats (NAPA, GHS, Cargomax, Paramarine) with a free tier that any class society inspector, surveyor, or chief engineer can open in 30 seconds.

| Domain | What we ship |
|---|---|
| **Stability** | GZ curves (intact + damage), weather criterion, Second-Generation IS (parametric roll, dead-ship, surf-riding, pure loss, excessive accel), 3-DOF Monte-Carlo |
| **Loading & ballast** | LP-optimised stowage, trim, free-surface, longitudinal strength, full Pareto sweep |
| **Emissions compliance** | CII (MEPC.336/354/400), EU ETS Phase 2, FuelEU Maritime, bulk fleet |
| **Bunker reconciliation** | MFM vs BDN per MPA SS 660 + TR 48, Letter of Protest generator, eBDN audit trail |
| **Scantlings** | ISO 12215-5 hull plating + framing |
| **Operations** | Draft Survey (full cycle, 13 port pages), PSC compliance, hull design studio |
| **AI Copilot** | 35 specialised maritime agents — BYOK on your OpenAI / Anthropic / OpenRouter key |

## Why now

- **FuelEU Maritime** first surrender cycle: January 2026 — fleets are mid-audit *right now*.
- **MPA Singapore SS 660** mandatory for all bunker deliveries from Q1 2026.
- **EU ETS Phase 2** — 75% allowances 2026 → 100% 2027.
- **WebGPU + Rust → WASM** crossed mainstream-browser maturity in 2024. The window to be the default browser-native CAD opens once.

## Public repositories

| Repo | What |
|---|---|
| [`benchmarks`](https://github.com/metacadio/benchmarks) | Reproducible validation cases — ONRT capsize MC, KVLCC2 GZ-curve, CII bulk fleet wall-clock. Open-core: fixtures + expected outputs only; runtime is in the closed-source WASM core. |

More repos open as Phase 0 validation milestones land.

## Stack

- **Rust core →** `vesselcalc-wasm` (closed-source, 208/208 cargo tests, 10 modules, 3,500+ LOC)
- **Web →** Next.js + TypeScript ([metacad.io](https://metacad.io), 500/500 vitest tests, ~45 routes)
- **WebGPU shaders →** ocean spectrum (5 wgsl) + Monte-Carlo dynamics (3 wgsl)
- **AI Copilot →** BYOK on user's OpenAI / Anthropic / OpenRouter key — we do not ship inference

## Get in touch

- **Email** — mmotorin@gmail.com
- **Telegram** — [@fxadmins](https://t.me/fxadmins)
- **Founder** — Dmitriy Motorin · [linkedin.com/in/dmotorin](https://www.linkedin.com/in/dmotorin/) · MS Engineering (Naval Architecture), St. Petersburg State Marine Technical University, 2005

We're raising a **$300K SAFE round** (post-money cap $5M) to fund Singapore validation runway. Maritime / deeptech / climate VCs, scouts, angels, class-society partners — reach out.
