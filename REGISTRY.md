# Systems Registry

This file is the lightweight index for the current first-class systems under the `systems/` umbrella.

It is intentionally smaller and less rigid than a full architecture document.
Its purpose is to answer:

- what systems currently exist
- what each system is for
- what stage each system is in
- how they relate at a high level

---

## Current systems

### 1. `self-improving-system`

**Role**
- manual self-improving workflows
- event capture
- pattern drafting
- cluster-based distillation

**Current status**
- active
- independently versioned
- runtime-connected via skill and plugin surfaces
- already usable through `/self-improve ...` and `openclaw self-improve ...`

**Primary artifacts**
- events
- patterns
- reviews
- specs
- implementation source

**Primary concern**
- convert raw experience into durable learning artifacts

**Relationship to other systems**
- depends on `constraints` indirectly for safe/structured behavior boundaries
- uses `development` as a neighboring meta-system for broader development-program organization, not as its direct runtime substrate

---

### 2. `constraints`

**Role**
- rules governance
- runtime constraints
- routing and rule-pack structure
- system-level operational boundaries

**Current status**
- active
- independently versioned
- foundational system

**Primary artifacts**
- constraints entrypoints
- rules packs
- registry routing files
- governance/runtime docs

**Primary concern**
- define and maintain how actions are bounded, routed, and justified

**Relationship to other systems**
- acts as a foundational control layer for behavior and operational safety
- not primarily an artifact-generation system
- likely to remain a lower-level system relative to `self-improving-system`

---

### 3. `development`

**Role**
- development-system conventions and governance
- program-level planning / status / review / gap tracking
- repository-level design and project-management records

**Current status**
- active
- independently versioned
- meta-development system

**Primary artifacts**
- top-level development-system docs
- `programs/` planning/status/review/gaps structure
- `repositories/` project-level design and management records

**Primary concern**
- organize how development work itself is structured and reviewed

**Relationship to other systems**
- meta-system for development organization rather than runtime behavior
- can host planning and design records that influence other systems
- distinct from `self-improving-system`, which focuses on learning artifacts rather than development governance

---

## Current system map

```text
systems/
  self-improving-system/   -> experience distillation system
  constraints/             -> behavior/rule/governance system
  development/             -> development governance / program system
```

---

## High-level relationships

### `constraints` -> foundational guard layer

`constraints` primarily answers:
- what is allowed
- what route to follow
- what governance or safety structure applies

### `self-improving-system` -> learning/artifact layer

`self-improving-system` primarily answers:
- what happened
- what should be learned
- what pattern or event should be retained

### `development` -> meta-development organization layer

`development` primarily answers:
- how development work is planned
- how repository/program status is tracked
- how system-building efforts are reviewed and advanced

---

## Current maturity view

### Stable enough to operate now
- `constraints`
- `self-improving-system`

### Stable enough to treat as a first-class system, but still meta-layer oriented
- `development`

---

## Notes

- This registry is intentionally lightweight.
- It should be updated when a new first-class system is promoted into the umbrella, or when one system's role materially changes.
- If cross-system interfaces become richer and more stable, a future `ARCHITECTURE.md` may become worthwhile.
