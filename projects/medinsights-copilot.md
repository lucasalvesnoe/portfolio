# Copiloto clínico na Rede Bem Estar

| | |
|---|---|
| **Cliente** | Rede Bem Estar |
| **Setor** | Saúde |
| **Período** | 2026-06-06 → 2026-09-22 |
| **Commits** | 22 |
| **Linguagens** | TypeScript 99%, HTML 1% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Extensão Chrome em Manifest V3 que injeta o copiloto clínico dentro do prontuário eletrônico da Rede Bem Estar, sem que a operadora do PEP precise integrar nada. O content script lê o atendimento aberto na tela, manda para o backend RAG do PACK e devolve uma análise de aderência ao protocolo. O detalhe de produto que define o projeto é o gate: o botão "Registrar" fica bloqueado até o médico revisar as condutas sugeridas — a IA não escreve sozinha no prontuário. O motor opera em três modos: pergunta e resposta, geração de evolução, e gap-analysis da evolução escrita contra o PACK. React 19 + TypeScript + Vite com `@crxjs/vite-plugin`, e dois alvos de build — o CRX para o Chrome e uma simulação do PEP que roda sem o Chrome, para validar a interface sem depender do ambiente do cliente.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@vitejs/plugin-react · react · react-dom
```

---

[← voltar ao índice](../README.md)
