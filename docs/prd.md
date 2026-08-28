# Product Requirements Document (PRD) - FinanceBook

## 1. Visão Geral e Objetivo

A organização das finanças pessoais pode se tornar uma tarefa difícil quando informações sobre gastos e investimentos estão distribuídas em diferentes aplicativos e planilhas.

Diante desse cenário, o **FinanceBook — Livro Financeiro** tem como objetivo facilitar a organização financeira pessoal, oferecendo uma aplicação que permita ao usuário registrar e acompanhar seus gastos e investimentos em um único lugar.

Na área de investimentos, o sistema também utilizará uma **API pública de cotações de ativos** para complementar as informações cadastradas pelo usuário.

O FinanceBook possui caráter exclusivamente informativo e organizacional. A aplicação não realizará pagamentos, transferências ou operações reais de compra e venda de ativos.

---

## 2. Atores do Sistema

- **Visitante:** Usuário que acessa o FinanceBook e pode conhecer a proposta da aplicação, realizar seu cadastro ou acessar sua conta.

- **Usuário:** Pessoa autenticada que utiliza o sistema para registrar e acompanhar seus gastos e investimentos.

---

## 3. Histórias de Usuário e Escopo

As funcionalidades abaixo são descritas sob a perspectiva do usuário que deseja organizar suas finanças pessoais.

---

### 👀 Épico 1: Acesso ao Sistema

- **US01 - Apresentação do sistema:** Como um Visitante, quero visualizar a proposta e as principais funcionalidades do FinanceBook, para entender como a aplicação pode me ajudar na organização das minhas finanças.

- **US02 - Cadastro de usuário:** Como um Visitante, quero criar uma conta informando meus dados, para poder utilizar o FinanceBook.

- **US03 - Login:** Como um Usuário, quero realizar login utilizando meu e-mail e senha, para acessar meus dados financeiros.

- **US04 - Encerramento da sessão:** Como um Usuário, quero sair da minha conta, para impedir o acesso aos meus dados quando eu não estiver utilizando o sistema.

---

### 💰 Épico 2: Gastos

- **US05 - Cadastro de gastos:** Como um Usuário, quero cadastrar meus gastos informando descrição, valor, categoria e data, para manter meu controle financeiro atualizado.
  - *Critérios de Aceitação:* Os campos obrigatórios devem ser preenchidos, o valor deve ser maior que zero e a data deve ser válida.

- **US06 - Consulta de gastos:** Como um Usuário, quero visualizar meus gastos cadastrados, para acompanhar minhas despesas.
  - *Critérios de Aceitação:* Devem ser exibidos somente os gastos associados ao usuário autenticado.

- **US07 - Edição de gastos:** Como um Usuário, quero editar um gasto cadastrado, para corrigir ou atualizar suas informações.
  - *Critérios de Aceitação:* Os dados alterados devem passar pelas mesmas validações utilizadas no cadastro.

- **US08 - Exclusão de gastos:** Como um Usuário, quero excluir um gasto cadastrado, para remover informações que não sejam mais necessárias.
  - *Critérios de Aceitação:* O sistema deve solicitar confirmação antes da exclusão.

- **US09 - Filtro de gastos:** Como um Usuário, quero filtrar meus gastos por categoria e período, para localizar informações específicas com maior facilidade.

- **US10 - Total de gastos:** Como um Usuário, quero visualizar o total dos meus gastos em determinado período, para acompanhar quanto estou gastando.

---

### 📈 Épico 3: Investimentos

- **US11 - Cadastro de investimentos:** Como um Usuário, quero cadastrar meus investimentos informando ativo, tipo, quantidade, valor investido e data, para manter minha carteira organizada.
  - *Critérios de Aceitação:* Os campos obrigatórios devem ser preenchidos e a quantidade e o valor investido devem ser maiores que zero.

- **US12 - Consulta de investimentos:** Como um Usuário, quero visualizar meus investimentos cadastrados, para acompanhar minha carteira.
  - *Critérios de Aceitação:* Devem ser exibidos somente os investimentos associados ao usuário autenticado.

- **US13 - Edição de investimentos:** Como um Usuário, quero editar um investimento cadastrado, para corrigir ou atualizar suas informações.
  - *Critérios de Aceitação:* Os dados alterados devem passar pelas mesmas validações utilizadas no cadastro.

