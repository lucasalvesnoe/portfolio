# Cariacica — integração dos sistemas de saúde

| | |
|---|---|
| **Cliente** | Prefeitura Municipal de Cariacica / SEMUS |
| **Setor** | Setor público |
| **Período** | 2026-06-19 → 2026-07-01 |
| **Commits** | 15 |
| **Linguagens** | HTML 63%, JavaScript 20%, CSS 17% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Arquitetura de integração para os sistemas de saúde da Prefeitura de Cariacica (SEMUS), dentro da iniciativa Cariacica Digital. O problema levantado no AS-IS: o Minha Saúde, onde o cidadão agenda, e o CELK, onde a consulta é executada, não se falam — um operador redigita o agendamento à mão, sem rastreabilidade, e o cancelamento por SMS libera a vaga no CELK mas não a devolve ao Minha Saúde, gerando vaga ociosa. O desenho proposto é uma camada de mediação (anti-corruption layer + orquestração de APIs) que não toca no core dos legados: leitura do Minha Saúde pela API REST que ele já expõe, com resolver de De-Para UUID→CNES, e escrita no CELK por uma API de ingestão nova. Inclui orquestrador com saga, retry e idempotência, barramento de eventos, reconciliador de vagas, MDM com golden record do cidadão e um serviço de IA de consulta em linguagem natural, read-only e auditado. Dimensionado para ~30 mil consultas/mês.

---

[← voltar ao índice](../README.md)
