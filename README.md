# Awesome AI Safety Research

A curated reading list for AI safety, enterprise security and national governance.

Sections follow the learning order. **★ marks the two starting resources in each section.**

## Contents

- [1. Foundations and alignment](#1-foundations-and-alignment)
- [2. Risk assessment](#2-risk-assessment)
- [3. Evaluations and red teaming](#3-evaluations-and-red-teaming)
- [4. Agent security and Zero Trust](#4-agent-security-and-zero-trust)
- [5. Privacy and lifecycle security](#5-privacy-and-lifecycle-security)
- [6. Secure deployment](#6-secure-deployment)
- [7. Monitoring and incident response](#7-monitoring-and-incident-response)
- [8. Human oversight and fairness](#8-human-oversight-and-fairness)
- [9. Governance and assurance](#9-governance-and-assurance)
- [10. National policy and institutions](#10-national-policy-and-institutions)
- [Courses](#courses)
- [Notes](#notes)

## 1. Foundations and alignment

- ★ [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1) (Course) - Transformers, tokenisation, model inference and fine-tuning, with code examples.
- ★ [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155) (Paper, 2022) - The InstructGPT paper: supervised fine-tuning, reward modelling and reinforcement learning from human feedback.
- [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/abs/2305.18290) (Paper, 2023) - Preference optimisation without a separately trained reward model; includes the derivation and experiments.
- [AI Control: Improving Safety Despite Intentional Subversion](https://arxiv.org/abs/2312.06942) (Paper, 2023) - Tests monitoring and auditing protocols against a model attempting to insert backdoors.
- [Alignment faking in large language models](https://arxiv.org/abs/2412.14093) (Paper, 2024) - Experiments on models changing their behaviour when they infer that training is taking place.
- [Mapping the mind of a large language model](https://www.anthropic.com/research/mapping-mind-language-model) (Research explainer, 2024) - Anthropic's introduction to sparse autoencoders, interpretable features and feature interventions.

## 2. Risk assessment

- ★ [International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026) (Report, 2026) - Evidence on frontier capabilities, misuse, loss of control and risk management. Start with the summary.
- ★ [NIST AI RMF 1.0](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) (Framework, 2023) - The Govern, Map, Measure and Manage functions for assessing and managing AI risk.
- [The AI risk repository: A meta-review, database, and taxonomy of risks from artificial intelligence](https://arxiv.org/abs/2408.12622) (Paper, 2024) - A taxonomy compiled from existing AI risk frameworks. Useful for finding gaps in a risk register.
- [Concrete Problems in AI Safety](https://arxiv.org/abs/1606.06565) (Paper, 2016) - Side effects, reward hacking, scalable supervision, safe exploration and distribution shift.

## 3. Evaluations and red teaming

- ★ [International consensus and open questions in AI evaluations](https://www.aisi.gov.uk/blog/international-ai-network-consensus-and-open-questions) (Guidance, 2026) - Evaluation validity, reproducibility, uncertainty, realistic deployment conditions and multilingual testing.
- ★ [Inspect](https://inspect.aisi.org.uk/) (Tool) - UK AISI's evaluation framework: datasets, tasks, solvers, scorers and inspection of execution logs.
- [Holistic Evaluation of Language Models](https://arxiv.org/abs/2211.09110) (Paper, 2022) - HELM: evaluating accuracy, calibration, robustness, fairness and other properties across shared scenarios.
- [AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for LLM Agents](https://arxiv.org/abs/2406.13352) (Paper, 2024) - An environment for testing tool-using agents against indirect prompt injection, alongside ordinary task performance.
- [Project Moonshot](https://github.com/aiverify-foundation/moonshot) (Tool) - AI Verify Foundation toolkit for application benchmarking, adversarial testing and reports.
- [SEA-SafeguardBench: Evaluating AI Safety in SEA Languages and Cultures](https://arxiv.org/abs/2512.05501) (Paper, 2025) - Safety evaluation across Southeast Asian languages, using culturally grounded, human-verified examples.

## 4. Agent security and Zero Trust

- ★ [OWASP Top 10 for Agentic Applications for 2026](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/) (Security guide, 2026) - Agent-specific threats, including misuse of tools and identity, compromised memory and cascading failures.
- ★ [Design Patterns for Securing LLM Agents against Prompt Injections](https://arxiv.org/abs/2506.08837) (Paper, 2025) - Architectural approaches to prompt injection, with explicit security assumptions and utility trade-offs.
- [OWASP Top 10 for LLM Applications](https://genai.owasp.org/llm-top-10/) (Security guide) - Application risks including injection, disclosure, poisoning, supply chains and excessive agency.
- [NIST SP 800-207: Zero Trust Architecture](https://csrc.nist.gov/pubs/sp/800/207/final) (NIST publication, 2020) - Resource access, identity and policy enforcement. A foundation for designing workload and agent permissions.
- [Securing Agentic AI](https://www.csa.gov.sg/resources/publications/securing-agentic-ai-a-discussion-paper/) (Discussion paper, 2025) - Singapore CSA and FAR.AI on agent attack surfaces, responsibilities and unresolved security problems.

## 5. Privacy and lifecycle security

- ★ [NIST AI 100-2 E2025: Adversarial Machine Learning](https://csrc.nist.gov/pubs/ai/100/2/e2025/final) (NIST publication, 2025) - Attack terminology and threat models covering poisoning, evasion, privacy attacks and mitigations.
- ★ [Programming Differential Privacy](https://programming-dp.com/front/) (Open textbook) - Differential privacy through worked examples: sensitivity, noise mechanisms and composition.
- [Extracting Training Data from Large Language Models](https://arxiv.org/abs/2012.07805) (Paper, 2020) - Demonstrates training-data extraction from a language model and studies the conditions that enable it.
- [Deep Learning with Differential Privacy](https://arxiv.org/abs/1607.00133) (Paper, 2016) - Private model training using gradient clipping, noise and privacy accounting.
- [NIST SP 800-218A](https://csrc.nist.gov/pubs/sp/800/218/a/final) (NIST publication, 2024) - Secure development practices for generative AI and foundation models, including lifecycle and supplier responsibilities.
- [European Commission: Data protection explained](https://commission.europa.eu/law/law-topic/data-protection/data-protection-explained_en) (Official overview) - Personal-data rights and organisational obligations, with links to GDPR resources.

## 6. Secure deployment

- ★ [AWS Well-Architected Generative AI Lens](https://docs.aws.amazon.com/wellarchitected/latest/generative-ai-lens/generative-ai-lens.html) (Architecture guide) - AWS guidance for generative AI security, reliability, operations and deployment choices.
- ★ [Baseline Microsoft Foundry Chat Reference Architecture](https://learn.microsoft.com/en-us/azure/architecture/ai-ml/architecture/baseline-microsoft-foundry-chat) (Reference architecture) - Azure production chat architecture covering identity, network isolation, data flow and operations.
- [Kubernetes Security Checklist](https://kubernetes.io/docs/concepts/security/security-checklist/) (Documentation) - Cluster and workload controls: RBAC, secrets, pod security and network policies.
- [Argo CD security overview](https://argo-cd.readthedocs.io/en/stable/operator-manual/security/) (Documentation) - GitOps deployment authority, repository trust, credentials and access controls.
- [Databricks security and compliance](https://docs.databricks.com/aws/en/security/) (Documentation) - Identity, networking, data access and governance. This link covers the AWS edition.
- [Open WebUI security](https://docs.openwebui.com/security/) (Documentation) - Authentication, permissions, deployment assumptions and security considerations for extensions.

## 7. Monitoring and incident response

- ★ [NIST SP 800-61 Rev. 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final) (NIST publication, 2025) - Incident preparation, detection, response and recovery within an organisation.
- ★ [AgentSpec: Customizable Runtime Enforcement for Safe and Reliable LLM Agents](https://arxiv.org/abs/2503.18666) (Paper, 2025) - A language for defining runtime triggers, conditions and enforcement rules for agents.
- [OpenTelemetry GenAI semantic conventions](https://github.com/open-telemetry/semantic-conventions-genai) (Documentation) - The current repository for GenAI traces, metrics and events, including model and tool calls.
- [Google SRE: Monitoring Distributed Systems](https://sre.google/sre-book/monitoring-distributed-systems/) (Book chapter) - Monitoring signals, alert design and operational diagnosis for distributed services.
- [AIR: Improving Agent Safety through Incident Response](https://arxiv.org/abs/2602.11749) (Paper, 2026) - Integrates incident detection, containment, recovery and new guardrail rules into an agent execution loop.

## 8. Human oversight and fairness

- ★ [To Trust or to Think: Cognitive Forcing Functions Can Reduce Overreliance on AI in AI-assisted Decision-making](https://arxiv.org/abs/2102.09692) (Paper, 2021) - Tests interventions that reduce overreliance on AI, including their usability costs and uneven effects.
- ★ [Closing the AI Accountability Gap: Defining an End-to-End Framework for Internal Algorithmic Auditing](https://arxiv.org/abs/2001.00973) (Paper, 2020) - An internal auditing process spanning development, deployment and organisational accountability.
- [Model Cards for Model Reporting](https://arxiv.org/abs/1810.03993) (Paper, 2018) - A documentation format for intended uses, evaluation conditions, subgroup results and model limitations.
- [Fairness and Machine Learning](https://fairmlbook.org/) (Open textbook) - Fairness definitions, their mathematical tensions and their relationship to social decisions.
- [Fairness and Abstraction in Sociotechnical Systems](https://www.microsoft.com/en-us/research/publication/fairness-and-abstraction-in-sociotechnical-systems/) (Paper, 2019) - How technical abstractions can omit the people, institutions and incentives that determine fairness.

## 9. Governance and assurance

- ★ [NIST Generative AI Profile](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf) (NIST publication, 2024) - Generative AI risks and suggested actions, extending the AI Risk Management Framework.
- ★ [Safety Cases: How to Justify the Safety of Advanced AI Systems](https://arxiv.org/abs/2403.10462) (Paper, 2024) - Structured arguments and evidence for advanced-AI safety, with a focus on catastrophic risk.
- [ISO/IEC 42001:2023](https://www.iso.org/standard/42001) (Standard, 2023) - Requirements for an organisational AI management system. Free overview; the full standard is paid.
- [European Commission: AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) (Official overview) - Risk categories, provider and deployer responsibilities, general-purpose AI and implementation resources.
- [GovTech Agentic Risk & Capability Framework](https://govtech-responsibleai.github.io/agentic-risk-capability-framework/) (Framework) - Maps agent components and capabilities to risks and technical controls.

## 10. National policy and institutions

- ★ [OECD AI Principles](https://oecd.ai/en/ai-principles) (Intergovernmental principles) - Human rights, transparency, robustness, accountability and recommendations for national AI policy.
- ★ [The 2026 Singapore Consensus on Global AI Safety Research Priorities](https://arxiv.org/abs/2608.14611) (Research agenda, 2026) - Updated research priorities covering autonomous agents, technical safety and societal resilience.
- [UNESCO Recommendation on the Ethics of Artificial Intelligence](https://www.unesco.org/en/artificial-intelligence/recommendation-ethics) (Recommendation, 2021) - Human rights, inclusion and implementation of AI ethics in public policy.
- [Frontier AI Regulation: Managing Emerging Risks to Public Safety](https://arxiv.org/abs/2307.03718) (Policy paper, 2023) - Proposals for standards, reporting, oversight and enforcement for frontier AI developers.
- [International Institutions for Advanced AI](https://arxiv.org/abs/2307.04699) (Policy paper, 2023) - Institutional options for international scientific assessment, standards, access and safety research.

## Courses

- [BlueDot: Technical AI Safety](https://bluedot.org/courses/technical-ai-safety) (Course) - Guided study of alignment, interpretability, evaluations, control and oversight. Free; live cohorts require an application.
- [BlueDot: Frontier AI Governance](https://bluedot.org/courses/ai-governance) (Course) - Frontier AI policy, institutional choices and briefing exercises. Free; live cohorts require an application.
- [ARENA curriculum](https://www.arena.education/curriculum) (Practical curriculum) - Coding exercises in AI safety, interpretability and reinforcement learning. Materials are available for independent study.