- **US14 - Exclusão de investimentos:** Como um Usuário, quero excluir um investimento cadastrado, para manter minha carteira atualizada.
  - *Critérios de Aceitação:* O sistema deve solicitar confirmação antes da exclusão.

- **US15 - Total investido:** Como um Usuário, quero visualizar o valor total investido, para ter uma visão geral dos recursos destinados aos meus investimentos.

- **US16 - Consulta de cotação:** Como um Usuário, quero consultar a cotação atual de um ativo cadastrado, para obter uma referência atualizada sobre seu valor.
  - *Critérios de Aceitação:* O sistema deve realizar uma requisição assíncrona à API pública e informar o usuário caso a consulta não esteja disponível.

---

### 📊 Épico 4: Dashboard

- **US17 - Resumo financeiro:** Como um Usuário, quero visualizar um resumo das minhas informações financeiras no Dashboard, para compreender rapidamente minha situação financeira.

- **US18 - Resumo de gastos:** Como um Usuário, quero visualizar o total dos meus gastos no Dashboard, para acompanhar minhas despesas sem precisar acessar a página de gastos.

- **US19 - Resumo de investimentos:** Como um Usuário, quero visualizar o total investido no Dashboard, para acompanhar rapidamente minha carteira.

- **US20 - Distribuição de gastos:** Como um Usuário, quero visualizar a distribuição dos meus gastos por categoria, para identificar onde estou concentrando minhas despesas.

---

### 📝 Épico 5: Formulários e Validações

- **US21 - Validação de formulários:** Como um Usuário, quero receber mensagens de validação ao preencher os formulários, para corrigir informações inválidas antes de enviá-las.
  - *Critérios de Aceitação:* O sistema deve impedir o envio quando houver campos obrigatórios vazios ou informações inválidas.

- **US22 - Seleção de categorias:** Como um Usuário, quero selecionar categorias através de listas de opções, para facilitar a classificação dos meus gastos e investimentos.

- **US23 - Persistência dos dados:** Como um Usuário, quero que meus gastos e investimentos sejam armazenados após o cadastro, para que eu possa consultá-los posteriormente.

- **US24 - Identificação dos registros:** Como um Usuário, quero que meus gastos e investimentos sejam associados à minha conta, para manter meus dados separados dos demais usuários.

---

## 4. Regras de Negócio

- **RN01 - Valor dos gastos:** O valor informado para um gasto deve ser maior que zero.

- **RN02 - Dados dos gastos:** Todo gasto deve possuir descrição, valor, categoria e data.

- **RN03 - Categorias de gastos:** Todo gasto deve estar associado a uma categoria.

- **RN04 - Dados dos investimentos:** Todo investimento deve possuir ativo, tipo, quantidade, valor investido e data.

- **RN05 - Quantidade de investimentos:** A quantidade informada para um investimento deve ser maior que zero.

- **RN06 - Valor dos investimentos:** O valor investido deve ser maior que zero.

- **RN07 - Associação de registros:** Todo gasto e investimento deve estar associado a um usuário.

- **RN08 - Isolamento de dados:** O usuário deve visualizar somente os gastos e investimentos associados à sua conta.

- **RN09 - Exclusão de registros:** Gastos e investimentos excluídos pelo usuário não devem permanecer disponíveis na listagem.

- **RN10 - Consulta de cotação:** As cotações dos ativos serão obtidas através de uma API pública e utilizadas como informações complementares aos investimentos cadastrados.

- **RN11 - Indisponibilidade da API:** Caso a API pública não esteja disponível, o sistema deverá informar o usuário sem comprometer os dados cadastrados.

- **RN12 - Operações financeiras:** O FinanceBook não realizará pagamentos, transferências ou operações reais de compra e venda de ativos.

---

## 5. Fora do Escopo

As seguintes funcionalidades não fazem parte do escopo inicial do FinanceBook:

- Realização de pagamentos.
- Transferências bancárias.
- Compra ou venda de ativos.
- Integração com contas bancárias.
- Abertura de contas.
- Operações de cartão de crédito.
- Consultoria financeira.
- Recomendação personalizada de investimentos.
- Custódia de ativos financeiros.
- Notícias sobre o mercado financeiro.
- Indicadores econômicos gerais.
- Cotação de dólar, petróleo ou índices como funcionalidades independentes.
