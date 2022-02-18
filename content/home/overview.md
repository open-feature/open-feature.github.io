---
title: "Overview of OpenFeature"
summary: "What is OpenFeature?"
date: 2022-02-18
weight: 1
---

OpenFeature is an **open standard** for feature flag management, created to support a robust feature flag ecosystem using cloud native technologies. OpenFeature will provide a **unified API and SDK**, and a **developer-first, cloud-native implementation**, with **extensibility for open source and commercial offerings**.

## Why are we doing this?

Feature flags have become an essential tool in the modern software delivery lifecycle. However, for some, the entry barrier is still too high. Standardizing feature flag management allows organizations to confidently and easily get started using feature flags, knowing that a vendor neutral SDK helps them avoid lock-in, enabling them to focus on building great software.

## How does it work?

OpenFeature's cloud native architecture allows teams to get started with feature flag management quicker than ever. By utilizing the [Operator pattern](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/), OpenFeature is enterprise-grade and easy to install. Configurations are stored as a [custom resource definition](https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/) and flag evaluation can also be centralized as a [sidecar](https://kubernetes.io/docs/concepts/workloads/pods/#how-pods-manage-multiple-containers) or [headless service](https://kubernetes.io/docs/concepts/services-networking/service/#headless-services), drastically reducing the complexity of the SDKs while providing low overhead.

Planned [OpenTelemetry](https://opentelemetry.io) support will mean feature flag metadata can be attached to distributed traces, logs, and metrics, providing the ability to quickly determine the impact a new feature has on your application. It will also allow developers to utilize features such as [baggage](https://opentelemetry.io/docs/reference/specification/baggage/api/), allowing feature flag metadata to be a part of the shared distributed context.

## Join Us

If you're interested in learning more or becoming involved, consider joining the [OpenFeature community](./community.md).

