# 🚀 Escalas e Ponto DevOps

Sistema web para gerenciamento de escalas de trabalho, funcionários e controle de ponto eletrônico, desenvolvido como parte do Projeto de Extensão em Desenvolvimento de Software da Universidade Nove de Julho (UNINOVE).

O projeto foi construído utilizando conceitos de **DevOps, Infraestrutura como Código (IaC) e arquitetura de software em três camadas**, buscando oferecer uma aplicação organizada, modular e portátil entre diferentes ambientes.

## 🎯 Objetivo do projeto

Desenvolver uma solução para simplificar o gerenciamento de jornadas de trabalho, automatizar a distribuição de escalas e facilitar o acompanhamento dos registros de ponto dos colaboradores.

## ⚙️ Funcionalidades

- **Dashboard administrativo:** visualização de indicadores e informações gerais do sistema.
- **Gestão de funcionários:** cadastro, consulta, edição e exclusão de colaboradores (CRUD).
- **Gerenciamento de escalas:** distribuição automatizada de turnos e visualização em calendário mensal.
- **Ponto eletrônico:** registro de entrada, saída para intervalo, retorno do intervalo e saída definitiva.
- **Super Punch:** acompanhamento semanal das marcações de ponto.
- **Relatórios:** consolidação de horas trabalhadas e informações para fechamento de folha.
- **Controle de acesso (RBAC):** permissões diferenciadas para administradores e funcionários.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Aplicação |
|---|---|
| HTML5 | Estrutura da aplicação |
| CSS3 | Estilização e responsividade |
| JavaScript | Interatividade e funcionalidades |
| PHP 8.2 | Lógica de negócio e backend |
| MySQL 8 | Banco de dados |
| Docker | Containerização |
| Docker Compose | Orquestração dos containers |

## 🏗️ Arquitetura

O sistema utiliza uma arquitetura cliente-servidor dividida em três camadas:

1. **Frontend:** interface desenvolvida com HTML5, CSS3 e JavaScript.
2. **Backend:** processamento das regras de negócio utilizando PHP 8.2.
3. **Banco de dados:** persistência e integridade dos registros utilizando MySQL 8.

### 🐳 Infraestrutura com Docker

A aplicação utiliza Docker Compose para orquestrar dois serviços principais:

- **Web:** PHP 8.2 com servidor Apache.
- **Database:** MySQL 8.

Mapeamento de portas:

- Aplicação Web: `localhost:8080`
- Banco de dados: `localhost:3307`

Essa estrutura permite executar os serviços em containers isolados, facilitando a configuração e a portabilidade do ambiente.

## 📁 Estrutura do projeto

```text
escalas-ponto-devops/
│
├── demo_app/
│   ├── config.php
│   ├── dashboard.php
│   ├── funcionarios.php
│   ├── escalas.php
│   ├── ponto.php
│   ├── relatorios.php
│   ├── style.css
│   └── script.js
│
├── schema_mysql_escalas_e_ponto.sql
└── docker-compose.php.yml
```

## 🔐 Segurança e permissões

O sistema implementa controle de acesso baseado em funções (RBAC):

- **Administrador:** gerenciamento de funcionários, escalas e relatórios.
- **Funcionário:** acesso ao próprio registro de ponto e calendário individual de trabalho.

## 📚 Aprendizados

Durante o desenvolvimento, tivemos contato com conceitos importantes de:

- Desenvolvimento Full Stack.
- Arquitetura de software.
- Modelagem e gerenciamento de banco de dados.
- Containerização com Docker.
- Infraestrutura como Código (IaC).
- DevOps e organização de ambientes.
- Controle de acesso e segurança de aplicações.

## 👥 Equipe de desenvolvimento

Projeto acadêmico desenvolvido em equipe na Universidade Nove de Julho (UNINOVE).

- Luana Dias da Silva Sacutti
- Maria Eduarda Ferraz Silva
- Guilherme Almeida da Silva

## 🎓 Instituição

Universidade Nove de Julho (UNINOVE)

Projeto de Extensão em Desenvolvimento de Software.

---

**Desenvolvido para fins acadêmicos e educacionais.**
