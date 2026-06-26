# FUNDAMENT

[Website](#) · [Community](https://www.audiosciencereview.com/forum/index.php?threads/fundament-an-open-source-fully-documented-subwoofer-platform-build-001-sealed-18%E2%80%B3-bms-18n862-fa502.72012/) · [Current builds](#current-builds) · [Principles](#core-principles)

---

**Open-source, fully measured loudspeaker design.** 

Reference-level audio hardware that is modular, validated, documented, measurable, repairable and reproducible, and built to stay that way. 

Open by design. Enhanceable and modular, based on needs.
They can be either fully built DIY, commissioned locally, or — where available — built to order.

Serious loudspeakers without black-box lock-in.

---

# What is FUNDAMENT?

FUNDAMENT is a community-driven platform for open loudspeaker design. It exists to make reference-level loudspeaker engineering transparent, modular, reproducible and buildable anywhere in the world.

Good loudspeakers are often hard or expensive to get hold of, and serious subwoofers most of all. Shipping heavy cabinets internationally, import duties, VAT, limited local availability and manufacturer lock-in put many of today's best designs out of reach for much of the community.

At the same time, plenty of excellent DIY designs already exist. The engineering behind them is usually scattered across forum threads, personal websites and image hosts that eventually disappear, so valuable knowledge is easily lost.

FUNDAMENT exists to solve both problems. We take known-good engineering, document it properly, validate it openly and publish it as complete, reproducible reference designs.

The platform is the method. Each loudspeaker is a build on top of it.

---

# What FUNDAMENT is (and isn't)

FUNDAMENT is an open engineering platform for modular loudspeaker systems.

It is **not** a closed loudspeaker brand. The engineering is public first: enclosure design, driver selection, DSP & Amp selection and settings, measurements, BOMs, revision history and build paths remain open.

Some FUNDAMENT builds may also be available as built-to-order systems. Buying one is a convenience path, not a paywall around the design.

Individual repositories (S18, S15, M8C and so on) implement specific loudspeaker designs using the shared principles, documentation standards, measurement methodology and recommendation model defined by the platform.

The goal is not simply to publish loudspeaker plans. The goal is to preserve engineering knowledge.

---

# How can I own a FUNDAMENT system?

There are multiple ownership paths:

| Path | For whom | What you get |
|---|---|---|
| **DIY build** | Builders, engineers, hobbyists | Plans, BOM, DSP files, measurements and validation data |
| **Partial DIY / Partial BTO** | Half builder, half buyer | Buy a flat pack, do the DSP config on your own – or the other way around. You don't have to DIY everything |
| **Local build / cabinetmaker** | People who want local sourcing | Same open design, built by someone near you |
| **Built-to-order** | People who want a finished system | A completed FUNDAMENT build assembled to the published reference design |

All paths use the same open engineering.  
The difference is effort, not access.

---

# Current builds

| Build                                          | Description                         | Status            |
| ---------------------------------------------- | ----------------------------------- | ----------------- |
| [**S18**](https://github.com/fundament-audio/S18) | Sealed 18″ reference subwoofer   | 🟡 Initial design |
| **S15**                                        | Sealed 15″ reference subwoofer      | ⚪ Concept         |
| **D12**                                        | Dual 12″ force-cancelling subwoofer | ⚪ Concept         |
| **M8C**                                        | Active 4×8″ cardioid module         | ⚪ Concept         |

--- 

# Platform documents

These documents define FUNDAMENT itself and apply to every build.

| Document                                              | Purpose                                                           |
| ----------------------------------------------------- | ----------------------------------------------------------------- |
| **README.md**                                         | Introduction to the platform (you are here)                       |
| [**PHILOSOPHY.md**](./PHILOSOPHY.md)                   | Why FUNDAMENT exists and the principles behind every build        |
| [**DECISION_MODEL.md**](./DECISION_MODEL.md)           | How FUNDAMENT recommends validated solutions and build paths      |
| [**MEASUREMENT_PROTOCOL.md**](./MEASUREMENT_PROTOCOL.md) | Shared measurement and validation methodology                   |
| [**DOCUMENTATION_STANDARD.md**](./DOCUMENTATION_STANDARD.md) | Repository structure and documentation conventions          |
| [**AGENTS.md**](./AGENTS.md)                                   | Guidance for contributors, AI assistants and future configurators |

Every build repository extends these documents rather than redefining them.

---

# Core principles

Every FUNDAMENT build should be:

* Open enclosure designs
* Modularity in mind
* Open DSP presets and protection filters
* Measured using a published protocol
* Revision controlled
* Built from accessible off-the-shelf parts
* Repairable
* Upgradeable
* Reproducible

If it isn't documented, measurable and reproducible, it isn't FUNDAMENT.

## Why modular matters

A conventional active subwoofer often becomes obsolete when one proprietary part fails.

A FUNDAMENT build is designed as a serviceable platform:

```text
Cabinet
  ├── Driver: replaceable / upgradable
  ├── Amplifier: replaceable
  ├── DSP: portable presets / documented filters
  ├── Protection: documented, not hidden
  ├── Finish: build-path dependent
  └── Measurements: public baseline for future revisions
```

The cabinet should last decades.
The electronics do not have to.

---

# Repository structure

This organisation contains two kinds of repositories.

## Platform

The platform repository defines the shared methodology. It contains the philosophy, recommendation model, documentation standards and measurement protocol used by every FUNDAMENT build.

## Builds

Each loudspeaker lives in its own repository. A build repository contains only build-specific information, such as:

* enclosure drawings
* CAD
* bill of materials
* DSP presets
* measurements
* validation data
* build paths

Everything that applies to every loudspeaker stays in the platform documentation.

---

# What "reference-level" means

Reference-level means one thing: a documented reference design validated against a published measurement protocol.

The measured reference build is the benchmark. Community builds are expected to follow the same protocol so results stay comparable.

It does not mean every home-built loudspeaker automatically becomes reference-grade. Material selection, machining accuracy, assembly quality and component tolerances all influence the final result.

FUNDAMENT therefore promises transparency rather than perfection. The design, measurements, methodology and raw data stay open so anyone can understand, reproduce and improve the work.

Independent validation is actively encouraged, whether from Klippel NFS, anechoic measurements, Audio Science Review, universities, laboratories or experienced community members.

---

# Contributing

FUNDAMENT is intended to be a long-term community project.

You can contribute by:

* building a design
* measuring it using the published protocol
* submitting measurement data
* improving documentation
* proposing revisions
* reviewing engineering decisions
* contributing CAD, DSP or tooling improvements

Independent measurements are especially valuable.

---

# Built-to-order (future)

Not everyone wants to become a loudspeaker builder.

In the future, complete FUNDAMENT builds may also be offered as hand-built systems assembled in Denmark. The engineering always stays open. Plans, documentation, measurements, DSP presets and design files remain public.

Built-to-order exists purely as a convenience service. It is not a paywall around the knowledge.

---

# Licence

Hardware / designs
CERN-OHL-S-2.0

Documentation / measurements
CC BY-SA 4.0

Code / scripts
MIT

---

**Let's build something nice together.**
