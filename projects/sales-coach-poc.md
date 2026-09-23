# Sales Coach — coaching de venda em tempo real

| | |
|---|---|
| **Cliente** | Rede de varejo de calçados |
| **Setor** | Varejo |
| **Arquivos de código** | 15 |
| **Linhas de código** | 3.494 |
| **Extensões** | `.jsx` ×6, `.js` ×5, `.html` ×3, `.css` ×1 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

Coach de vendas que roda durante o atendimento presencial, feito para uma rede de lojas físicas de calçados. Captura o áudio do microfone no navegador, transcreve a conversa entre vendedor e cliente ao vivo pela Web Speech API em pt-BR, e manda o texto ao Claude para gerar orientação de venda enquanto a conversa ainda está acontecendo — não um relatório depois. A tela é dividida: transcrição à esquerda, insights à direita. React + Vite + Tailwind.

## Dependências declaradas

Extraídas do `package.json` / `requirements.txt` do projeto.

```
react · react-dom
```

## Estrutura

```
docs/
public/
src/
```

---

[← voltar ao índice](../README.md)
