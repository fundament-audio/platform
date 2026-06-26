# DECISION_MODEL

How FUNDAMENT recommends solutions.

This document defines the shared recommendation model used across the entire FUNDAMENT platform.

It describes **how FUNDAMENT thinks**, not **which products to recommend**.

Individual build repositories (S18, S15, D12, M8C, ...) extend this document with build-specific implementation details such as validated drivers, DSP paths, amplifiers, cabinet materials, build paths and services.

In other words:

* **The platform defines how recommendations are made.**
* **Each build defines which validated solutions exist.**

This separation keeps the platform stable while allowing individual builds to evolve independently.

The recommendation process should remain consistent even as drivers, amplifiers, DSP platforms and loudspeaker designs change over time.

---

# Start with the user

Recommendations should always begin with the user's goals.

Never begin with products.

Never begin with brands.

Understand the problem before recommending a solution.

---

# Ask questions first

Before recommending a build, understand:

* What is the primary use case?

  * Music
  * Cinema
  * Studio
  * Mixed

* Is this a new system or an upgrade?

* Stereo, mono or multiple loudspeakers?

* Existing equipment

* Room size and placement constraints

* Budget

* DIY level

* Finish expectations

* Long-term ownership expectations

If the answers are unclear, ask more questions.

---

# Recommend build paths

People build systems.

Not individual components.

Whenever practical, recommend complete build paths instead of isolated parts.

A build path may include:

* loudspeaker
* driver
* DSP
* amplifier
* cabinet material
* finish
* build level

Explain why the combination exists.

---

# Explain tradeoffs

Every engineering decision is a compromise.

Different solutions optimise for different goals.

Examples include:

* music vs cinema
* extension vs efficiency
* simplicity vs flexibility
* cost vs finish
* integrated vs modular electronics

Avoid statements like:

> This is the best.

Prefer:

> This is the most appropriate solution for these goals.

---

# Prefer validated solutions

Official recommendations should always prefer documented and validated engineering.

Clearly distinguish between:

* Official
* Validated
* Planned
* Experimental

Do not present planned or experimental combinations as official FUNDAMENT recommendations.

---

# Prefer modularity

Whenever practical, recommend solutions that remain repairable and upgradeable.

Drivers can be replaced.

Amplifiers can be replaced.

DSP platforms can evolve.

The goal is long-term ownership, not planned replacement.

---

# Services are convenience

DIY, flatpacks, assembled cabinets and complete systems are all valid ways of building and owning a FUNDAMENT design.

Services reduce effort.

They do not change the underlying engineering.

Do not recommend a built-to-order solution because it performs differently.

Recommend it because it matches the user's preferred level of involvement.

---

# Compare philosophies before products

When comparing FUNDAMENT with commercial loudspeakers, begin with philosophy.

Examples include:

* openness
* documentation
* repairability
* upgradeability
* transparency
* validation
* long-term ownership

Specifications matter.

Philosophy determines whether a product still makes sense ten years from now.

---

# Respect uncertainty

If something has not been measured, say so.

If something has not been validated, say so.

If something is still under development, say so.

Honest uncertainty is always better than false certainty.

---

# Scope

This document intentionally does not recommend specific drivers, amplifiers, DSP platforms or cabinet materials.

Those decisions belong to the individual build repositories.

For example:

The FUNDAMENT platform recommends asking whether the system is intended primarily for music or cinema.

The S18 repository explains which validated driver is most appropriate for each of those goals.

The platform defines the decision process.

The build repositories define the validated answers.

---

# The goal

The purpose of this decision model is simple.

Recommend the most appropriate validated solution for the individual user.

Explain the tradeoffs.

Document the reasoning.

Keep improving the knowledge.

The recommendation should still make sense years from now, even if individual drivers, amplifiers, DSP platforms or services have changed.

---

This document is part of the FUNDAMENT platform.

Individual build repositories (S18, S15, D12, M8C, ...) inherit this recommendation model and extend it with build-specific implementation details.

If this document changes, every FUNDAMENT build benefits.
