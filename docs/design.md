# Design System — FinanceBook

> **Framework:** Bootstrap 5.3.8  
> **Fonte:** Inter (Google Fonts)  
> **Protótipo:** [Stitch](https://stitch.withgoogle.com/projects/18410765180009445588)

---

## 1. Cores

| Token | Valor | Uso |
|-------|-------|-----|
| `primary` | `#0F172A` (Navy) | Botões principais, navbar, títulos |
| `secondary` | `#10B981` (Verde) | Valores positivos, sucesso, variações favoráveis |
| `error` | `#EF4444` (Vermelho) | Gastos, erros, alertas críticos |
| `background` | `#F8FAFC` | Fundo das páginas |
| `surface` | `#FFFFFF` | Cards, containers, modais |
| `border` | `#E2E8F0` | Bordas, divisores, inputs |

**Status (Soft):**

- Sucesso: `#ECFDF5` + `#059669`
- Alerta: `#FEF3C7` + `#D97706`
- Erro: `#FEF2F2` + `#DC2626`
- Neutro: `#F1F5F9` + `#475569`

**Justificativa:** Azul escuro transmite confiança; verde e vermelho seguem convenções visuais do contexto financeiro; tons suaves reduzem o impacto visual.

---

## 2. Tipografia

**Fonte:** `Inter` (única família para consistência)

| Estilo | Tamanho | Peso | Uso |
|--------|---------|------|-----|
| `display` | `clamp(2rem, 4vw, 3rem)` | 700 | Saldos e valores em destaque |
| `h1` | `2rem` | 600 | Títulos principais |
| `h2` | `1.5rem` | 600 | Subtítulos |
| `body-md` | `0.875rem` | 400 | Corpo de texto e tabelas |
| `label-sm` | `0.75rem` | 600 | Labels, headers e chips |
| `numeric-data` | `0.875rem` | 500 | Valores financeiros + `tabular-nums` |

---

## 3. Componentes

### Botões

| Tipo | Cor | Uso |
|------|-----|-----|
| Primary | `#0F172A` | Salvar, Novo gasto, Novo investimento |
| Secondary | `#FFFFFF` + `#E2E8F0` | Cancelar, Voltar |
| Success | `#10B981` | Confirmações positivas |
| Danger | `#EF4444` | Excluir e ações irreversíveis |

### Cards

- Background: `#FFFFFF`
- Borda: `1px solid #E2E8F0`
- Raio: `8px`
- Sombra: `0px 1px 3px rgba(0,0,0,0.05)`
- Usados para saldos, gastos, investimentos e cotações

### Inputs

- Borda default: `1px solid #E2E8F0`
- Borda focus: `1px solid #0F172A`
- Borda error: `1px solid #EF4444`
- Label sempre acima
- Utilizar validação nativa do HTML5

### Tabelas

- Header: `#F8FAFC` + `label-sm`
- Row hover: `#F8FAFC`
- Colunas numéricas: alinhadas à direita + `tabular-nums`
- Tabelas devem ser responsivas

### Chips

- Fundo claro + texto escuro
- Raio: `9999px`
- Texto: `label-sm`
- Usados principalmente para categorias e classificações

### Feedback

- Sucesso: operação concluída
- Erro: operação ou requisição não concluída
- Alerta: atenção necessária
- Neutro: informações gerais
- Utilizar componentes de alerta do Bootstrap

### Filtros

- Filtro por período, categoria e tipo quando aplicável
- Utilizar `select`, `input` e componentes do Bootstrap

### Estado vazio

- Mensagem objetiva
- Orientação para a próxima ação
- Botão relacionado à ação quando aplicável

### Cotações

- Card com ativo, cotação atual e variação
- Dados obtidos através da API `brapi.dev`
- Exibir feedback caso a API esteja indisponível

---

## 4. Layout e Responsividade

**Framework:** Bootstrap 5.3.8

- Grid baseado no sistema de 12 colunas do Bootstrap
- Layout responsivo com Flexbox e Grid
- `max-width`: `1280px`
- Espaçamentos baseados em múltiplos de `4px`
- Utilizar unidades relativas (`rem`, `%`, `vw`, `vh`) sempre que possível

**Breakpoints:**

- Mobile: `< 768px`
- Tablet: `768px – 991px`
- Desktop: `≥ 992px`

**Navegação:**

- Desktop: navbar completa
- Mobile: menu hambúrguer
- Conteúdo reorganizado conforme o tamanho da tela

---

## 5. Imagens

- `max-width: 100%`
- `height: auto`
- Preferência por formatos `WebP` ou `AVIF`
- Utilizar carregamento `lazy` quando aplicável
- Imagens devem se adaptar ao espaço disponível

---

## 6. Acessibilidade

- Contraste mínimo: `4.5:1` para texto normal e `3:1` para texto grande
- Foco visível em elementos interativos
- Área de toque mínima: `44x44px`
- Suporte a zoom de até `200%`
- Utilizar HTML semântico e atributos apropriados