## Documentação - Sprint 3

---
## 🏅 Desafio

O desafio desta sprint é dar o primeiro passo para transformar nosso sistema de reativo para proativo, introduzindo Inteligência Artificial no fluxo de trabalho do agente. O objetivo é automatizar tarefas cognitivas e repetitivas, como a classificação e a etiquetagem de chamados. Ao final da sprint, a plataforma deverá analisar o conteúdo de novos chamados e, de forma autônoma, sugerir uma categoria e tags relevantes, reduzindo drasticamente o tempo de triagem manual e acelerando o processo de resolução para o usuário final.

---
## 📋 User Stories

| Prioridade | User Story                                                                                                                                       | Sprint | Requisito do Cliente | Status   |
| :--------: | -----------------------------------------------------------------------------------------------------------------------------------------------  | :----: | :------------------: | :------: |
|    Média   | Como agente, quero que a IA classifique automaticamente o tipo de chamado, para que o encaminhamento seja mais rápido.                           |   3    | R07                  |    ✅    |
|    Média   |	Como agente, quero que a IA sugira tags relevantes para um chamado, para que a organização seja mais eficiente.                                 |   3    | R08                  |    ✅    |

---

## 🏅 DoR - Definition of Ready

|  Critério                    | Descrição                                                                                                                                                                                                                                                                         |
| :--------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|Formato da História           |	As histórias estão no formato padrão, focadas no valor para o agente.                                                                                                                                                                                                            |
|Critérios de Aceitação Claros |	Os critérios definem o comportamento esperado e as métricas de sucesso. Exemplo (para R07): "1. A classificação da IA deve ser exibida na tela do chamado. 2. O agente deve poder corrigir a classificação. 3. A precisão do modelo em nossos testes deve ser de no mínimo 75%." |
|Independência                 |	As dependências técnicas entre as histórias são conhecidas. Exemplo: Foi definido que ambas as histórias (R07 e R08) podem usar a mesma chamada para a API de IA, otimizando o processo.                                                                                         |
|Valor de Negócio              |	O impacto no processo está claro. Exemplo: A equipe entende que a R08 (sugestão de tags) irá padronizar a catalogação dos problemas, facilitando a criação de relatórios futuros.                                                                                                |
|Estimativa Acordada           |	As histórias foram estimadas, considerando a complexidade da integração com um novo serviço de IA.                                                                                                                                                                               |
|Dependências Mapeadas         |	As dependências externas foram resolvidas. Exemplo: "A API de IA (ex: OpenAI, Vertex AI) foi escolhida. As chaves de acesso foram geradas e configuradas. Uma análise de custo inicial foi realizada."                                                                           |
|Protótipos/Mockups Anexados   |	A experiência do usuário com a IA está desenhada. Exemplo (para R08): "O Figma mostra como as tags sugeridas aparecerão: como pílulas clicáveis que o agente pode aceitar ou descartar."                                                                                         |
|Escopo Técnico Definido       |	A arquitetura da solução está planejada. Exemplo (para R07 e R08): "Está definido que o Backend, ao criar um chamado, enviará o título e a descrição para a API de IA e armazenará a resposta (categoria e tags) em novos campos no banco de dados."                             |

---

## 🏅 DoD - Definition of Done

|  Critério                       | Descrição                                                                                                                                                                                                                                         |
| :-----------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|Código em Produção               |	O código que faz a integração com a IA foi integrado à branch principal e está funcionando no ambiente de homologação.                                                                                                                            |
|Critérios de Aceitação Atendidos |	As funcionalidades foram validadas, incluindo as métricas. Exemplo: Foi confirmado que a precisão da classificação automática (R07) atingiu a meta de 75% no conjunto de testes e que o agente consegue corrigir as sugestões.                    |
|Testes Unitários/Integrados      |	A integração com o serviço de IA é resiliente. Exemplo: Existem testes que validam o comportamento do sistema quando a API de IA responde com sucesso, com erro ou demora para responder (timeout).                                               |
|Revisão de Código (Code Review)  |	O Pull Request com a lógica de IA foi revisado, com atenção especial ao tratamento de chaves de API e segurança dos dados.                                                                                                                        |
|Testes Manuais Realizados        |	O fluxo foi testado considerando a natureza da IA. Exemplo: "Criei 5 chamados com temas diferentes (hardware, software, acesso). Verifiquei se as classificações (R07) e tags (R08) foram coerentes e se consegui corrigi-las quando a IA errou." |
|Validação do PO                  |	O Product Owner validou o valor da automação. Exemplo: O PO confirmou que as sugestões da IA são, na maioria das vezes, úteis e representam uma economia real de tempo para o agente.                                                             |
|Documentação Atualizada          |	A documentação técnica reflete a nova arquitetura. Exemplo: O README do projeto foi atualizado com as novas variáveis de ambiente necessárias (ex: AI_API_KEY, AI_API_ENDPOINT).                                                                  |
|Sem Débitos Técnicos Graves      |	A integração foi feita de forma segura e escalável, sem expor chaves de API no código-fonte.                                                                                                                                                      |
---

## 🎓 Equipe

| Membro          |  Função                      |
| :-------------: | :--------------------------: |
| Caio Damaceno   | Product Owner & Scrum Master |
| Giovani Algusto | Developer                    |
