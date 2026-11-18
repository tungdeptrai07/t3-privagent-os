# T3 GuardAgent OS — Privacy-Preserving Smart Verifiable Credentials & Attested AI Compliance Copilot

**Grant Submission:** Terminal 3 Build+Scale Agent Micro Grant (DoraHacks)  
**Core SDK Stack:** `@terminal3/t3n-sdk` (TEE Attestation & SIWE ADK) + `@terminal3/ecdsa_vc` (W3C `did:ethr` & `EcdsaSecp256k1Signature2019` Smart VCs)

---

## 1. Executive Summary
Institutional DeFi, Real-World Assets (RWAs), and enterprise AI agents face a severe compliance paradox: protocols must enforce strict KYC/AML and investor accreditation rules, yet feeding raw Personal Identifiable Information (PII) into AI models or public blockchains violates data privacy regulations.

**T3 GuardAgent OS** solves this using Terminal 3's decentralized identity and confidential computing stack:
1. **Encrypted Regulatory Vaults (`@terminal3/ecdsa_vc`)**: Raw user identity data (legal name, passport, exact net worth) is encrypted inside a Regulatory Vault. Users receive a W3C-compliant **Smart Verifiable Credential** signed with `EcdsaSecp256k1Signature2019`.
2. **Selective Disclosure & Zero-Knowledge Predicates (`T3 Verify`)**: Users generate portable Verifiable Presentations disclosing only boolean claims (`isOver18: true`, `isAccreditedInvestor: true`, `amlSanctionsCleared: true`) with **0% raw PII leakage**.
3. **Attested AI Compliance Copilot (`@terminal3/t3n-sdk`)**: An autonomous AI agent running inside an attested Trusted Execution Environment (TEE) verifies the user's cryptographic presentation before executing institutional RWA allocations.
4. **Built-In Traction & Telemetry Engine (80% Grant Metric)**: Real-time analytics tracking Unique Active DIDs onboarded, Smart VCs issued, ZK presentations verified, and T3 Platform Credits consumed.

---

## 2. Quick Start
```bash
python -m http.server 8082 --directory web
```
Open `http://localhost:8082` to test the full interactive suite.
