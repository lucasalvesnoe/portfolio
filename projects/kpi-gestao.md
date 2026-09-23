# KPI Engine — gestão financeira multiloja para rede de restaurantes

| | |
|---|---|
| **Cliente** | Franqueadora de restaurantes — rede multiunidade |
| **Setor** | Financeiro, jurídico e conformidade |
| **Arquivos de código** | 261 |
| **Linhas de código** | 69.528 |
| **Extensões** | `.tsx` ×138, `.js` ×46, `.ts` ×40, `.sql` ×33, `.css` ×2 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

Sistema de gestão financeira multiloja construído para a operação de uma franqueadora de restaurantes, e o trabalho mais maduro do acervo — 261 arquivos e 69.528 linhas na versão canônica, dentro de um acervo de 5,8 GB com mais de trinta versões nomeadas. O que o torna um sistema de food service e não um controle financeiro genérico é o modelo de análise: as despesas são classificadas em grupos econômicos — custo fixo, custo variável, **CMV**, impostos e investimento — que são exatamente as linhas da DRE de uma operação de restaurante, e é sobre eles que a tela de análise econômica e a DRE se montam. O multiloja não é filtro de tela: são quatro migrations dedicadas (schema, políticas RLS, massa de teste e a função que resolve quais lojas cada usuário enxerga), com `loja_id` atravessando 71 pontos do código — cada unidade da rede tem o dado isolado no banco, e o franqueado só vê a própria. São 22 telas: dashboard, DRE, análise econômica, vendas, receitas, despesas, transações, lançamentos futuros com parcelamento e recebíveis, conciliação, conciliação por calendário, categorias, grupos, metas, planos, configurações, mais as áreas de autenticação e administração. A entrada de extrato cobre OFX e integração direta — **Sicoob** por API com certificado mTLS, **PagBank**, **RecargaPay** e **Pluggy** para open banking — com categorização automática por regra sobre a descrição e conciliação contra o que já está lançado. Tem white label por cliente, sistema de planos, controle de acesso por status do usuário (ativo, inativo, bloqueado) e Turnstile no login. React + TypeScript + Tailwind sobre Supabase, com servidor próprio, 34 migrations versionadas — incluindo um hotfix de RLS que fechou o isolamento entre lojas — e deploy em Netlify. A evolução é longa e está registrada em nome de pasta, não em histórico de git: V.013 em junho de 2025, GranaZap, KPI Engine, KPI Engine Multiloja, KPI Gestão, a versão inicial da rede em agosto, e a atual com conciliação sobre open banking. As pastas de versão validada descrevem o estado em que cada uma foi congelada — *"tudo ok, sicoob 99%, último antes do pagbank"* é um nome de pasta real, e funciona como changelog.

## Dependências declaradas

Extraídas do `package.json` / `requirements.txt` do projeto.

```
@hookform/resolvers · @radix-ui/react-accordion · @radix-ui/react-alert-dialog · @radix-
ui/react-aspect-ratio · @radix-ui/react-avatar · @radix-ui/react-checkbox · @radix-ui/react-
collapsible · @radix-ui/react-context-menu · @radix-ui/react-dialog · @radix-ui/react-
dropdown-menu · @radix-ui/react-hover-card · @radix-ui/react-label · @radix-ui/react-menubar
· @radix-ui/react-navigation-menu · @radix-ui/react-popover · @radix-ui/react-progress ·
@radix-ui/react-radio-group · @radix-ui/react-scroll-area · @radix-ui/react-select · @radix-
ui/react-separator · @radix-ui/react-slider · @radix-ui/react-slot · @radix-ui/react-switch
· @radix-ui/react-tabs · @radix-ui/react-toast · @radix-ui/react-toggle · @radix-ui/react-
toggle-group · @radix-ui/react-tooltip · @supabase/supabase-js · @tanstack/react-query ·
@types/pdf-parse · class-variance-authority · clsx · cmdk · date-fns · embla-carousel-react
· i18next · i18next-browser-languagedetector · input-otp · jspdf · jspdf-autotable · lucide-
react · next-themes · node-fetch · pdfjs-dist · react · react-day-picker · react-dom ·
react-hook-form · react-i18next · react-icons · react-resizable-panels · react-router-dom ·
recharts · sonner · tailwind-merge · tailwindcss-animate · vaul · xlsx · zod · express ·
cors · dotenv · axios
```

## Estrutura

```
certs/
migrations/
public/
src/
supabase/
```

---

[← voltar ao índice](../README.md)
