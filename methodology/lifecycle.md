# Shinka Project Lifecycle

## Purpose of This Document

This document defines the **lifecycle model** used by the Shinka methodology.
It describes how a software project progresses over time, how versions are handled,
and what happens before, during, and after a release.

The lifecycle is designed to be:

- Lightweight and explicit
- Suitable for solo developers
- Scalable to small teams (up to ~10 people)
- Iterative, version-based, and feedback-driven

---

## Core Lifecycle Principle

**Shinka is a version-based lifecycle.**

A *project* is not a single lifecycle run.
Instead, a project consists of **multiple versions**, and **each version runs through the lifecycle independently**.

> One project → many versions
> One version → one lifecycle iteration

This allows long-lived projects to evolve in a controlled, intentional way.

---

## Lifecycle Overview

Each version of a project passes through the following phases:

1. **Inception**
2. **Elaboration**
3. **Construction**
4. **Transition**

After Transition, the version enters a **post-release state** that determines what happens next.

The lifecycle is iterative and may repeat multiple times throughout the lifetime of a project.

---

## Lifecycle Phases (High-Level)

### 1. Inception

**Goal:** Establish *why* the version exists and what problem it solves.

Focus areas:

- Vision and intent
- Scope boundaries
- High-level goals
- Initial risks and assumptions

Outcome:

- A clear reason to proceed (or not)
- A consciously limited scope

---

### 2. Elaboration

**Goal:** Decide *what* will be built and *how* it should be structured.

Focus areas:

- Refining requirements
- Architectural decisions
- Risk reduction
- Planning construction work

Outcome:

- A stable enough understanding to begin implementation confidently

---

### 3. Construction

**Goal:** Build the version iteratively and incrementally.

Focus areas:

- Feature implementation
- Testing and validation
- Continuous refinement
- Documentation updates

Outcome:

- A potentially releasable version at all times

---

### 4. Transition

**Goal:** Move the version into actual use.

Focus areas:

- Release preparation
- Deployment
- Validation in real usage
- Final documentation updates

Outcome:

- A released version
- A conscious decision about the future of the project

---

## Post-Transition States (Critical)

After Transition, **every version enters exactly one post-transition state**.
This makes the lifecycle explicit beyond “release”.

### 1. Active (Next Version Planned)

The project continues with a new version.

Typical triggers:

- User feedback
- New ideas
- Strategic changes
- Identified improvements

What happens:

- Monitoring continues
- A new lifecycle iteration starts at **Inception** for the next version
- Earlier versions may enter maintenance

---

### 2. Maintenance Mode

The version is considered stable and complete.

Characteristics:

- No new features planned
- Bug fixes and security updates only
- Minimal documentation changes

Maintenance work usually runs in **small Construction cycles** without full Elaboration.

---

### 3. Paused

The project is intentionally inactive.

Characteristics:

- No active development
- Minimal or no monitoring
- Clear documentation of the paused state

A paused project can later re-enter the lifecycle at Inception.

---

### 4. Archived / End-of-Life

The project is finished.

Characteristics:

- No further development planned
- Final release marked
- Documentation finalized
- Repository archived or clearly labeled

Archiving is considered a valid and successful outcome.

---

## Monitoring and Feedback (Project Continuum)

Monitoring exists **outside individual lifecycle phases** and spans the entire project lifetime.

Monitoring includes:

- Usage observations
- Error reports
- Performance signals
- Developer experience and friction
- Maintenance cost vs. value

Monitoring data feeds decisions such as:

- Starting a new version
- Entering maintenance mode
- Pausing or archiving a project

---

## Lifecycle Compression for Later Versions

Later versions of a project typically:

- Shorten Inception
- Narrow Elaboration
- Focus Construction
- Streamline Transition

However, **no phase is skipped entirely**.
Even minimal versions require conscious intent and scope decisions.

---

## Lifecycle as a Decision Tool

The Shinka lifecycle is not meant to be bureaucratic.
Its primary purpose is to:

- Make decisions explicit
- Prevent unconscious drift
- Support intentional progress
- Reduce long-term cognitive load

The lifecycle should be adapted consciously, never followed blindly.

---

## Relationship to Other Documents

This document defines the *structure*.
Detailed guidance for each phase is provided in:

- `phases/inception.md`
- `phases/elaboration.md`
- `phases/construction.md`
- `phases/transition.md`

Templates and examples are provided separately.
