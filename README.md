# Systems Umbrella

This directory is the umbrella layer for higher-order systems evolving inside the workspace.

## Purpose

The goal of `systems/` is to provide a stable top-level home for distinct systems that are managed as independent repositories and attached here as submodules.

This layer should stay light.
It is not meant to duplicate the full contents of each child system.

## Current structure

```text
systems/
  README.md
  self-improving-system/   # submodule
  constraints/             # submodule
  development/             # submodule
```

## Current first-class child systems

### `self-improving-system`

Purpose:
- manual self-improving workflows
- event capture
- pattern drafting
- cluster-based distillation

This system already has:
- its own repository history
- specs / implementation / review structure
- runtime-facing skill and plugin surfaces
- event / pattern / cluster workflows

### `constraints`

Purpose:
- rules governance
- runtime constraints
- registry routing
- pack/rule structure and maintenance

This system already has:
- its own repository history
- constraint packs, rules, registry, and governance files
- a clear boundary from application-level systems

### `development` -> project **`clawworks`**

Purpose:
- development-system conventions and governance
- program-level planning / status / review / gap tracking
- repository-level design and project-management records

This system should be interpreted as a real system in its own right, not as a generic scratch directory.
Its role is to provide development-system structure rather than end-user runtime behavior.

## Principles

- `systems/` is the umbrella layer, not the main content layer
- only genuinely independent systems should graduate into submodules
- each child system should own its own internal structure, history, and review process
- the umbrella repo should mainly provide orientation, registry-level context, and light coordination

## Current migration outcome

The first-stage umbrella migration is now in place:

- `self-improving-system` promoted into a first-class submodule
- `constraints` promoted into a first-class submodule
- `development` promoted into a first-class submodule

This means `systems/` has now moved from a loose directory convention to an actual systems umbrella repository.

## What should live here

Good fits for the umbrella layer:

- top-level README / orientation
- future architecture or registry index
- light coordination notes across systems
- submodule references to first-class child systems

Bad fits for the umbrella layer:

- duplicating the full internal docs of child systems
- turning the umbrella repo into another giant content repo
- promoting every folder into a submodule too early

## Current note on submodule URLs

The current submodule URLs now point at the formal GitHub HTTPS remotes for the child-system repositories.

Current public repository mapping:

- `systems` -> project **`clawframe`**
- `self-improving-system` -> project **`clawforge`**
- `constraints` -> project **`clawguard`**
- `development` -> project **`clawworks`**
local validation, but may later be replaced by more stable local paths or formal remotes when the multi-repository layout is hardened.
ocally.
They are acceptable for local validation, but may later be replaced by more stable local paths or formal remotes when the multi-repository layout is hardened.
