Validação de Banco de Dados - E-commerce

 Visão Geral do Projeto

Este projeto tem como objetivo realizar a validação de integridade de dados em um sistema de e-commerce utilizando SQL.

A proposta é simular um cenário real de teste de banco de dados (Database Testing), identificando inconsistências, validando regras de negócio e documentando os problemas encontrados de forma estruturada.

A base analisada contém 1000 registros de usuários.


Objetivo

Simular um processo real de QA validando:

- Campos obrigatórios e opcionais
- Valores nulos (NULL)
- Valores inválidos
- Integridade dos dados
- Impacto funcional das inconsistências
- Classificação de severidade
- Documentação formal de bugs


 Contexto do Sistema (Cenário Assumido)

Sistema de e-commerce onde:

- Usuário precisa se cadastrar para realizar compras
- Login é realizado via email
- Email é utilizado para comunicação e recuperação de senha
- Status controla o acesso do usuário ao sistema
- Idade é utilizada para análise demográfica
- Telefone é opcional para contato


 Campos Obrigatórios

- ID (Chave Primária – único e não pode ser NULL)
- Nome
- Email (único e obrigatório)
- Status
- Data de Cadastro



 Campos Opcionais

- Idade (se informada, deve ser ≥ 0)
- Telefone
- Último Login (gerado automaticamente pelo sistema)
- 

 Escopo da Validação

Foram realizadas consultas SQL para verificar:

- Registros com campos obrigatórios nulos
- Valores inválidos (ex: idade negativa)
- Inconsistências relacionadas às regras definidas
- Possível impacto no fluxo do sistema



 Ferramentas Utilizadas

- SQL
- Planilha para análise auxiliar
- Documentação estruturada em Markdown



 Principais Inconsistências Identificadas

- Usuários com email NULL (Impacto crítico – login e recuperação de senha)
- Usuários com idade negativa ou inválida (Falha de validação)
- Usuários com status NULL (Risco de controle de acesso)

Os detalhes completos estão documentados no arquivo `bug_reports.md`.


 Competências Demonstradas

- Teste de banco de dados
- Análise de integridade de dados
- Definição e validação de regras de negócio
- Classificação de severidade
- Elaboração de bug reports
- Pensamento crítico aplicado a QA


 Finalidade

Este projeto demonstra a aplicação prática de técnicas de QA voltadas para validação de dados, indo além da execução de consultas SQL e focando na análise estruturada e documentação profissional de inconsistências.
