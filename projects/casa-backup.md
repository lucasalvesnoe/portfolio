# casa-backup — backup com prova de restauração

| | |
|---|---|
| **Setor** | Agentes, infraestrutura e ferramentas |
| **Período** | 2026-08-20 → 2026-09-03 |
| **Commits** | 76 |
| **Linguagens** | Shell 90%, Python 10% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Sistema de backup dos dois Macs para armazenamento em nuvem, com restic sobre rclone — e tratado como problema de operação, não como script de cópia. São 22 executáveis em `bin/`: preparação por máquina, backup separado por criticidade, arquivamento de mídia fora do restic, espelho navegável, instalação dos agentes no launchd, conferência, restauração com listar/procurar/tirar/montar, e um `provar` que testa restauração de verdade em vez de só contar arquivo. A chave de 256 bits é gerada e gravada no Keychain sem ninguém digitar nem colar, e a documentação é explícita sobre a consequência disso — Keychain morre com o Mac, repositório restic sem senha é lixo criptografado. Inclui scanner de segredo próprio em Python, relatório de incidente, registro de lições e runbook de restauração. Também trata a validade do plano de armazenamento como risco com data marcada.

## Composição do repositório

81 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `etc` | 39 | 3164 KB |
| `bin` | 23 | 140 KB |
| `(raiz)` | 15 | 113 KB |
| `migracao` | 4 | 22 KB |

---

[← voltar ao índice](../README.md)
