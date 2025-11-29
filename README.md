# Sistema_Academia
SOBRE O PROJETO:

Este repositório contém o desenvolvimento completo de um sistema de gestão de academia, incluindo:

-Modelagem conceitual (Minimundo)
-Modelo Entidade-Relacionamento (DER)
-Modelo lógico normalizado (1FN, 2FN e 3FN)
-Scripts SQL (DDL e DML)
-Testes de consultas SQL
-Operações completas de manipulação de dados (INSERT, SELECT, UPDATE, DELETE)
-Documentação do processo

O objetivo do projeto é demonstrar o ciclo completo de construção de um banco de dados relacional, do desenho conceitual até a implementação prática em SQL.

MINIMUNDO RESUMIDO

A academia precisa gerenciar:

-Alunos
-Professores
-Planos
-Contratos
-Pagamentos
-Treinos personalizados
-Exercícios
-Relação treino-exercício
-Check-ins dos alunos

O banco garante integridade, histórico completo e evita redundâncias.

Modelo Lógico – Visão Geral

Todas as tabelas foram normalizadas até 3FN, evitando duplicações e dependências parciais ou transitivas.

Entidades principais:

-ALUNO
-PROFESSOR
-PLANO
-CONTRATO
-PAGAMENTO
-TREINO
-EXERCICIO
-TREINO_EXERCICIO (N:N)
-CHECKIN

Tecnologias Utilizadas

MySQL Workbench

Configuração do Ambiente:
Arquivo: Sistema_Academia

Criação de tabelas:
Arquivo: CriacaoTabelas

Inserir dados:
Arquivo: InsertDados
