# Index / Índice

- [English](#english)
  - [System Overview](#system-overview)
  - [Database Structure](#database-structure)
  - [SQL Files](#sql-files)
  - [Trigger Files](#trigger-files)
  - [Stored Procedure Files](#stored-procedure-files)

- [Português](#português)
  - [Visão Geral do Sistema](#visão-geral-do-sistema)
  - [Estrutura do Banco de Dados](#estrutura-do-banco-de-dados)
  - [Arquivos SQL](#arquivos-sql)
  - [Arquivos de Gatilho](#arquivos-de-gatilho)
  - [Arquivos de Procedimento Armazenado](#arquivos-de-procedimento-armazenado)

---

## English

<a name="english"></a>

## System Overview

This project is a user and subject management system that allows registering users, associating subjects with users, and performing basic authentication checks. The system is implemented using an Oracle database and includes the following components:

## Database Structure

### Tables

- `USERS`: Stores information about registered users.
- `SEMESTERS`: Stores information about semesters.
- `SUBJECTS`: Stores information about subjects.
- `USERS_SUBJECTS`: Association table between users and subjects.

### Sequences

- `USER_SEQUENCE`: Generates sequential values for the user IDs.
- `SEMESTER_SEQUENCE`: Generates sequential values for the semester IDs.

## SQL Files

- `01_create_tables.sql`: Creates the necessary tables in the database.
- `02_create_sequences.sql`: Creates the sequences to generate sequential values.
- `03_create_triggers.sql`: Creates the triggers to execute business logic.
- `04_create_procedures.sql`: Creates the stored procedures to perform specific operations.

## Trigger Files

- `triggers/trg_auto_sequence_id.sql`: Contains the SQL code for the `AUTO_SEQUENCE_USERS` trigger.
- `triggers/trg_capture_registration_date.sql`: Contains the SQL code for the `CAPTURE_REGISTRATION_DATE` trigger.
- `triggers/trg_basic_authentication_verification.sql`: Contains the SQL code for the `BASIC_AUTHENTICATION_VERIFICATION` trigger.

## Stored Procedure Files

- `procedures/prc_delete_relationship_user_subject.sql`: Contains the SQL code for the `DELETE_RELATIONSHIP_USER_SUBJECT` stored procedure.
- `procedures/prc_register_relationship_user_subject.sql`: Contains the SQL code for the `REGISTER_RELATIONSHIP_USER_SUBJECT` stored procedure.

---

## Português

<a name="português"></a>

## Visão Geral do Sistema

Este projeto é um sistema de gerenciamento de usuários e matérias que permite registrar usuários, associar matérias aos usuários e realizar verificações básicas de autenticação. O sistema é implementado usando um banco de dados Oracle e inclui os seguintes componentes:

## Estrutura do Banco de Dados

### Tabelas

- `USERS`: Armazena informações sobre os usuários registrados.
- `SEMESTERS`: Armazena informações sobre os semestres.
- `SUBJECTS`: Armazena informações sobre as matérias.
- `USERS_SUBJECTS`: Tabela de associação entre usuários e matérias.

### Sequências

- `USER_SEQUENCE`: Gera valores sequenciais para os IDs de usuário.
- `SEMESTER_SEQUENCE`: Gera valores sequenciais para os IDs de semestre.

## Arquivos SQL

- `01_create_tables.sql`: Cria as tabelas necessárias no banco de dados.
- `02_create_sequences.sql`: Cria as sequências para gerar valores sequenciais.
- `03_create_triggers.sql`: Cria os gatilhos para executar a lógica de negócio.
- `04_create_procedures.sql`: Cria os procedimentos armazenados para realizar operações específicas.

## Arquivos de Gatilho

- `triggers/trg_auto_sequence_id.sql`: Contém o código SQL para o gatilho `AUTO_SEQUENCE_USERS`.
- `triggers/trg_capture_registration_date.sql`: Contém o código SQL para o gatilho `CAPTURE_REGISTRATION_DATE`.
- `triggers/trg_basic_authentication_verification.sql`: Contém o código SQL para o gatilho `BASIC_AUTHENTICATION_VERIFICATION`.

## Arquivos de Procedimento Armazenado

- `procedures/prc_delete_relationship_user_subject.sql`: Contém o código SQL para o procedimento armazenado `DELETE_RELATIONSHIP_USER_SUBJECT`.
- `procedures/prc_register_relationship_user_subject.sql`: Contém o código SQL para o procedimento armazenado `REGISTER_RELATIONSHIP_USER_SUBJECT`.

---
