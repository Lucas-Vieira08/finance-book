# 📋 Checklist de Funcionalidades

## RA1 — Utilizar Frameworks CSS para estilização de elementos HTML e criação de layouts responsivos

- [x] **ID 01** — Prototipa interfaces adaptáveis para mobile e desktop. *(Concluído na Entrega 1.)*
- [x] **ID 02** — Implementa layout responsivo com Framework CSS utilizando Flexbox ou Grid. *(Evidenciado pelo uso do Bootstrap e de layout responsivo.)*
- [x] **ID 03** — Implementa layout responsivo com CSS puro utilizando Flexbox ou Grid Layout. *(Evidenciado por Flexbox e Grid em `assets/css`.)*
- [x] **ID 04** — Utiliza componentes prontos de um Framework CSS e componentes JavaScript do framework. *(Evidenciado por componentes Bootstrap e pelo bundle JavaScript.)*
- [x] **ID 05** — Utiliza unidades relativas para criação de layouts fluidos. *(Evidenciado por unidades `rem`, `%`, `vw` e `clamp()`.)*
- [x] **ID 06** — Aplica um Design System consistente. *(Evidenciado por `tokens.css` e `docs/design.md`.)*
- **ID 07 — Não aplicável** — Utiliza Sass/SCSS com variáveis, mixins e funções. *(O projeto utiliza CSS puro, sem Sass.)*
- [x] **ID 08** — Aplica tipografia responsiva ou fluida. *(Evidenciado por `clamp()` em `tokens.css`.)*
- [x] **ID 09** — Utiliza técnicas de responsividade de imagens com CSS. *(Evidenciado por `max-width`, `object-fit` e `aspect-ratio`.)*
- [x] **ID 10** — Otimiza imagens utilizando formatos modernos e carregamento adaptativo. *(Evidenciado por imagens WebP e `srcset`/`sizes`.)*

## RA2 — Realizar tratamento de formulários e aplicar validações customizadas no lado cliente

- [ ] **ID 11** — Implementa validação HTML nativa.
- [ ] **ID 12** — Utiliza expressões regulares (REGEX).
- [ ] **ID 13** — Utiliza elementos de seleção em formulários.
- [ ] **ID 14** — Utiliza Web Storage para persistência local.

## RA3 — Aplicar ferramentas para otimização do processo de desenvolvimento web

- [x] **ID 15** — Configura ambiente com Node.js e NPM.
- [ ] **ID 16** — Utiliza boas práticas de versionamento com Git/GitHub. *(Pendente de publicação no GitHub e criação da tag `entrega-2`.)*
- [ ] **ID 17** — Mantém README.md padronizado.
- [ ] **ID 18** — Organiza os arquivos de forma modular.
- [ ] **ID 19** — Configura linters e formatadores.

## RA4 — Aplicar bibliotecas de funções e componentes em JavaScript

- [ ] **ID 20** — Utiliza jQuery para manipulação do DOM e interatividade.
- [ ] **ID 21** — Integra e configura um plugin jQuery relevante.

## RA5 — Efetuar requisições assíncronas para APIs

- [ ] **ID 22** — Realiza requisições assíncronas para API fake para persistência dos dados.
- [ ] **ID 23** — Realiza requisições assíncronas para API fake para exibição dos dados.
- [ ] **ID 24** — Realiza requisições assíncronas para uma API pública de cotações de ativos,   exibindo os dados e tratando possíveis erros.

---

## 📎 Evidências (Entrega 2)

> Os links públicos serão preenchidos após a publicação no GitHub e a criação da tag `entrega-2`. Até lá, permanecem pendentes. Nenhum link fictício foi inserido.

### ID 01 — Prototipação de interfaces adaptáveis

- **Arquivo e linhas:** `README.md:29-33`; `docs/design.md:1-5`.
- **Evidência:** seção de prototipação com o link do protótipo inicial no Stitch, registrado na Entrega 1.
- **Link público (tag `entrega-2`):** pendente.

### ID 02 — Layout responsivo com Framework CSS

- **Arquivo e linhas:** `index.html:64-65`; `index.html:175-176`.
- **Evidência:** uso do grid responsivo do Bootstrap com classes `row`, `col-lg-6`, `row-cols-1` e `row-cols-md-2`.
- **Link público (tag `entrega-2`):** pendente.

