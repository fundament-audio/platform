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

Every build follows roughly the same structure.

A build starts small and grows. Early on, a README and a single documented path are enough. The rest is added as the build matures.

```text
README.md              # always

REFERENCE_BUILD.md     # once a reference build is defined
BUILD_PATHS.md         # once more than one path exists
DECISION_MODEL.md      # build-specific extensions, once options diverge

enclosure/
dsp/
bom/
research/              # exploration, simulation, design notes
measurements/          # raw measured data
validation/            # later: confirmation the reference build meets its targets
docs/
```

Not every project needs every file or directory.

Most early builds only need a README, one build path and some research.

The goal is consistency, not rigidity. Add structure when the project earns it, not before.

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

Every build should eventually define one official reference implementation.

This is the combination measured, validated and documented by the project.

Early on, the reference build can be described directly in the README. A dedicated REFERENCE_BUILD.md becomes useful once that description outgrows it.

Additional build paths may exist later.

The reference build always remains the baseline.

---

# Decision model

Once a build offers more than one option, it should document why those options exist.

A build with a single path does not need this yet. It becomes useful as soon as the choices begin to diverge.

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

With a single path, the reference build is the only path, and the README is enough. A dedicated BUILD_PATHS.md becomes useful once a second path exists.

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

# Research and validation

These are two different activities, and they belong to different stages.

**Research** is exploratory. It is the work done while a build is still being figured out: driver comparisons, box simulations, modelling, design notes, dead ends. Early builds are almost entirely research. This lives in `research/`.

**Validation** is confirmation. It is the evidence that the finished reference build meets its documented targets: final measurements against the stated goals, revision history, sign-off. This is a later-stage activity. It lives in `validation/`, and an early build will not have it yet.

Validation is not limited to the project's own measurements. Independent reproductions by other builders — someone following the published plans and confirming the same results — are among the strongest validation a build can have. Those contributed builds and measurements belong in `validation/` too.

Raw measured data lives in `measurements/` and can feed either.

Whatever stage a build is at, the supporting data should stay in the repository rather than in forum threads or private files.

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
