# Product Requirements Document (PRD) - FinanceBook

## 1. Visão Geral e Objetivo

A organização das finanças pessoais pode se tornar uma tarefa difícil quando informações sobre gastos e investimentos estão distribuídas em diferentes aplicativos e planilhas.

Diante desse cenário, o **FinanceBook — Livro Financeiro** tem como objetivo facilitar a organização financeira pessoal, oferecendo uma aplicação que permita ao usuário registrar, consultar e acompanhar seus gastos e investimentos em um único lugar.

Na área de investimentos, o sistema utilizará a **brapi.dev**, uma API pública de dados financeiros, para consultar cotações de ativos e complementar as informações cadastradas pelo usuário.

O FinanceBook possui caráter exclusivamente informativo e organizacional. A aplicação não realizará pagamentos, transferências ou operações reais de compra e venda de ativos.

---

## 2. Atores do Sistema

- **Visitante:** Usuário que acessa o FinanceBook e pode conhecer a proposta da aplicação, realizar seu cadastro ou acessar sua conta.

- **Usuário:** Pessoa autenticada que utiliza o sistema para registrar, consultar e acompanhar seus gastos e investimentos.

---

## 3. Histórias de Usuário e Escopo

As funcionalidades abaixo são descritas sob a perspectiva do usuário que deseja organizar suas finanças pessoais.

### 👀 Épico 1: Acesso e Conta

- **US01 - Apresentação do sistema:** Como um Visitante, quero conhecer a proposta e as principais funcionalidades do FinanceBook, para entender como a aplicação pode auxiliar na organização das minhas finanças.

- **US02 - Cadastro de usuário:** Como um Visitante, quero criar uma conta informando meus dados, para poder utilizar o FinanceBook.
  - *Critérios de Aceitação:* Os campos obrigatórios devem ser preenchidos, o e-mail deve possuir formato válido e a senha deve atender aos requisitos definidos pelo sistema.

- **US03 - Autenticação:** Como um Usuário, quero entrar e sair da minha conta utilizando minhas credenciais, para acessar meus dados financeiros de forma controlada.
  - *Critérios de Aceitação:* O sistema deve solicitar e-mail e senha para acesso, impedir o acesso com credenciais inválidas e permitir o encerramento da sessão.

### 💰 Épico 2: Cadastro de Gastos

- **US04 - Registro de gastos:** Como um Usuário, quero cadastrar um gasto informando descrição, valor, categoria e data, para registrar minhas despesas e manter meu controle financeiro atualizado.
  - *Critérios de Aceitação:* Descrição, valor, categoria e data devem ser preenchidos, o valor deve ser maior que zero, a data deve ser válida e o registro deve ser associado ao usuário autenticado.

### 📝 Épico 3: Gerenciamento de Gastos

- **US05 - Atualização de gastos:** Como um Usuário, quero editar um gasto cadastrado, para corrigir ou atualizar suas informações.
  - *Critérios de Aceitação:* O gasto deve pertencer ao usuário autenticado e os dados alterados devem passar pelas mesmas validações utilizadas no cadastro.

- **US06 - Exclusão de gastos:** Como um Usuário, quero excluir um gasto cadastrado, para remover registros que não sejam mais necessários.
  - *Critérios de Aceitação:* O gasto deve pertencer ao usuário autenticado, o sistema deve solicitar confirmação antes da exclusão e o registro excluído não deve permanecer disponível para consulta.

### 🔎 Épico 4: Consulta e Análise de Gastos

- **US07 - Consulta de gastos:** Como um Usuário, quero visualizar meus gastos cadastrados e filtrá-los por categoria e período, para localizar e acompanhar minhas despesas com facilidade.
  - *Critérios de Aceitação:* Devem ser exibidos somente os gastos associados ao usuário autenticado e devem estar disponíveis filtros por categoria e período.

- **US08 - Análise de gastos:** Como um Usuário, quero visualizar o total dos meus gastos e sua distribuição por categoria, para compreender como estou utilizando meu dinheiro.

### 📈 Épico 5: Cadastro de Investimentos

- **US09 - Registro de investimentos:** Como um Usuário, quero cadastrar um investimento informando ativo, tipo, quantidade, valor investido e data, para manter minha carteira organizada.
  - *Critérios de Aceitação:* Os campos obrigatórios devem ser preenchidos, a quantidade deve ser maior que zero, o valor investido deve ser maior que zero e o registro deve ser associado ao usuário autenticado.

### ⚙️ Épico 6: Gerenciamento de Investimentos

- **US10 - Atualização de investimentos:** Como um Usuário, quero editar um investimento cadastrado, para corrigir ou atualizar suas informações.
  - *Critérios de Aceitação:* O investimento deve pertencer ao usuário autenticado e os dados alterados devem passar pelas mesmas validações utilizadas no cadastro.

- **US11 - Exclusão de investimentos:** Como um Usuário, quero excluir um investimento cadastrado, para manter minha carteira atualizada.
  - *Critérios de Aceitação:* O investimento deve pertencer ao usuário autenticado, o sistema deve solicitar confirmação antes da exclusão e o registro excluído não deve permanecer disponível para consulta.

