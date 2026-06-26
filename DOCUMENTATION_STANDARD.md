# DOCUMENTATION_STANDARD

How FUNDAMENT repositories are organised.

The goal of FUNDAMENT is not only to build loudspeakers.

The goal is to preserve engineering knowledge in a form that remains understandable, reproducible and maintainable for years to come.

Every repository should be understandable without relying on forum threads, private conversations or disappearing image hosts.

---

# One repository, one build

Every loudspeaker lives in its own repository.

Examples:

* [**S18**](https://github.com/fundament-audio/S18)
* S15
* D12
* M8C

A build repository documents one implementation of the FUNDAMENT platform.

General platform philosophy belongs in the FUNDAMENT repository.

Build repositories only contain build-specific information.

---

# Repository structure

Every build should follow roughly the same structure.

```text
README.md

REFERENCE_BUILD.md
DECISION_MODEL.md
BUILD_PATHS.md

enclosure/
dsp/
bom/
measurements/
validation/
docs/
```

Not every project will need every directory.

The goal is consistency, not rigidity.

---

# README

The README introduces the build.

It should answer:

* What is this?
* Who is it for?
* What is the official reference build?
* Where should the reader go next?

General FUNDAMENT philosophy should be linked, not duplicated.

---

# Reference build

Every build should define one official reference implementation.

This is the combination measured, validated and documented by the project.

Additional build paths may exist.

The reference build always remains the baseline.

---

# Decision model

Every build should document why different options exist.

Not every user wants the same thing.

Examples include:

* different drivers
* different DSP paths
* different amplifiers
* different cabinet materials
* different finishes
* different DIY levels

The goal is not to list every possible combination.

The goal is to document validated choices and the tradeoffs between them.

---

# Build paths

People build systems, not individual parts.

Whenever practical, repositories should document complete build paths rather than isolated components.

Examples:

* Reference
* Budget
* Cinema
* Music
* Plug-and-play
* Premium

Each build path should explain:

* who it is for
* why it exists
* what compromises it makes

---

# Validation

Engineering decisions should be supported by measurements whenever practical.

Validation data should remain with the repository.

Whenever possible, include:

* measurements
* simulations
* design notes
* revision history

Future contributors should understand not only what changed, but why.

---

# Modularity

Every build should document which parts are modular.

Examples include:

* drivers
* amplifiers
* DSP platforms
* cabinet materials
* finishes

When alternative components are supported, document:

* validation status
* intended use case
* advantages
* tradeoffs

Avoid presenting unvalidated combinations as official FUNDAMENT recommendations.

---

# Link back to the platform

Every build repository should link back to the FUNDAMENT platform documents.

General philosophy should not be duplicated.

Instead, build repositories extend the platform with implementation-specific knowledge.

Platform documents always take precedence.

---

# Write for the future

Documentation should answer questions that future builders will have.

Why was this driver chosen?

Why this crossover?

Why this amplifier?

Why this measurement?

Good documentation explains decisions, not only results.

---

# The goal

Someone should be able to discover a FUNDAMENT repository ten years from now and still understand:

* what was built
* why it was built
* how it was measured
* how it can be reproduced
* how it can be repaired
* how it can be improved

If the repository can do that without requiring a forum thread, the documentation has done its job.
