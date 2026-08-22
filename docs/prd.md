# Product Requirements Document (PRD) - FinanceBook

## 1. Visão Geral e Objetivo

A organização das finanças pessoais pode se tornar uma tarefa difícil quando informações sobre gastos, investimentos e mercado financeiro estão distribuídas em diferentes aplicativos, planilhas e sites.

Essa falta de centralização pode dificultar o acompanhamento das despesas, dos investimentos e das mudanças no cenário econômico, tornando mais difícil para o usuário compreender sua situação financeira.

Diante desse cenário, o projeto tem como objetivo facilitar a organização financeira pessoal, oferecendo uma aplicação que permita ao usuário registrar seus gastos, acompanhar seus investimentos e consultar informações relevantes do mercado financeiro em um único lugar.

O **FinanceBook — Livro Financeiro** permitirá que o usuário tenha uma visão mais clara de sua situação financeira, além de acompanhar indicadores como cotação do dólar, Ibovespa e petróleo.

O sistema possui caráter exclusivamente informativo e organizacional. A aplicação não realizará pagamentos, transferências ou operações reais de compra e venda de ativos.

---

## 2. Atores do Sistema

- **Visitante:** Usuário que acessa o FinanceBook e pode conhecer a proposta e as principais funcionalidades da aplicação.

- **Usuário:** Pessoa que utiliza o sistema para registrar e acompanhar seus gastos, gerenciar seus investimentos e consultar informações do mercado financeiro.

- **Mercado Financeiro:** Fonte externa responsável pelo fornecimento de informações e indicadores utilizados na área de acompanhamento do mercado.

---

## 3. Histórias de Usuário e Escopo

Abaixo estão as funcionalidades escritas sob a perspectiva do usuário final, que deseja organizar suas finanças pessoais e acompanhar informações do mercado financeiro.

---

### 👀 Épico 1: Visitante

- **US01 - Apresentação do sistema:** Como um Visitante, quero visualizar de forma clara a proposta e as principais funcionalidades do FinanceBook, para entender como a aplicação pode me ajudar na organização das minhas finanças.

- **US02 - Visualização das áreas:** Como um Visitante, quero visualizar quais recursos estão disponíveis na aplicação, para conhecer as possibilidades oferecidas pelo FinanceBook.

---

### 💰 Épico 2: Gastos

- **US03 - Cadastro de gastos:** Como um Usuário, quero cadastrar meus gastos informando descrição, valor, categoria e data, para manter meu controle financeiro atualizado.
  - *Critérios de Aceitação:* Os campos obrigatórios devem ser preenchidos; o valor deve ser maior que zero; a data deve ser válida.

- **US04 - Listagem de gastos:** Como um Usuário, quero visualizar todos os meus gastos cadastrados, para acompanhar minhas despesas.

- **US05 - Edição de gastos:** Como um Usuário, quero editar um gasto cadastrado, para corrigir ou atualizar informações.
  - *Critérios de Aceitação:* Os dados alterados devem passar pelas mesmas validações utilizadas no cadastro.

- **US06 - Exclusão de gastos:** Como um Usuário, quero excluir um gasto cadastrado, para remover informações que não sejam mais necessárias.
  - *Critérios de Aceitação:* O sistema deve solicitar uma confirmação antes da exclusão do registro.

- **US07 - Categorização de gastos:** Como um Usuário, quero selecionar uma categoria para cada gasto, para organizar melhor minhas despesas.

- **US08 - Filtro de gastos:** Como um Usuário, quero filtrar meus gastos por categoria e/ou período, para localizar informações específicas com maior facilidade.

- **US09 - Visualização do total de gastos:** Como um Usuário, quero visualizar o valor total dos meus gastos, para acompanhar quanto estou gastando em determinado período.

---

### 📈 Épico 3: Investimentos

- **US10 - Cadastro de investimentos:** Como um Usuário, quero cadastrar meus investimentos informando ativo, tipo, quantidade, valor investido e data, para manter minha carteira organizada.
  - *Critérios de Aceitação:* Os campos obrigatórios devem ser preenchidos; a quantidade e o valor investido devem ser maiores que zero.

- **US11 - Listagem de investimentos:** Como um Usuário, quero visualizar todos os meus investimentos cadastrados, para acompanhar minha carteira.

- **US12 - Edição de investimentos:** Como um Usuário, quero editar um investimento cadastrado, para corrigir ou atualizar suas informações.

- **US13 - Exclusão de investimentos:** Como um Usuário, quero excluir um investimento cadastrado, para manter minha carteira atualizada.
  - *Critérios de Aceitação:* O sistema deve solicitar confirmação antes da exclusão.

