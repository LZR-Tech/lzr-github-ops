## O que mudou?

<!-- Descreva as mudancas de forma clara e concisa -->

## Por que?

<!-- Qual problema resolve ou qual feature adiciona -->

## Como testar?

- [ ] Passo 1
- [ ] Passo 2
- [ ] Passo 3

## Checklist de Qualidade (Engineering Handbook v2.2)

### Codigo
- [ ] JSDoc em todos os metodos publicos novos/modificados
- [ ] Comentarios explicativos em decisoes nao obvias (trade-offs, workarounds, regras de negocio)
- [ ] `tryCatch()` + `toast.error()` nos hooks (sem `console.error`)
- [ ] `aria-labels` em componentes interativos novos
- [ ] Paginacao em queries de listagem (`.range()` ou `.limit()`)
- [ ] Testes para logica nova (services, hooks, libs)
- [ ] Sem `console.log` ou `debugger`
- [ ] Sem `any` no TypeScript

### Design System (v1.3)
- [ ] Tokens do DS usados (sem cores Tailwind hardcoded: `bg-emerald-600`, `text-blue-500`)
- [ ] Sem prefixo `dark:` (CSS variables mudam automaticamente)
- [ ] Toasts com Lucide icons (sem emojis)
- [ ] Componentes de `@/components/ui/` (sem tags HTML diretas)
- [ ] Placeholders usam `--text-placeholder` (nunca `--text-3` — WCAG AA 4.5:1)
- [ ] Touch targets minimos 44x44px em elementos interativos

### Data Fetching
- [ ] React Query para server data (sem `useState` + `useEffect` para fetch)
- [ ] Query keys registradas em `query-keys.ts`

### Navegacao
- [ ] Botoes de retroceder usam `router.back()` (nunca `router.push('/rota-fixa')`)

### Validacao
- [ ] `npm run build` passa (0 erros)
- [ ] `npm run lint` sem erros novos
- [ ] `npm run typecheck` sem erros
- [ ] Variaveis sensiveis via env vars (nao hardcoded)

## Screenshots (se aplicavel)

<!-- Cole prints se for mudanca visual -->
