---
title: "Project Manifesto"
summary: "What is this project about?"
date: 2022-02-11
weight: 2
---

Our goal is to create an open standard for feature flag management to support a robust feature flag ecosystem using cloud native technologies.

The scope includes:
- An **open standard** that allows adopters and vendors to easily integrate with spec-compliant feature flag solutions
- Creating a **vendor-agnostic ecosystem** supported by the CNCF that provide a seamless experience for developers, SREs, and vendors
- Providing Unified API and SDK;
- Developer-first, cloud-native reference implementation; 
- Ensuring extensibility for open source and commercial offerings.

## Why?

There are many existing solutions, open source or not.
Unfortunately they lack key features needed for wide adoption
by companies and in the open source ecosystem:

- **Many SDKs** doing the same thing, but slightly differently
- Many companies **“rebuilding” the wheel**
- SDKs are generally open source but have no ecosystem
- **“Vendor” lock-in** at code-level
- **No collaboration** across vendors. 
- **Missing integration** with observability tools (e.g. OpenTelemetry)

## Differentiators

This project is more than just copy and paste of existing solutions

* Current solutions often have **eval logic in SDKs**.
  This may require **updating all your apps** for a new rule type.
* Config in Feature Flagging tools that are **separate from the rest of the app** make it harder to use approaches like GitOps. 
* Config and rule changes are **hard to integrate into observability** tools 
* Information to decide on features already available in observability tools is **not leveraged and collected twice**
* No **agreed on grammar/structure** for rules which could be automatically validated (e.g. with CUE)
