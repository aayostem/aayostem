# Ayobami Adejumo — Platform Engineering · SOC2 · FinOps

> *I build the infrastructure that lets startups ship fast without breaking trust.*

---

## What I do

Most seed-to-Series A companies hit the same wall: they've moved fast, won customers, raised money — and now those enterprise buyers are asking for SOC2 Type II, HIPAA evidence, PCI-DSS controls, or a Kubernetes architecture that doesn't collapse under load.

That's where I come in.

I'm a **Senior Platform Engineer and FinOps specialist** who sits at the intersection of three disciplines that most engineers treat as separate jobs: **cloud infrastructure**, **security compliance**, and **cloud cost engineering**. My thesis is simple — infrastructure built for speed is not built for trust, and you can't bolt trust on after the fact.

I work with **EU and US companies at the seed-to-Series A inflection point** through my consultancy [Cloudfrugal](https://cloudfrugal.com), and I'm selectively available for **founding engineer engagements** where the infrastructure layer is a strategic bet, not an afterthought.

---

## Flagship: Financial RAG Agent

**[github.com/aayostem/financial-rag-agent](https://github.com/aayostem/financial-rag-agent)**

A production-grade multi-agent financial intelligence system built end-to-end — from SEC EDGAR ingestion to LLM-powered Q&A — across 14 architectural layers with 106 passing tests.

**What makes it production-grade, not a demo:**

| Layer | Technology |
|---|---|
| Vector search | PostgreSQL + pgvector |
| Caching | Redis |
| LLM compatibility | OpenAI · Groq · Azure (swappable) |
| API | FastAPI |
| Migrations | Alembic |
| Observability | Prometheus + Grafana |
| Security scanning | Trivy · gitleaks · pip-audit |
| CI/CD | GitHub Actions (multi-stage) |
| Containers | Docker multi-stage builds |
| Orchestration | EKS on Terragrunt-wrapped Terraform |
| Networking | Cilium CNI |
| Secrets | HCP Vault + Agent Injector |
| Autoscaling | Karpenter |
| Service mesh | Istio |
| GitOps | ArgoCD ApplicationSets |

The full 7-phase Kubernetes production deployment spans 6 Terragrunt modules across 3 environments. The staging cluster (`financial-rag-staging-cluster`, us-east-1) reached Helm revision 7 with the complete LGTM observability stack, Falco runtime security, and OPA/Gatekeeper policy enforcement.

**Companion projects in the same mono-repo infrastructure:**

- **Drift Sentinel** — ML model drift detection with automated alerting pipelines
- **RiskOracle** — Quantitative risk analytics for financial institutions

All three share a Transit Gateway-compatible CIDR allocation strategy for future inter-VPC routing.

---

## Technical depth

```
Platform Engineering    EKS · Karpenter · Cilium · Istio · ArgoCD · Helm · Terragrunt/Terraform
Security & Compliance   SOC2 Type II · HIPAA · PCI-DSS · HCP Vault · Falco · OPA/Gatekeeper
FinOps                  Cloud cost attribution · Kubernetes cost-per-workload · Spot/on-demand strategy
Observability           Prometheus · Grafana · Loki · Tempo (LGTM stack) · OpenTelemetry
Post-Quantum Crypto     ML-DSA-65 (FIPS 204) · ML-KEM-768 (FIPS 203) · Hybrid ECDSA/X25519
Data                    PostgreSQL + pgvector · Redis · Alembic · SEC EDGAR ingestion pipelines
Languages               Python · Bash · HCL · YAML · SQL
```

---

## What I've shipped for clients

**Alva (post-quantum transaction identity)** — Designed the full hybrid PQC architecture for a transaction identity startup building on ML-DSA-65 (FIPS 204) + ECDSA for signatures and ML-KEM-768 (FIPS 203) + X25519 for key encapsulation. Produced the 8-week MVP scope, infra cost model (~$224–384/mo), and the founding engineer engagement structure.

**LexClaro** — Identified three critical compliance gaps (PII scrubbing for GDPR Art.25, customer-managed KMS, document-level audit trail) after reviewing their AWS architecture. Proposed a targeted Gap Sprint to remediate before enterprise client onboarding.

---

## How I engage

**For sub-10 companies** (pre-product-market-fit, pre-SOC2):
- On-Call CTO · Pre-Launch Audit · Gap Sprint · First Hire Infrastructure Review

**For 10+ companies** (post-Series A, scaling platform):
- FinOps Principal · Platform Engineering Lead · SOC2 Type II Program Lead · Fractional CTO

**Geography:** Lagos, Nigeria — serving EU and US clients via Deel / Payoneer / Remote.com

---

## Writing & teaching

I write about the intersection of platform engineering, SOC2, and FinOps as one unified discipline — not three separate jobs.

- **dev.to/aayostem** — Long-form technical breakdowns
- **hashnode/aayostem** — technical breakdowns
- **Medium/@aayostem** — Architecture patterns for seed-to-Series A infra

Five-course portfolio in development:
1. Financial RAG Agent (26h) — Production ML system on EKS
2. SOC2 Type II Engineering (20h) — Evidence pipelines, not paperwork
3. FinOps + IDP Engineering (20h) — Cost attribution at Kubernetes granularity
4. ML Drift Detection: Drift Sentinel (16h)
5. Enterprise ML Risk: RiskOracle (18h)

---

## Contact

**Consulting:** Cloudfrugal
**Email:** aayo.software@gmail.com
**Available for:** Founding engineer roles · Fractional CTO · SOC2 retainers · FinOps audits

> *If your infrastructure can't pass a vendor security questionnaire, you're leaving enterprise revenue on the table. Let's fix that.*