### ID 03 — Layout responsivo com CSS puro

- **Arquivo e linhas:** `assets/css/layout.css:41-46`; `assets/css/layout.css:304-306`; `assets/css/pages.css:47-49`.
- **Evidência:** layout construído com Flexbox (`display: flex`) e Grid (`display: grid`, `grid-template-columns`) em CSS puro.
- **Link público (tag `entrega-2`):** pendente.

### ID 04 — Componentes do Framework CSS e JavaScript

- **Arquivo e linhas:** `index.html:11`; `gastos.html:69`; `gastos.html:159-177`; `gastos.html:183`.
- **Evidência:** inclusão do CSS do Bootstrap, botão com `data-bs-toggle`, modal do Bootstrap e inclusão do bundle JavaScript do framework.
- **Link público (tag `entrega-2`):** pendente.

### ID 05 — Unidades relativas em layouts fluidos

- **Arquivo e linhas:** `assets/css/tokens.css:26-44`; `assets/css/pages.css:5-9`.
- **Evidência:** uso de `rem`, `vw`, `clamp()` e `width: 100%` para espaçamentos, tipografia e imagens fluidas.
- **Link público (tag `entrega-2`):** pendente.

### ID 06 — Design System consistente

- **Arquivo e linhas:** `assets/css/tokens.css:1-44`; `docs/design.md:1-30`.
- **Evidência:** tokens de cores, espaçamento, tipografia e bordas definidos em CSS, acompanhados da documentação do Design System.
- **Link público (tag `entrega-2`):** pendente.

### ID 07 — Sass/SCSS

- **Arquivo e linhas:** não aplicável — não há arquivos `.sass` ou `.scss` no repositório.
- **Evidência:** requisito não aplicável, pois a estilização é feita em CSS puro (`assets/css/*.css`). Não há evidência de uso de Sass.
- **Link público (tag `entrega-2`):** não aplicável.

### ID 08 — Tipografia responsiva ou fluida

- **Arquivo e linhas:** `assets/css/tokens.css:37-44`; `assets/css/pages.css:16-18`.
- **Evidência:** definição de `--fb-font-display: clamp(2rem, 4vw, 3rem)` e uso do token de tipografia no título principal.
- **Link público (tag `entrega-2`):** pendente.

### ID 09 — Responsividade de imagens com CSS

- **Arquivo e linhas:** `assets/css/base.css:58-61`; `assets/css/pages.css:5-10`.
- **Evidência:** imagens com `max-width: 100%`, `height: auto`, `width: 100%`, `aspect-ratio` e `object-fit`.
- **Link público (tag `entrega-2`):** pendente.

### ID 10 — Formatos modernos e carregamento adaptativo

- **Arquivo e linhas:** `index.html:82-90`.
- **Evidência:** imagens em WebP com `srcset` e `sizes` para carregamento adaptativo, além de `width`, `height` e `loading`.
- **Link público (tag `entrega-2`):** pendente.

### ID 15 — Ambiente Node.js e NPM

- **Evidência principal (configuração e dependências):** `package.json:1-32` — registra os metadados do projeto, scripts e dependências.
- **Evidências complementares:**
  - `package-lock.json:86-87` — Bootstrap 5.3.8.
  - `package-lock.json:280` — gh-pages 6.3.0.
  - `package-lock.json:387` — jQuery 4.0.0.
  - `package-lock.json:669` — uuid 14.0.2.
  - `.gitignore:1-2` — exclui `node_modules` e `.env` do versionamento.
- **Evidência de execução:** Node.js e NPM foram instalados e utilizados desde o início do projeto. O vídeo da entrega demonstrará o ambiente pelo terminal com `node -v`, `npm -v` e `npm ls`.
- **Link público (tag `entrega-2`):** pendente.

### ID 16 — Versionamento com Git/GitHub

- **Arquivo e linhas:** `.gitignore:1-2`.
- **Evidência de organização:** `.gitignore` exclui `node_modules` e `.env` do versionamento.
- **Evidência complementar:** histórico Git com o commit `58d55a7` (`feat: implementa estrutura visual da entrega 2`).
- **Pendências:** criação da tag `entrega-2` e publicação/links públicos no GitHub.
- **Link público (tag `entrega-2`):** pendente.
