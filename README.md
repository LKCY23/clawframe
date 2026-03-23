# Systems Umbrella

This directory is the umbrella layer for higher-order systems that are evolving inside the workspace.

## Purpose

The goal of `systems/` is to provide a stable top-level home for distinct systems that may eventually be managed as independent repositories and attached here as submodules.

This layer should stay light.
It is not meant to duplicate the full contents of each child system.

## Current direction

The intended structure is:

```text
systems/
  README.md
  self-improving-system/   # first confirmed independent system
  constraints/             # likely future candidate, not yet promoted here as a submodule by default
```

## Principles

- `systems/` is the umbrella layer, not the main content layer
- only genuinely independent systems should graduate into submodules
- each child system should own its own internal structure, history, and review process
- the umbrella repo should mainly provide orientation, registry-level context, and light coordination

## Current first-class child system

### `self-improving-system`

This is the first clearly independent system under `systems/`.
It already has:

- its own repository history
- specs / implementation / review structure
- runtime-facing skill and plugin surfaces
- event / pattern / cluster workflows

It is the first intended submodule candidate for the `systems/` umbrella.

## Likely future candidate

### `constraints`

`constraints` appears to be another strong candidate for eventual promotion into its own system boundary.
However, it should be evaluated separately rather than bundled into the first migration step automatically.

## Migration strategy

Recommended order:

1. initialize `systems/` as a light umbrella repository
2. keep the umbrella layer minimal
3. attach `self-improving-system` as the first submodule candidate
4. evaluate additional systems only after the first submodule workflow feels clean in practice

## What should live here

Good fits for the umbrella layer:

- top-level README / orientation
- a future architecture or registry index
- light coordination notes across systems

Bad fits for the umbrella layer:

- duplicating the full internal docs of child systems
- turning the umbrella repo into another giant content repo
- promoting every folder into a submodule too early
