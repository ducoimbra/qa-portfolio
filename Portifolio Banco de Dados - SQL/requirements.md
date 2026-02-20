Requisitos e Regras de Negócio

Contexto do Sistema

Sistema de e-commerce onde usuários precisam se cadastrar para realizar compras.

O cadastro permite acesso à plataforma, realização de pedidos e acompanhamento de compras.



Regras Gerais do Sistema

1. Usuário deve possuir cadastro válido para realizar login.
2. Login é realizado utilizando email.
3. Email é utilizado para comunicação e recuperação de senha.
4. Status controla o acesso do usuário ao sistema.
5. Dados devem manter integridade e consistência.

Campos Obrigatórios

1. ID
 Deve ser único
 Não pode ser NULL
 Representa a chave primária da tabela

2. Nome
 Não pode ser NULL
 Utilizado para identificação do usuário na interface

3. Email
 Não pode ser NULL
 Deve ser único
 Utilizado para login e recuperação de senha

4. Status
 Não pode ser NULL
 Deve possuir valor válido (ativo, inativo, bloqueado)
 Controla o acesso do usuário ao sistema

5. Data de Cadastro
 Não pode ser NULL
 Utilizada para auditoria e controle


  Campos Opcionais

1. Idade
- Não é obrigatória
- Se informada, deve ser maior ou igual a 0

2. Telefone
- Opcional
- Se informado, deve seguir formato válido

3. Último Login
- Gerado automaticamente pelo sistema
- Pode ser NULL caso o usuário nunca tenha acessado


Critérios de Validação Aplicados

Durante a análise foram verificados:

Campos obrigatórios nulos
- Valores inválidos
- Inconsistência com regras definidas
- Possível impacto funcional no sistema