### 📊 Épico 7: Consulta e Análise de Investimentos

- **US12 - Consulta da carteira:** Como um Usuário, quero visualizar meus investimentos cadastrados e o total investido, para acompanhar minha carteira e ter uma visão geral dos recursos destinados aos investimentos.
  - *Critérios de Aceitação:* Devem ser exibidos somente os investimentos associados ao usuário autenticado e o total investido deve considerar os investimentos cadastrados pelo usuário.

### 📡 Épico 8: Cotações de Ativos

- **US13 - Consulta de cotação:** Como um Usuário, quero consultar a cotação atual de um ativo cadastrado, para obter uma referência atualizada sobre seu valor.
  - *Critérios de Aceitação:* O sistema deve realizar uma requisição assíncrona à brapi.dev, apresentar os dados retornados pela API e informar o usuário caso a consulta não esteja disponível.

### 📋 Épico 9: Dashboard Financeiro

- **US14 - Visão geral financeira:** Como um Usuário, quero visualizar um resumo das minhas informações financeiras no Dashboard, para compreender rapidamente minha situação financeira.
  - *Critérios de Aceitação:* O Dashboard deve apresentar informações consolidadas dos gastos e investimentos, incluindo o total de gastos, o total investido e a distribuição dos gastos por categoria.

### 🏷️ Épico 10: Classificação de Gastos

- **US15 - Classificação de gastos:** Como um Usuário, quero selecionar uma categoria ao cadastrar um gasto, para organizar minhas despesas e facilitar sua análise.
  - *Critérios de Aceitação:* O gasto deve possuir uma categoria e ela deve ser selecionada a partir das opções disponíveis no sistema.

### ✅ Épico 11: Validação e Feedback

- **US16 - Validação dos dados:** Como um Usuário, quero receber mensagens de validação ao preencher os formulários, para corrigir informações inválidas antes de enviar meus dados.
  - *Critérios de Aceitação:* O sistema deve impedir o envio de informações inválidas, identificar campos obrigatórios não preenchidos e apresentar mensagens adequadas para os dados inválidos.

- **US17 - Feedback das operações:** Como um Usuário, quero receber um retorno após realizar uma operação, para saber se ela foi concluída corretamente ou se ocorreu algum problema.
  - *Critérios de Aceitação:* O sistema deve informar o sucesso ou falha das operações realizadas e apresentar mensagens compreensíveis para erros de comunicação com APIs ou outras operações.

---

## 4. Regras de Negócio

- **RN01 - Valor dos gastos:** O valor informado para um gasto deve ser maior que zero.
- **RN02 - Dados dos gastos:** Todo gasto deve possuir descrição, valor, categoria e data.
- **RN03 - Categorias de gastos:** Todo gasto deve estar associado a uma categoria.
- **RN04 - Dados dos investimentos:** Todo investimento deve possuir ativo, tipo, quantidade, valor investido e data.
- **RN05 - Quantidade de investimentos:** A quantidade informada para um investimento deve ser maior que zero.
- **RN06 - Valor dos investimentos:** O valor investido deve ser maior que zero.
- **RN07 - Associação de registros:** Todo gasto e investimento deve estar associado a um usuário.
- **RN08 - Isolamento de dados:** O usuário deve visualizar e manipular somente os gastos e investimentos associados à sua conta.
- **RN09 - Persistência dos registros:** Os gastos e investimentos cadastrados devem ser armazenados e permanecer disponíveis para consulta posteriormente.
- **RN10 - Exclusão de registros:** Gastos e investimentos excluídos pelo usuário não devem permanecer disponíveis para consulta.
- **RN11 - Consulta de cotação:** As cotações dos ativos serão obtidas através da brapi.dev e utilizadas como informações complementares aos investimentos cadastrados.
- **RN12 - Indisponibilidade da API:** Caso a brapi.dev esteja indisponível ou a consulta não seja realizada com sucesso, o sistema deverá informar o usuário sem comprometer os dados cadastrados.
- **RN13 - Validação dos dados:** Os dados inseridos pelo usuário devem atender às validações definidas para cada tipo de registro antes de serem armazenados.
- **RN14 - Operações financeiras:** O FinanceBook não realizará pagamentos, transferências ou operações reais de compra e venda de ativos.

---

## 5. Fora do Escopo

As seguintes funcionalidades não fazem parte do escopo inicial do FinanceBook:

- Realização de pagamentos.
- Transferências bancárias.
- Compra ou venda de ativos.
- Integração com contas bancárias.
- Abertura de contas.
- Operações de cartão de crédito.
- Gerenciamento de perfil pessoal.
- Consultoria financeira.
- Recomendação personalizada de investimentos.
- Custódia de ativos financeiros.
- Notícias sobre o mercado financeiro.
- Indicadores econômicos gerais.
- Cotação de dólar, petróleo ou índices como funcionalidades independentes.