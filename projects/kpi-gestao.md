# KPI Engine — multi-store financial management for a restaurant chain

| | |
|---|---|
| **Client** | Restaurant franchisor — multi-unit chain |
| **Sector** | Finance, legal and compliance |
| **Source code** | not versioned on GitHub — available on request |

## What it is

Multi-store financial management system built for the operation of a restaurant franchisor, and the most mature piece of work in the archive — 261 files and 69,528 lines in the canonical version, within a 5.8 GB archive holding more than thirty named versions. What makes it a food service system rather than generic financial control is the analysis model: expenses are classified into economic groups — fixed cost, variable cost, **COGS**, taxes and investment — which are exactly the lines of a restaurant operation's **P&L**, and the economic analysis screen and the P&L are built on top of them. Multi-store is not a screen filter: it takes four dedicated migrations (schema, RLS policies, test data and the function that resolves which stores each user can see), with `loja_id` running through 71 points in the code — each unit in the chain has its data isolated in the database, and a franchisee sees only their own. There are 22 screens: dashboard, P&L, economic analysis, sales, income, expenses, transactions, future entries with instalments and receivables, reconciliation, calendar reconciliation, categories, groups, targets, plans, settings, plus the authentication and administration areas. Statement intake covers OFX and direct integration — **Sicoob** via API with an mTLS certificate, **PagBank**, **RecargaPay** and **Pluggy** for open banking — with automatic rule-based categorisation on the description and reconciliation against what has already been entered. It has per-client white labelling, a plans system, access control by user status (active, inactive, blocked) and Turnstile on login. React + TypeScript + Tailwind on Supabase, with its own server, 34 versioned migrations — including an RLS hotfix that closed the isolation gap between stores — and deployment on Netlify. The evolution is long and is recorded in folder names, not in git history: V.013 in June 2025, GranaZap, KPI Engine, KPI Engine Multiloja, KPI Gestão, the chain's initial version in August, and the current one with reconciliation over open banking. The validated-version folders describe the state each was frozen in — *"tudo ok, sicoob 99%, último antes do pagbank"* ("all OK, Sicoob 99%, last one before PagBank") is a real folder name, and works as a changelog.

## Stack

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

---

[← back to index](../README.md)
