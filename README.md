# Awesome-GitOps with stars

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list for awesome GitOps resources inspired by [@sindresorhus' awesome](https://github.com/sindresorhus/awesome) ⭐ 502,597 | 🐛 105 | 📅 2026-09-02

We follow this [code of conduct](CODE-OF-CONDUCT.md).

## What is GitOps? <!-- omit in toc -->

GitOps is a way to do Kubernetes cluster management and application delivery.
It works by using [Git](https://git-scm.com/) as a single source of truth for
[declarative infrastructure and applications](https://en.wikipedia.org/wiki/Infrastructure_as_code),
together with tools ensuring the *actual state* of infrastructure and
applications converges towards the *desired state* declared in Git. With Git at
the center of your delivery pipelines, developers can make pull requests to
accelerate and simplify application deployments and operations tasks to your
infrastructure or container-orchestration system (e.g. [Kubernetes](https://kubernetes.io/)).

<p align="center"><img src="img/gitops_conceptual_diagram.svg" alt="Conceptual diagram of GitOps-based infrastructure" width="800px" /></p>

## Why is GitOps awesome? <!-- omit in toc -->

It [increases developer productivity](https://www.weave.works/technologies/gitops/#key-benefits), [enhances developer experience](https://www.weave.works/technologies/gitops/#key-benefits), [improves stability](https://www.weave.works/technologies/gitops/#key-benefits), all while having [higher reliability](https://www.weave.works/technologies/gitops/#key-benefits), [higher consistency](https://www.weave.works/technologies/gitops/#key-benefits) and [stronger security guarantees](https://www.weave.works/technologies/gitops/#key-benefits).

Modern software development practices *assume* support for reviewing changes, tracking history, comparing versions, and rolling back bad updates; GitOps applies the same tooling and engineering perspective to managing the systems that deliver direct business value to users and customers.

<!-- toc -->

* [Background](#background)
* [Tools](#tools)
* [Ancillary Tools](#ancillary-tools)
  * [Notifications](#notifications)
  * [Secrets](#secrets)
* [Tutorials](#tutorials)
* [Community](#community)

<!-- tocstop -->

## Background

* [Operations by pull request](https://www.weave.works/blog/gitops-operations-by-pull-request) - a blog entry about how GitOps came about at Weaveworks
* [GitOps.tech](https://www.gitops.tech/) - a summary of how GitOps works
* [GitOps Conversation Kit](https://gitops-community.github.io/kit/) - How to showcase GitOps awesomeness and convince all stakeholders to implement it
* [GitOps Working Group](https://github.com/gitops-working-group/gitops-working-group) ⚠️ Archived - GitHub repo of GitOps working group under the CNCF App Delivery SIG.

## Tools

* [ArgoCD](https://github.com/argoproj/argo-cd) ⭐ 24,069 | 🐛 4,389 | 🌐 Go | 📅 2026-09-03 - Declarative continuous deployment for Kubernetes
* [Flux](https://github.com/fluxcd/flux2) ⭐ 8,381 | 🐛 256 | 🌐 Go | 📅 2026-09-03 - Open and extensible continuous delivery solution for Kubernetes. Powered by GitOps Toolkit
* [Flagger](https://github.com/weaveworks/flagger) ⭐ 5,397 | 🐛 387 | 🌐 Go | 📅 2026-09-02 - Progressive delivery Kubernetes operator (Canary, A/B testing and Blue/Green deployments automation)
* [Ignite](https://github.com/weaveworks/ignite) ⚠️ Archived - A Virtual Machine manager with a container UX and built-in GitOps
* [Kubefirst](https://github.com/kubefirst/kubefirst) ⭐ 2,058 | 🐛 289 | 🌐 Go | 📅 2026-02-25 - Fully-automated OSS delivery & infrastructure management gitops platforms
* [Sceptre](https://github.com/Sceptre/sceptre) ⭐ 1,533 | 🐛 26 | 🌐 Python | 📅 2026-08-03 - Sceptre is a tool to drive AWS CloudFormation as part of a CI/CD pipeline by using Hooks
* [Weave GitOps OSS](https://github.com/weaveworks/weave-gitops) ⭐ 1,128 | 🐛 162 | 🌐 MDX | 📅 2026-09-03 - Weave GitOps is a simple open source developer platform for people who want cloud native applications, without needing Kubernetes expertise.
* [Helm Operator](https://github.com/fluxcd/helm-operator) ⚠️ Archived - Automates Helm Chart releases in a GitOps manner
* [Proxmox-GitOps](https://github.com/stevius10/Proxmox-GitOps) ⭐ 580 | 🐛 0 | 🌐 Ruby | 📅 2026-08-30 - Self-contained GitOps framework for LXC-based container automation on Proxmox VE.
* [Gimlet](https://github.com/gimlet-io/gimlet) ⚠️ Archived - The Flux-based Internal Developer Platform
* [Autoapply](https://github.com/autoapply/autoapply) ⭐ 159 | 🐛 12 | 🌐 JavaScript | 📅 2025-11-14 - Automatically apply changes from a Git repository to a Kubernetes cluster
* [Faros](https://github.com/pusher/faros) ⚠️ Archived - CRD based GitOps controller
* [Grant.rs](https://github.com/duyet/grant.rs) ⭐ 37 | 🐛 15 | 🌐 Rust | 📅 2026-07-21 - Manage Redshift/Postgres privileges in GitOps style
* [argocd-backup-s3](https://github.com/oguzhan-yilmaz/argocd-backup-s3/) ⭐ 16 | 🐛 0 | 🌐 Shell | 📅 2025-12-14 -  Kubernetes CronJob to backup ArgoCD with `argocd admin export` cmd and upload to S3 compatible storage
* [Atlantis](https://www.runatlantis.io/) - Terraform pull request automation
* [Carvel](https://carvel.dev) — Tool suite for building, packaging, and managing software on Kubernetes in a GitOps way
* [CloudBees Rollout](https://rollout.io/) - Feature Flag as-a-Service that leverages GitOps & Config-as-Code (commercial product from CloudBees)
* [Jenkins X](https://jenkins-x.io/) - a CI/CD platform for Kubernetes that provides pipeline automation, built-in GitOps and preview environments
* [KubeStack](https://www.kubestack.com/) - GitOps framework using Terraform for Cloud Kubernetes distros (AKS, GKE, and EKS) with CI/CD examples for common tools
* [Weave GitOps Enterprise](https://www.weave.works/product/gitops-enterprise/) - Weave GitOps Enterprise is a continuous operations product that makes it easy to deploy and manage Kubernetes clusters and applications at scale in any environment. (commercial product from Weaveworks)
* [Werf](https://werf.io) - GitOps tool with advanced features to build images and deploy them to Kubernetes (integrates with any existing CI system)
* [PipeCD](https://pipecd.dev/) - Continuous Delivery for Declarative Kubernetes, Serverless and Infrastructure Applications

## Ancillary Tools

### Notifications

* [Fluxcloud](https://github.com/topfreegames/fluxcloud) ⭐ 36 | 🐛 6 | 🌐 Go | 📅 2022-05-10 - Slack notifications for Flux without Weave Cloud

### Secrets

* [SOPS](https://github.com/mozilla/sops) ⭐ 23,009 | 🐛 442 | 🌐 Go | 📅 2026-09-02 - Secrets OPerationS
* [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets) ⭐ 9,271 | 🐛 67 | 🌐 Go | 📅 2026-09-03 - One-way encrypted Secrets
* [git-secret](https://github.com/sobolevn/git-secret) ⭐ 4,040 | 🐛 153 | 🌐 Shell | 📅 2026-08-24 - A bash-tool to store your private data inside a git repository
* [Kamus](https://github.com/Soluto/kamus) ⚠️ Archived - Zero-trust secret encryption/decryption solution for Kubernetes applications
* [Vault Secrets Operator](https://github.com/ricoberger/vault-secrets-operator) ⭐ 685 | 🐛 18 | 🌐 Go | 📅 2026-09-02 - Sync secrets from Vault with Kubernetes
* [argocd-vault-plugin](https://argocd-vault-plugin.readthedocs.io/en/stable/) - An ArgoCD plugin to retrieve secrets from Vault and inject them into Kubernetes resources

## Tutorials

* [Managing Helm releases the GitOps way](https://github.com/fluxcd/flux2-kustomize-helm-example) ⭐ 1,297 | 🐛 0 | 🌐 Shell | 📅 2026-07-08 - Flux and Helm Operator tutorial
* [Automating Istio canary deployments with GitOps](https://github.com/stefanprodan/gitops-istio) ⭐ 670 | 🐛 3 | 📅 2026-05-19 - Progressive Delivery tutorial with Flagger, Flux, Helm Operator and Istio
* [Managing a multi-tenant cluster with GitOps](https://github.com/fluxcd/flux2-multi-tenancy) ⭐ 604 | 🐛 6 | 📅 2026-05-08 - Flux and Kustomize tutorial
* [GitOps-style continuous delivery with Cloud Build](https://cloud.google.com/kubernetes-engine/docs/tutorials/gitops-cloud-build) - Google Cloud Build tutorial

## Community

* [Kubernetes slack](https://slack.kubernetes.io/) - #gitops channel for discussion of GitOps patterns and tooling
* [CNCF slack](https://slack.cncf.io/) - #flux channel for discussion of GitOps patterns and tooling
* [Weaveworks slack](https://slack.weave.works/) - multiple channels (including #flagger, #wksctl and others) to discuss Weaveworks GitOps products, give feedback, and talk about general approaches

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-03._
