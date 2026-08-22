
# Architecture — FinanceBook

## 1. Visão Geral

O FinanceBook será desenvolvido como uma aplicação web responsiva, utilizando tecnologias de frontend e APIs para manipulação e consulta de dados.

A aplicação será responsável por apresentar as interfaces, receber informações do usuário, validar formulários, realizar operações de cadastro e consumir serviços externos.

A arquitetura será organizada de forma modular, permitindo separar responsabilidades entre páginas, componentes, serviços, estilos e funções auxiliares.

---

## 2. Arquitetura da Aplicação

```mermaid
flowchart TD

    U[Usuário]

    U --> F[Frontend]

    F --> D[Dashboard]
    F --> G[Gastos]
    F --> I[Investimentos]
    F --> M[Mercado]

    D --> JS[JavaScript / jQuery]
    G --> JS
    I --> JS
    M --> JS

    JS --> WS[Web Storage]

    JS --> JSON[JSON Server]
    JS --> API[API Pública]

    JSON --> DB[(Dados Financeiros)]
    API --> MF[Dados do Mercado]