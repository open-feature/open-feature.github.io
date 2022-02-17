---
title: "Principles of OpenFeature"
summary: "What is this project about?"
date: 2022-02-18
weight: 1
---

## Overview

OpenFeature is an **open standard** for feature flag management, created to support a robust feature flag ecosystem using cloud native technologies. OpenFeature will provide a **unified API and SDK**, and a **developer-first, cloud-native implementation**, with **extensibility for open source and commercial offerings**.

## Why are we doing this?

Feature flags have become an essential tool in the modern software delivery lifecycle. However, for some, the entry barrier is still too high. Standardizing feature flag management allows organizations to confidently and easily get started using feature flags, knowing that a vendor neutral SDK helps them avoid lock-in, enabling them to focus on building great software.

## How does it work?

OpenFeature's cloud native architecture allows teams to get started with feature flag management quicker than ever. By utilizing an [Operator pattern](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/), OpenFeature is enterprise-grade and easy to install. Configurations are stored as a [CRD](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) and flag evaluation can also be centralized as a [sidecar](https://kubernetes.io/docs/concepts/workloads/pods/#how-pods-manage-multiple-containers) or [headless service](https://kubernetes.io/docs/concepts/services-networking/service/#headless-services), drastically reducing the complexity of the SDKs while providing low overhead.

OpenFeature will support OpenTelemetry, which will add feature flag metadata to distributed traces. That will provide the ability to quickly determine the impact a feature has on a system. It will also allow developers to utilize features such as [baggage](https://opentelemetry.io/docs/reference/specification/baggage/api/), allowing context to be shared across distributed services.

## Join Us

If you're interested in learning more or becoming involved, consider joining the [OpenFeature community](./community.md).

<!--
### Improved end user experience

- Kubernetes native
-

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

- Current solutions often have **eval logic in SDKs**.
  This may require **updating all your apps** for a new rule type.
- Config in Feature Flagging tools that are **separate from the rest of the app** make it harder to use approaches like GitOps.
- Config and rule changes are **hard to integrate into observability** tools
- Information to decide on features already available in observability tools is **not leveraged and collected twice**
- No **agreed on grammar/structure** for rules which could be automatically validated (e.g. with CUE)
 -->