# Design System — FinanceBook

> **Framework:** Bootstrap 5  
> **Fonte:** Inter (Google Fonts)  
> **Protótipo:** [Stitch] https://stitch.withgoogle.com/projects/18410765180009445588

---

## 1. Cores

| Token | Valor | Uso |
|-------|-------|-----|
| `primary` | `#0F172A` (Navy) | Botões principais, navbar, títulos |
| `secondary` | `#10B981` (Verde) | Receitas, sucesso, metas atingidas |
| `error` | `#EF4444` (Vermelho) | Despesas, erros, alertas críticos |
| `background` | `#F8FAFC` | Fundo das páginas |
| `surface` | `#FFFFFF` | Cards, containers, modais |
| `border` | `#E2E8F0` | Bordas, divisores, inputs |

**Status (Soft):**
- Sucesso: `#ECFDF5` + `#059669`
- Alerta: `#FEF3C7` + `#D97706`
- Erro: `#FEF2F2` + `#DC2626`
- Neutro: `#F1F5F9` + `#475569`

**Justificativa:** Azul escuro transmite confiança; verde e vermelho seguem convenção financeira universal; tons "soft" evitam fadiga visual.

---

## 2. Tipografia

**Fonte:** `Inter` (única família para consistência)

| Estilo | Tamanho | Peso | Uso |
|--------|---------|------|-----|
| `display` | 48px | 700 | Saldo em destaque |
| `h1` | 32px | 600 | Títulos principais |
| `h2` | 24px | 600 | Subtítulos |
| `body-md` | 14px | 400 | Corpo de texto, tabelas |
| `label-sm` | 12px | 600 | Labels, headers, chips |
| `numeric-data` | 14px | 500 | **Valores financeiros** (+ `tabular-nums`) |

---

## 3. Componentes

### Botões
| Tipo | Cor | Uso |
|------|-----|-----|
| Primary | `#0F172A` | Ações principais (Salvar, Nova Transação) |
| Secondary | `#FFFFFF` + borda `#E2E8F0` | Cancelar, Voltar |
| Success | `#10B981` | Confirmações positivas |
| Danger | `#EF4444` | Excluir, ações irreversíveis |

### Cards
- Background: `#FFFFFF`
- Borda: `1px solid #E2E8F0`
- Raio: `8px`
- Sombra: suave (`0px 1px 3px rgba(0,0,0,0.05)`)

### Inputs
- Borda default: `1px solid #E2E8F0`
- Borda focus: `1px solid #0F172A` + ring `2px #E2E8F0`
- Borda error: `1px solid #EF4444`
- Label: sempre acima (`label-sm`)

### Tabelas
- Header: `#F8FAFC` + `label-sm`
- Row hover: `#F8FAFC`
- Colunas numéricas: direita + `tabular-nums`

### Chips
- Estilo: soft (fundo claro + texto escuro)
- Raio: `9999px` (full)
- Texto: `label-sm`

---

## 4. Layout

**Grid:** 12 colunas (desktop), 4 colunas (mobile)  
**Max-width:** `1280px`  
**Spacing base:** 4px (ritmo de 8px para componentes)

**Breakpoints:**
- Mobile: 0–640px (1 coluna, menu hambúrguer)
- Tablet: 641–1024px (2 colunas)
- Desktop: 1025px+ (3–4 colunas, sidebar fixa)

---

## 5. Acessibilidade

- Contraste mínimo: 4.5:1 (texto normal), 3:1 (texto grande)
- Foco visível em todos os elementos interativos
- Área de toque mínima: `44x44px`
- Zoom suportado até 200%
