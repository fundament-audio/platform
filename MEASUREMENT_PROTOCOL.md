
# MEASUREMENT_PROTOCOL

How FUNDAMENT validates loudspeakers.

This document defines the shared measurement philosophy used across all FUNDAMENT builds.

It intentionally starts small.

As the platform evolves, the protocol will evolve with it.

---

# Why measure?

Good engineering should be reproducible.

Measurements allow designs to be validated, revisions to be compared and improvements to be verified.

Simulation predicts.

Measurements verify.

Both matter.

---

# Validation workflow

Every FUNDAMENT build should ideally progress through the following stages.

## 1. Simulation

Every design begins with simulation.

Simulations guide engineering decisions before anything is built.

Whenever practical, simulation files should be published alongside the project.

Simulation is prediction.

It is not validation.

---

## 2. Ground-plane reference measurement

Ground-plane measurement is the primary validation method for FUNDAMENT.

It provides a practical, repeatable and room-independent baseline that can be reproduced by both the project and the community.

Every official reference build should include a documented ground-plane measurement.

This becomes the baseline against which future revisions are compared.

---

## 3. Independent validation

Whenever possible, independent measurements are encouraged.

Examples include:

* Klippel NFS
* anechoic chambers
* Audio Science Review
* universities
* independent laboratories

Independent validation increases confidence in the reference design.

---

## 4. In-room measurements

Rooms are part of every real system.

In-room measurements are encouraged as supplementary information.

They should never replace the reference measurement.

Instead, they demonstrate how the design behaves in real listening environments.

---

# Publish everything

Whenever practical, publish:

* raw measurement data
* processed graphs
* measurement conditions
* equipment used
* software versions

Transparency is more valuable than perfect-looking graphs.

---

# The goal

The purpose of this protocol is not to produce the most measurements.

The purpose is to produce measurements that are honest, repeatable and useful.

Every FUNDAMENT build should answer one simple question:

**Can someone else reproduce these results?**
