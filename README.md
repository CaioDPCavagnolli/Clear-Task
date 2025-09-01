<img width="500" height="300" alt="Logo Empresa" src="https://github.com/user-attachments/assets/d149f69b-cad5-46eb-8bb7-35b0443278bb" />

# Clear Task - Sistema de Gerenciamento de Chamados com IA Integrada

**Clear Task** é uma plataforma inteligente de gerenciamento de chamados que funciona em **desktop**, **web** e **mobile**. Utilizando **Electron**, **JavaScript**, **TypeScript** e a IA **Copilot**, o sistema visa otimizar o processo de resolução de problemas e melhorar a experiência do usuário através de automações, categorização inteligente e respostas automatizadas.

## 📝 Índice

- [Visão Geral](#visão-geral)
- [Funcionalidades](#funcionalidades)
- [Tecnologias](#tecnologias)
- [Instalação](#instalação)
- [Uso](#uso)
- [Arquitetura](#arquitetura)
- [Diagramas UML](#diagramas-uml)
- [Contribuição](#contribuição)
- [Licença](#licença)

---

## 🏅 Desafio
Desenvolver um sistema web de Help Desk de chamados, com controle de acesso baseado em três níveis hierárquicos:

**Supervisor:** pode abrir chamados e direcioná-los para técnicos específicos.

**Técnico:** pode editar os chamados atribuídos, ajustando prioridade, categoria e localização.

**Administrador:** possui acesso total ao sistema, incluindo a criação e gestão de contas de usuários, além de visualizar e editar todos os chamados.

O sistema deve registrar o histórico completo dos chamados, permitir filtros por status e categorias, e garantir segurança e rastreabilidade das ações realizadas por cada perfil. Todas as interações devem ser persistidas em banco de dados para auditoria e melhoria contínua dos processos de atendimento.

## 🏅 Solução
O Clear HelpDesk será uma plataforma inteligente e escalável para gestão de chamados técnicos, com foco em agilidade, organização e controle operacional. Supervisores poderão registrar demandas diretamente para os técnicos, que terão autonomia para atualizar os chamados com informações relevantes. O administrador atuará como gestor do sistema, garantindo a integridade dos dados e o funcionamento adequado da plataforma.

A solução será construída com boas práticas de desenvolvimento web, autenticação segura, controle de permissões por perfil e banco de dados relacional. Essa abordagem visa melhorar o fluxo de atendimento interno, reduzir o tempo de resposta e oferecer uma visão clara da operação para todos os envolvidos.

---

## 📋 Backlog do Produto
[Backlog do Produto](https://github.com/CaioDPCavagnolli/Clear-Task/blob/main/Documenta%C3%A7%C3%A3o/BackLog%20do%20Produto.md)

---

### 🚀 Critérios para DoR

* User Stories com **Critérios de Aceitação**
* Subtarefas divididas **a partir das US**
* Design no **Figma**
* Modelagem do **Banco de Dados**
* Diagrama de **Casos de Uso**
* Diagrama de **Classes do Sistema**
* Diagrama de **Iteração e Sequencia**

### ✅ DoD - Definition of Done

* Manual de Usuário
* Manual da Aplicação
* Documentação da API (Application Programming Interface)

---

## 🚀 Visão Geral

O **Clear Task** foi desenvolvido para automatizar o gerenciamento de chamados, oferecendo uma solução multiplataforma (desktop, web e mobile). A IA integrada (Copilot) facilita a triagem, priorização e resposta de chamados, com aprendizado contínuo para aprimorar as soluções oferecidas.

- **Desktop:** Construído com **C#** para criar uma aplicação de desktop nativa para Windows, macOS e Linux.
- **Web:** Uma versão web responsiva, acessível via navegador em qualquer dispositivo.
- **Mobile:** Aplicação móvel disponível para **Android** oferecendo uma experiência otimizada para dispositivos móveis.

## ⚙️ Funcionalidades

- **Interface Multiplataforma:** A aplicação é acessível em desktop, web e dispositivos móveis.
- **Inteligência Artificial Copilot:** Classificação, priorização e sugestão automática de soluções com base em IA.
- **Gerenciamento de Chamados:** Criação, visualização, edição e resolução de chamados com possibilidade de adicionar notas, arquivos e anexos.
- **Notificações em Tempo Real:** Receba alertas e atualizações instantâneas sobre novos chamados e mudanças no status.
- **Suporte Multiplataforma:** Experiência integrada entre desktop, web e mobile, com dados sincronizados em tempo real.
- **Autenticação e Gestão de Usuários:** Suporte para múltiplos perfis e autenticação via JWT.

## 🔧 Tecnologias

O **Clear Task** é desenvolvido com as seguintes tecnologias:

- **Frontend (Desktop & Web):** Electron, React, TypeScript, JavaScript
- **Mobile:** React Native (para Android e iOS)
- **Backend:** Node.js, Express (API RESTful)
- **Banco de Dados:** (Em fase de escolha, informações serão atualizadas em breve)
- **IA:** Copilot (para automação e sugestões inteligentes)
- **Autenticação:** JWT (JSON Web Token)
- **Gerenciamento de Dependências:** npm, yarn