- **US14 - Visualização do valor investido:** Como um Usuário, quero visualizar o valor investido em cada ativo, para acompanhar quanto dinheiro está destinado aos meus investimentos.

- **US15 - Visualização do total investido:** Como um Usuário, quero visualizar o valor total dos meus investimentos, para ter uma visão geral do dinheiro destinado à minha carteira.

---

### 📊 Épico 4: Dashboard

- **US16 - Resumo financeiro:** Como um Usuário, quero visualizar um resumo da minha situação financeira, para compreender rapidamente minhas principais informações financeiras.

- **US17 - Resumo de gastos:** Como um Usuário, quero visualizar o total dos meus gastos no Dashboard, para acompanhar minhas despesas sem precisar acessar a página de gastos.

- **US18 - Resumo de investimentos:** Como um Usuário, quero visualizar o total investido no Dashboard, para acompanhar rapidamente minha carteira.

- **US19 - Indicadores financeiros:** Como um Usuário, quero visualizar alguns indicadores do mercado financeiro no Dashboard, para acompanhar rapidamente o cenário econômico.

---

### 🌎 Épico 5: Mercado Financeiro

- **US20 - Consulta ao mercado:** Como um Usuário, quero acessar informações do mercado financeiro, para acompanhar indicadores econômicos relevantes.

- **US21 - Cotação do dólar:** Como um Usuário, quero visualizar a cotação do dólar, para acompanhar a variação da moeda.

- **US22 - Consulta do Ibovespa:** Como um Usuário, quero visualizar informações do Ibovespa, para acompanhar o desempenho do principal índice da bolsa brasileira.

- **US23 - Consulta do petróleo:** Como um Usuário, quero visualizar informações relacionadas ao petróleo, para acompanhar a variação desse indicador no mercado.

- **US24 - Visualização de variações:** Como um Usuário, quero visualizar as variações dos indicadores financeiros, para identificar se houve valorização ou desvalorização.

- **US25 - Atualização dos dados:** Como um Usuário, quero atualizar as informações do mercado financeiro, para visualizar dados mais recentes.

- **US26 - Tratamento de erro:** Como um Usuário, quero receber uma mensagem quando não for possível carregar os dados do mercado financeiro, para saber que ocorreu um problema na consulta.

---

### 📝 Épico 6: Formulários

- **US27 - Validação de campos obrigatórios:** Como um Usuário, quero receber uma indicação quando deixar um campo obrigatório vazio, para saber o que preciso preencher antes de enviar o formulário.
  - *Critérios de Aceitação:* O formulário não deve ser enviado enquanto existirem campos obrigatórios vazios.

- **US28 - Validação de informações:** Como um Usuário, quero que informações inválidas sejam identificadas durante o preenchimento, para evitar o cadastro de dados incorretos.

- **US29 - Seleção de categorias:** Como um Usuário, quero selecionar uma categoria através de uma lista de opções, para facilitar a classificação dos meus gastos.

---

## 4. Regras de Negócio

- **RN01 - Valor dos gastos:** O valor informado para um gasto deve ser maior que zero.

- **RN02 - Dados dos gastos:** Todo gasto deve possuir descrição, valor, categoria e data.

- **RN03 - Categorias:** Todo gasto deve estar associado a uma categoria.

- **RN04 - Dados dos investimentos:** Todo investimento deve possuir ativo, tipo, quantidade, valor investido e data.

- **RN05 - Quantidade de investimentos:** A quantidade informada para um investimento deve ser maior que zero.

- **RN06 - Valor dos investimentos:** O valor investido deve ser maior que zero.

- **RN07 - Exclusão de registros:** Gastos e investimentos excluídos pelo usuário não devem permanecer disponíveis na listagem.

- **RN08 - Dados do mercado:** As informações apresentadas na área de mercado devem ser obtidas de uma fonte externa de dados financeiros.

- **RN09 - Indisponibilidade do mercado:** Caso não seja possível obter os dados do mercado financeiro, o sistema deve informar o usuário.

- **RN10 - Caráter informativo:** As informações do mercado financeiro apresentadas pelo FinanceBook possuem caráter exclusivamente informativo.

- **RN11 - Operações financeiras:** O FinanceBook não realizará pagamentos, transferências ou operações reais de compra e venda de ativos.

---

## 5. Fora do Escopo

As seguintes funcionalidades não fazem parte do escopo inicial do FinanceBook:

- Realização de pagamentos.
- Transferências bancárias.
- Compra de ativos.
- Venda de ativos.
- Integração com contas bancárias.
- Abertura de contas.
- Operações de cartão de crédito.
- Consultoria financeira.
- Recomendação personalizada de investimentos.
- Custódia de ativos financeiros.