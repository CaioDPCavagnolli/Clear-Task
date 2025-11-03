## Documentação - Sprint 2

---
## 🏅 Desafio

O desafio desta sprint é construir a camada de gerenciamento da plataforma, focando exclusivamente na perspectiva do agente. Após a Sprint 1, onde os usuários podem criar e ver seus próprios chamados, o objetivo agora é dar aos agentes as ferramentas essenciais para atuar sobre essas solicitações. Ao final da sprint, um agente deverá conseguir visualizar todo o fluxo de trabalho, alterar o progresso de um chamado e delegar responsabilidades, transformando o sistema de um portal de registro em uma central de operações funcional.

---
## 📋 User Stories

| Prioridade | User Story                                                                                                                                       | Sprint | Requisito do Cliente | Status   |
| :--------: | -----------------------------------------------------------------------------------------------------------------------------------------------  | :----: | :------------------: | :------: |
|    Alta    | Como agente, quero visualizar a lista de todos os chamados, para que eu possa gerenciar as solicitações.                                         |   2    | R04                  |    ✅    |
|    Alta    | Como agente, quero alterar o status de um chamado (ex: de "aberto" para "em andamento"), para que a equipe e o usuário saibam o progresso.       |   2    | R05                  |    ✅    |
|    Alta    | Como agente, quero atribuir um chamado a outro agente, para que a responsabilidade seja clara.                                                   |   2    | R06                  |    ✅    |

---

## 🏅 DoR - Definition of Ready

|  Critério                    | Descrição                                                                                                                                                                                                                                              |
| :--------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|Formato da História           |	Todas as histórias seguem o padrão "Como um agente, quero [...], para que [...]".                                                                                                                                                                     |
|Critérios de Aceitação Claros |	A história possui uma lista de verificação objetiva. Exemplo (para R05): "Dado que sou um agente na tela de um chamado, quando eu selecionar o status 'Em Andamento', então o sistema deve salvar a alteração e exibir o novo status na lista geral". |
|Independência                 |	A história pode ser desenvolvida sem bloqueios. Exemplo: Foi definido que a R05 (alterar status) e a R06 (atribuir agente) serão implementadas na tela de lista criada pela R04, portanto, a R04 deve ser iniciada primeiro.                          |
|Valor de Negócio              |	O propósito é claro para todos. Exemplo: A equipe entende que a R06 (atribuir chamado) é crucial para organizar o fluxo de trabalho e evitar que múltiplos agentes trabalhem na mesma tarefa.                                                         |
|Estimativa Acordada           |	A equipe pontuou o esforço necessário para cada uma das três histórias da sprint no Planning Poker.                                                                                                                                                   |
|Dependências Mapeadas         |	Exemplo: Para a R06 (atribuir chamado), foi identificado que o backend precisará de um endpoint que retorne a lista de agentes disponíveis.                                                                                                           |
|Protótipos/Mockups Anexados   |	A interface visual está definida. Exemplo: Para a R04 (visualizar lista), o link do Figma mostrando o design da tabela de chamados, com colunas para status e agente responsável, está anexado à tarefa.                                              |
|Escopo Técnico Definido       |	O contrato entre Frontend e Backend está claro. Exemplo: Para a R05, foi acordado que o front-end enviará uma requisição PATCH /api/chamados/{id} com o corpo {"status": "em_andamento"}.                                                             |

---

## 🏅 DoD - Definition of Done

|  Critério                       | Descrição                                                                                                                                                                                                                                      |
| :-----------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|Código em Produção               |	O código das funcionalidades de agente foi integrado à branch principal (main ou develop) e está disponível no ambiente de testes/homologação.                                                                                                 |
|Critérios de Aceitação Atendidos |	Todos os cenários foram validados. Exemplo: Para a R05, foi confirmado que a mudança de status funciona e que a interface reflete a alteração imediatamente.                                                                                   |
|Testes Unitários/Integrados      |	O código possui cobertura de testes automatizados. Exemplo: O método do backend que altera o status do chamado (R05) possui um teste unitário para garantir que apenas status válidos sejam aceitos.                                           |
|Revisão de Código (Code Review)  |	O Pull Request da funcionalidade de atribuir um chamado (R06) foi revisado e aprovado por outro desenvolvedor.                                                                                                                                 |
|Testes Manuais Realizados        |	O fluxo completo do agente foi testado manualmente. Exemplo: "Loguei como agente, acessei a lista (R04), atribuí um chamado a mim mesmo (R06), mudei seu status para 'Em Andamento' (R05) e verifiquei se os dados foram salvos corretamente." |
|Validação do PO                  |	O Product Owner validou a entrega. Exemplo: O PO confirmou que a lista de chamados (R04) exibe todas as informações necessárias para que o gerenciamento seja eficaz.                                                                          |
|Documentação Atualizada          |	A documentação técnica foi atualizada. Exemplo: Os novos endpoints para listar todos os chamados, alterar status e atribuir agentes foram adicionados à coleção do Postman/Swagger do projeto.                                                 |
|Sem Débitos Técnicos Graves      |	A solução é sustentável e não foram usados "atalhos" ou "gambiarras" para implementar as funcionalidades de gerenciamento.                                                                                                                     |
---

## 🎓 Equipe

| Membro          |  Função                      |
| :-------------: | :--------------------------: |
| Caio Damaceno   | Product Owner & Scrum Master |
| Giovani Algusto | Developer                    |
