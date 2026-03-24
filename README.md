# Clawframe

**Clawframe is the systems umbrella for the OpenClaw ecosystem — the frame that keeps Clawforge, Clawguard, and Clawworks legible as first-class systems.**

<p align="center">
  <img src="../artifacts/images/repo-covers/clawframe-10.jpeg" alt="Clawframe cover" width="100%">
</p>

<p align="center">
  <a href="https://github.com/LKCY23/clawforge"><strong>Clawforge</strong></a> ·
  <a href="https://github.com/LKCY23/clawguard"><strong>Clawguard</strong></a> ·
  <a href="https://github.com/LKCY23/clawworks"><strong>Clawworks</strong></a>
</p>

---

## Why this exists

As OpenClaw evolved beyond a single repo, some parts stopped being just folders and became real systems.

Clawframe is the layer that keeps those systems organized, named, and related without collapsing them back into one giant codebase.

It exists to make three things explicit:

- which systems are first-class
- what each system is responsible for
- how they fit together without losing their own boundaries

---

## Current systems

| Local system id | Project | Role |
|---|---|---|
| `self-improving-system` | **Clawforge** | event capture, pattern drafting, cluster-based distillation |
| `constraints` | **Clawguard** | rules, routing, runtime boundaries, governance |
| `development` | **Clawworks** | development-system conventions, programs, repository coordination |

---

## How the pieces relate

```text
Clawframe
├─ Clawforge  -> learning and distillation
├─ Clawguard  -> safety, governance, and boundaries
└─ Clawworks  -> development organization and coordination
```

### High-level interpretation

- **Clawforge** turns experience into durable learning artifacts
- **Clawguard** defines the constraints and governance around action
- **Clawworks** organizes how development itself is planned, reviewed, and advanced
- **Clawframe** keeps these systems coherent as a set

---

## Current state

Clawframe is now a real umbrella repository with child systems managed as submodules.

Current child systems:

- `self-improving-system` -> **Clawforge**
- `constraints` -> **Clawguard**
- `development` -> **Clawworks**

The umbrella stays intentionally light:

- child systems own their own histories
- Clawframe provides orientation, naming, mapping, and structure

---

## Repository structure

```text
systems/
  README.md
  REGISTRY.md
  self-improving-system/   # Clawforge
  constraints/             # Clawguard
  development/             # Clawworks
```

---

## Notes

- Local directory names stay descriptive and readable
- Public GitHub project names are more brand-like:
  - `clawforge`
  - `clawguard`
  - `clawworks`
- Clawframe itself is the umbrella, not a replacement for the systems it contains
