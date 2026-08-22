**# Architecture - FinanceBook**

**## 1. Visão Geral**

O **FinanceBook — Livro Financeiro** será desenvolvido como uma aplicação web responsiva para organização das finanças pessoais e acompanhamento do mercado financeiro.

A aplicação utilizará **HTML5, CSS3, Bootstrap, Sass, JavaScript e jQuery**, além do **JSON Server** para persistência dos dados e uma API pública para informações financeiras.

**---**

**## 2. Estrutura do Projeto**

A aplicação será organizada de forma modular, separando páginas, estilos, scripts, dados e arquivos de documentação.

- **\*\*pages:\*\*** páginas de Gastos, Investimentos e Mercado.
- **\*\*css:\*\*** arquivos de estilização.
- **\*\*js:\*\*** scripts e funcionalidades.
- **\*\*data:\*\*** arquivo utilizado pelo JSON Server.
- **\*\*docs:\*\*** documentação do projeto.

**---**

**## 3. Modelo de Dados**

O **JSON Server** será utilizado para armazenar os principais dados da aplicação.

As principais entidades serão:

- **\*\*Usuário:\*\*** dados básicos do usuário.
- **\*\*Gasto:\*\*** descrição, valor, categoria e data.
- **\*\*Investimento:\*\*** ativo, tipo, quantidade, valor e data.

**---**

**## 4. Comunicação**

O sistema realizará requisições assíncronas utilizando **JavaScript/jQuery**.

- **\*\*JSON Server:\*\*** responsável pelo armazenamento e gerenciamento dos dados.
- **\*\*API Pública:\*\*** responsável pelo fornecimento de informações do mercado financeiro.

**---**

**## 5. Tecnologias**

- **\*\*HTML5:\*\*** estrutura das páginas.

- **\*\*Bootstrap:\*\*** criação de layouts responsivos.

- **\*\*CSS3/Sass:\*\*** estilização da aplicação.

- **\*\*JavaScript/jQuery:\*\*** lógica e interatividade.

- **\*\*JSON Server:\*\*** persistência dos dados.

- **\*\*Node.js/NPM:\*\*** gerenciamento do projeto e dependências.

**---**

**## 6. Execução e Versionamento**

O projeto será executado localmente utilizando **Node.js, NPM e JSON Server**.

O código será versionado utilizando **Git** e hospedado no **GitHub**.

As instruções de instalação e execução serão documentadas no arquivo **README.md**.