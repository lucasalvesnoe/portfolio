# KPI Gestão — controle financeiro e conciliação bancária

| | |
|---|---|
| **Cliente** | BPO financeiro |
| **Setor** | Financeiro, jurídico e conformidade |
| **Arquivos de código** | 177 |
| **Linhas de código** | 53.920 |
| **Extensões** | `.tsx` ×136, `.ts` ×25, `.sql` ×10, `.js` ×3, `.css` ×2 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

Sistema de controle financeiro empresarial com conciliação bancária — o projeto de maior volume de reescrita do acervo, com cerca de 54 mil linhas em 177 arquivos escritos à mão. A linhagem está registrada nos nomes das pastas: nasceu como GranaZap, de finanças pessoais, virou KPI Gestão empresarial e chegou à versão com conciliação sobre open banking. Faz importação de extrato em CSV, XLSX, PDF e imagem, categorização automática das transações por regra sobre a descrição, conciliação contra o que já está lançado, lançamento futuro e parcelado, DRE mensal, relatórios e gestão multiusuário com marca configurável por cliente. React + TypeScript + Tailwind sobre Supabase, com servidor próprio para a integração Pluggy de open banking, migrations SQL versionadas (a de setup completo tem 2.271 linhas) e deploy em Netlify. As telas mais pesadas — lançamentos futuros, relatórios e gestão de usuário — passam de 1.800 linhas cada.

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
class-variance-authority · clsx · cmdk · date-fns · embla-carousel-react · input-otp · jspdf
· jspdf-autotable · lucide-react · next-themes · react · react-day-picker · react-dom ·
react-hook-form · react-icons · react-pluggy-connect · react-resizable-panels · react-
router-dom · recharts · sonner · tailwind-merge · tailwindcss-animate · vaul · xlsx · zod
```

## Estrutura

```
migrations/
public/
server/
src/
supabase/
```

---

[← voltar ao índice](../README.md)
