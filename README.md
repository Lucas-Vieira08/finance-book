# FinanceBook — Livro Financeiro

## 👤 Identificação

**Aluno:** Lucas Vieira  

**Projeto:** FinanceBook — Livro Financeiro  

**Tema:** Organização financeira pessoal

---

## 📖 Descrição do Projeto

O **FinanceBook** é uma aplicação web responsiva desenvolvida para auxiliar na organização e no acompanhamento das finanças pessoais.

A aplicação permitirá que o usuário registre seus **gastos e investimentos**, visualize seus registros e acompanhe um resumo de sua situação financeira.

Na área de investimentos, está prevista a integração com uma **API pública de cotações** para obter informações atualizadas sobre os ativos cadastrados, complementando os dados registrados pelo usuário. Essa integração faz parte da etapa final/funcional e **ainda não está implementada nesta entrega**.

O objetivo é centralizar informações financeiras pessoais em uma única aplicação, facilitando o controle dos gastos e o acompanhamento dos investimentos.

O FinanceBook possui caráter exclusivamente informativo e organizacional. A aplicação não realizará movimentações financeiras reais, pagamentos, transferências ou operações de compra e venda de ativos.

> **Escopo da Entrega 2:** esta entrega contempla a estrutura visual e responsiva da aplicação. As funcionalidades — incluindo lógica JavaScript, persistência de dados e integração com APIs — serão desenvolvidas nas próximas etapas.

---

## 🎨 Prototipação


**Figma/Stitch:** O protótipo inicial foi desenvolvido no Stitch. Refinamentos específicos poderão ser realizados no Figma.\
**Protótipo inicial:** [Stitch](https://stitch.withgoogle.com/projects/18410765180009445588)

---

## 🎨 Design System

**Documento:** [design.md](/docs/design.md)

---

## 🧩 Framework CSS

**Framework:** Bootstrap 5.3.8

---

## 📦 Tecnologias e Dependências

As principais tecnologias do projeto são listadas abaixo. Esta é uma lista das principais tecnologias, não necessariamente todas as dependências do `package.json`.

- HTML5
- CSS puro (CSS3)
- JavaScript ES6+ — lógica da aplicação prevista para a etapa final/funcional
- Bootstrap 5.3.8
- jQuery — instalado como dependência, mas ainda não utilizado; uso previsto para a etapa funcional
- JSON Server — previsto para a etapa final/funcional
- Persistência de dados — prevista para a etapa final/funcional
- Integração com API de cotações (brapi.dev) — prevista para a etapa final/funcional
- Node.js
- NPM
- Git
- GitHub

---

## 🌐 API Pública

O projeto prevê a integração com a **brapi.dev**, uma API pública de cotações de ativos, para complementar as informações dos investimentos cadastrados pelo usuário.

A API será utilizada na etapa final/funcional para consultar a cotação atual de determinados ativos e apresentar essas informações na aplicação. **Nesta entrega, a integração ainda não está implementada.**

**API:** brapi.dev\
**Integração:** prevista para a etapa final/funcional

---

## 🚀 Link para o projeto em produção

**GitHub Pages:** pendente de publicação

---

## ▶️ Instruções de Execução

Pré-requisitos: Node.js e NPM instalados.

1. Instale as dependências do projeto:

```bash
npm install
```

2. Execute o projeto localmente abrindo o arquivo `index.html` no navegador ou utilizando um servidor HTTP local de sua preferência (por exemplo, a extensão Live Server do VS Code).

> Observação: o `package.json` não possui scripts `start` ou `dev` configurados nesta entrega.

---

## 🖥️ Telas da Aplicação

As capturas de tela ainda serão adicionadas.

Páginas HTML implementadas:

- `index.html` — página inicial
- `login.html` — login
- `cadastro.html` — cadastro
- `dashboard.html` — dashboard
- `gastos.html` — listagem de gastos
- `gasto-form.html` — formulário de gasto
- `investimentos.html` — investimentos e área de cotações
- `investimento-form.html` — formulário de investimento
