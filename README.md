# Portfolio — Lucas Noé

Solutions Architect · Generative & Agentic AI

35 systems I have designed and delivered, most of them for clients and closed-source. I work as the architect and product owner: I define the problem, the architecture and the behaviour, and the code is produced through AI-assisted development (Claude Code). Each entry is a case study: what the system solves, the architectural decision that defines it, the stack taken from the project manifests, and metrics from the real history. Client names are omitted for confidentiality. **Read access to the source code can be granted on request, per repository and for a fixed period.**

## Public sector

| Project | Client | What it solves |
|---|---|---|
| **[EducAI — civil servant training portal](projects/educai-portal.md)** | Public sector — civil servant training | A training portal for public servants. |
| **[Intelligent public data platform](projects/plataforma-dados-publicos.md)** | State research and statistics institute | A platform for accessing state public data, built for a state research institute and delivered as a PoC for handoff to the client's Azure team. |
| **[Account holder change via WhatsApp with OCR](projects/whatsapp-ocr-saneamento.md)** | State water and sanitation company | A conversational chatbot that guides the company's customer through the whole process of changing the account holder on a water account over WhatsApp,… |
| **[Municipal healthcare systems integration](projects/integracao-saude-municipal.md)** | Municipal government of a mid-sized municipality | Integration architecture for a municipal government's healthcare systems, as part of the municipality's digital transformation programme. |
| **[Incremental modernisation of a legacy municipal system](projects/modernizacao-legado-municipal.md)** | State capital municipal government | Proof that a production system can be modernised without a big-bang rewrite. |
| **[PDF anonymiser for LGPD](projects/anonimizador-pdf-lgpd.md)** | State-owned urban transport company | An automatic PDF anonymiser for LGPD (Brazil's GDPR) compliance, built for an urban transport company and styled to match the original portal. |
| **[Intelligent automation of outstanding tax debt](projects/divida-ativa-procuradoria.md)** | State attorney general's office | An intelligent automation system for a state attorney general's office, aimed at the bottleneck in legal work on outstanding tax debt (dívida ativa). |
| **[Virtual assistant for pension policyholders](projects/assistente-previdencia.md)** | State pension institute | Prototype of a virtual assistant for the policyholders of a state pension institute, built as a commercial demonstration piece — entirely mocked, and… |

## Healthcare

| Project | Client | What it solves |
|---|---|---|
| **[Clinical copilot for protocol adherence](projects/copiloto-clinico-protocolo.md)** | Clinic network | Manifest V3 Chrome extension that injects the clinical copilot into a clinic network's electronic health record (EHR), without the EHR vendor having to… |
| **[Laboratory management and claim-denial prevention hub](projects/laboratorio-anti-glosa.md)** | Clinical laboratory | A laboratory management system for a clinical laboratory, with an attached anti-glosa hub. |
| **[Clinical inconsistency copilot](projects/copiloto-clinico-inconsistencias.md)** | Clinic using a cloud-based EHR | A clinical copilot for a cloud-based EHR, with a different angle from the protocol-adherence copilot: instead of checking adherence to a protocol, it looks… |
| **[PACK Copilot — clinical RAG that refuses to hallucinate](projects/medinsights-pack-poc.md)** | Medinsights | A clinical copilot with RAG over the PACK Brasil Adulto 2025 (Practical Approach to Care Kit, Porto Alegre version). |
| **[MedInsights — clinical copilot on a hospital information system](projects/copiloto-clinico-his.md)** | Hospital — off-the-shelf hospital management system | A proof of concept of the clinical copilot, demonstrated on top of the interface of an off-the-shelf hospital management system. |

## Transport and logistics

| Project | Client | What it solves |
|---|---|---|
| **[Logistics intelligence platform](projects/inteligencia-logistica.md)** | Logistics operator | A logistics intelligence platform with generative AI for a logistics operator, at version 3.4.0. |
| **[Driver rostering optimisation](projects/escala-motoristas.md)** | Intercity bus operator | Driver and vehicle rostering optimisation engine for an intercity bus operator. |
| **[DIRECTFUEL — external fleet refuelling](projects/abastecimento-frota.md)** | Road transport group | MVP for managing external fleet refuelling, built for a 60-day pilot at a road transport group and presented to the client under the DIRECTFUEL brand. |

## Finance, legal and compliance

| Project | Client | What it solves |
|---|---|---|
| **[KPI Engine — multi-store financial management for a restaurant chain](projects/kpi-gestao.md)** | Restaurant franchisor — multi-unit chain | Multi-store financial management system built for the operation of a restaurant franchisor, and the most mature piece of work in the archive — 261 files and… |
| **[Automated analysis of court-ordered government debts (precatórios)](projects/analise-precatorios.md)** | Judicial credit management firm | A system for automated analysis of court-ordered government debts (precatórios) and legal cases, built on top of Evadocs. |
| **[AI-assisted certificate screening](projects/triagem-certificados.md)** | Cosmetics manufacturer | A screening dashboard that uses AI to read professional training certificates, validate the issuing institution and give the operator a confidence… |
| **[NIST 800-53 — compliance platform](projects/nist-saas-poc.md)** | Information security consultancy | SaaS platform for managing NIST 800-53 compliance, with separate backend and frontend. |
| **[RegulaTech BR — banking regulatory monitoring](projects/monitoramento-regulatorio-bancario.md)** | State development bank | RegulaTech BR is a banking regulation monitoring system for a state development bank, at version 1.1.0. |
| **[Automated bank reconciliation in n8n](projects/n8n-bank-reconciliation.md)** | — | Bank reconciliation automation in n8n, integrated with Supabase — the orchestrated version of the same problem that KPI Gestão solves as an application. |

## Retail

| Project | Client | What it solves |
|---|---|---|
| **[Sales Coach — real-time sales coaching](projects/sales-coach-poc.md)** | Footwear retail chain — 320 stores in Brazil | A sales coach that runs during face-to-face customer service, built for a chain of physical footwear stores. |
| **[Information security quiz kiosk](projects/totem-seguranca-informacao.md)** | State development bank | Quiz and prize-wheel kiosk for a development bank's 1st Information Security Awareness Week — built to run on a free-standing unit in the lobby, with the… |

## Own products and platforms

| Project | Client | What it solves |
|---|---|---|
| **[PubliVeo — video into multichannel content](projects/publiveo.md)** | — | A SaaS platform that turns a recorded video into content ready to publish on the creator's social channels, with no manual editing. |
| **[Real-time collaborative Project Planner](projects/project-planner.md)** | — | Professional project manager with real-time collaboration — the web alternative to MS Project, at version 2.4.0. |
| **[CCA-F Trainer — certification exam prep](projects/cca-f-trainer.md)** | — | A study app for the Claude Certified Architect – Foundations certification. |
| **[ChurchControl — church management](projects/churchcontrol-web.md)** | Church management | Management system for churches, covering the whole administrative cycle rather than just member records. |

## Agents, infrastructure and tooling

| Project | Client | What it solves |
|---|---|---|
| **[AIsquad — a team of agents on top of company context](projects/paperclip.md)** | — | AIsquad is a team of AI agents that works on the company's real context: project folders, email, Teams and the CRM. |
| **[Image generation lab with locked identity](projects/geracao-de-imagem.md)** | — | An image generation lab with consistent identity, running on a GPU rented by the hour. |
| **[VibeTranscript — transcription with speaker separation](projects/vibetranscript.md)** | — | Meeting transcription with speaker separation, editable speaker cards (name, photo and CRUD) and AI analysis. |
| **[casa-backup — backup with proof of restore](projects/casa-backup.md)** | — | A backup system for two Macs to cloud storage, using restic over rclone, and treated as an operations problem rather than a copy script. |
| **[Architecture and pre-sales skills](projects/intelliway-skills.md)** | — | A set of Claude Code skills, versioned and synced across machines — automation of the architecture and pre-sales work itself. |
| **[Escriba — meetings recorded and transcribed on the Mac itself](projects/escriba.md)** | — | Records, transcribes and summarises meetings on the Mac with no bot joining the call, no virtual audio driver and no audio leaving the machine. |
| **[Claudinho — voice interface for Claude Code](projects/voice-claude.md)** | — | Portuguese-language voice interface for Claude Code — speak and the agent runs commands, edits files and executes scripts, without losing any tool along the… |

---

[github.com/lucasalvesnoe](https://github.com/lucasalvesnoe)
