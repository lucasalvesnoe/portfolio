# Copiloto clínico no Clínica nas Nuvens

| | |
|---|---|
| **Cliente** | Clínica nas Nuvens |
| **Setor** | Saúde |
| **Período** | 2026-09-08 → 2026-09-23 |
| **Commits** | 15 |
| **Linguagens** | TypeScript 100% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Copiloto clínico para o Clínica nas Nuvens, com um recorte diferente do copiloto da Rede Bem Estar: em vez de checar aderência a protocolo, ele procura o que não fecha no raciocínio. Ao abrir um atendimento, lê o que já foi escrito, busca os atendimentos anteriores do mesmo paciente e lista na barra lateral contradição entre registros, tendência de piora, exame pedido que nunca teve desfecho e conduta sem justificativa. Cada achado carrega o trecho do prontuário que o sustenta e, quando cabe, um botão que escreve a sugestão de volta. A priorização usa a escala de Manchester, com o modelo instruído a emitir nessa ordem e a barra reordenando por garantia: vermelho para conduta de tratamento, laranja para medicação e exames, amarelo para inconsistência de registro, verde para o resto. Os cards são numerados porque ler prioridade só pela cor exige conhecer a escala.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@vitejs/plugin-react · react · react-dom
```

---

[← voltar ao índice](../README.md)
