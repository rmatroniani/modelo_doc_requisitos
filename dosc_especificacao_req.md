# Especificação de Requisitos de Software (SRS)
## Nome do Projeto: Sistema de Gestão de Tarefas (SGT)
**Versão:** 1.0  
**Data:** 30/09/2026  
**Autor:** Equipe de Produto  

---

## 1. Introdução

### 1.1. Objetivo
Este documento descreve os requisitos funcionais e não funcionais para o desenvolvimento do **Sistema de Gestão de Tarefas (SGT)**, servindo como guia para desenvolvedores, testadores e gestores.

### 1.2. Escopo do Produto
O SGT é uma aplicação web que permite aos usuários criar, organizar, atribuir e acompanhar o progresso de tarefas diárias de forma colaborativa. 
* **O que está no escopo:** Cadastro de usuários, criação de quadros Kanban, envio de notificações por e-mail e relatórios de produtividade.
* **Fora do escopo:** Faturamento financeiro integrado e controle de ponto de funcionários.

---

## 2. Descrição Geral

### 2.1. Perspectiva do Sistema
O SGT é um sistema web independente, acessível via navegadores modernos, integrado a um serviço de autenticação externo e a um servidor de disparo de e-mails.

### 2.2. Perfis de Usuários
* **Administrador:** Gerencia usuários, permissões e configurações globais do sistema.
* **Usuário Comum:** Cria, edita e conclui suas próprias tarefas e participa de quadros compartilhados.

---

## 3. Requisitos Funcionais

* **[RF-001] Cadastro de Usuário**
  * **Descrição:** O sistema deve permitir que novos usuários criem uma conta informando nome, e-mail e senha.
  * **Prioridade:** Essencial
  * **Atores:** Visitante

* **[RF-002] Criação de Tarefas**
  * **Descrição:** O sistema deve permitir que o usuário autenticado crie uma nova tarefa com título, descrição, data de vencimento e nível de prioridade.
  * **Prioridade:** Essencial

* **[RF-003] Geração de Relatórios**
  * **Descrição:** O sistema deve exportar um relatório mensal de tarefas concluídas em formato PDF.
  * **Prioridade:** Importante

---

## 4. Requisitos Não Funcionais

* **[RNF-001] Desempenho**
  * **Descrição:** O tempo de resposta para carregamento das páginas principais não deve exceder 2 segundos sob condições normais de uso.
* **[RNF-002] Segurança**
  * **Descrição:** As senhas dos usuários devem ser armazenadas utilizando criptografia forte (ex: bcrypt).
* **[RNF-003] Disponibilidade**
  * **Descrição:** O sistema deve operar com disponibilidade de 99,9% ao longo do mês.
