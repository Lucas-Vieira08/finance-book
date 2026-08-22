````markdown
**# Architecture - FinanceBook**

**## 1. Visão Geral**

O **FinanceBook** será desenvolvido como uma aplicação web responsiva para organização financeira pessoal e acompanhamento do mercado financeiro.

A aplicação utilizará **HTML5, CSS3, Bootstrap, Sass, JavaScript e jQuery**, além do **JSON Server** para persistência dos dados e uma API pública para informações financeiras.

**---**

**## 2. Estrutura do Projeto**

```text
FinanceBook/
│
├── index.html
├── pages/
│   ├── gastos.html
│   ├── investimentos.html
│   └── mercado.html
│
├── css/
│   └── style.scss
├── js/
│   ├── main.js
│   ├── gastos.js
│   ├── investimentos.js
│   └── mercado.js
│
├── data/
│   └── db.json
│
└── docs/
````

**---**

**## 3. Modelo de Dados**

O **JSON Server** será utilizado para armazenar os dados principais da aplicação.

As principais entidades serão:

* **Usuário:** dados básicos do usuário.
* **Gasto:** descrição, valor, categoria e data.
* **Investimento:** ativo, tipo, quantidade, valor e data.

**---**

**## 4. Comunicação**

O sistema utilizará requisições assíncronas para comunicação entre o Frontend e os serviços externos.

* **JSON Server:** armazenamento e gerenciamento dos gastos e investimentos.
* **API Pública:** consulta de informações do mercado financeiro.

**---**

**## 5. Tecnologias**

* **HTML5:** estrutura das páginas.
* **Bootstrap:** layout responsivo.
* **Sass/CSS3:** estilização.
* **JavaScript/jQuery:** lógica e interatividade.
* **JSON Server:** persistência dos dados.
* **Node.js/NPM:** gerenciamento do projeto.

**---**

**## 6. Execução e Versionamento**

O projeto será executado localmente utilizando **Node.js, NPM e JSON Server**.

O código será versionado utilizando **Git** e hospedado no **GitHub**.
