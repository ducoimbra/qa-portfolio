BUG ID-01 — Email em Branco

Regra definida:
Email é obrigatório para login e comunicação.

Evidência:

81 registros com email NULL (conforme seu levantamento anterior).

Classificação
Tipo: Bug
Categoria: Validação de campo obrigatório
Severidade: Crítica

  Bug Report
Título: Sistema permite registro de usuário com email NULL

Ambiente: Banco de dados - tabela users

Passos para reproduzir:

Criar novo usuário

Não informar email

Salvar registro

  Resultado Atual:
Registro criado com campo email NULL
  Resultado Esperado:
Sistema deve impedir criação de usuário sem email
Impacto:
  Usuário não consegue realizar login nem recuperar senha

  BUG ID-02 — Idade negativa (-1 ou 0)
 Regra definida:
Idade não é obrigatória, mas se preenchida deve ser >= 0.
 Evidência:
31 registros com idade 0 ou -1.

  Classificação
Tipo: Bug
Categoria: Validação de regra de negócio
Severidade: Média

  Bug Report
  Título: Sistema aceita idade negativa ou inválida
  Passos:
Criar novo usuário
Informar idade -1
Salvar

  Resultado Atual:
Registro salvo com idade inválida
   Resultado Esperado:
Sistema deve bloquear idade menor que 0
  Impacto:
Relatórios demográficos incorretos

  BUG ID-03 — Status em Branco
  Regra definida:
Status é obrigatório e controla acesso.
  Evidência:
246 registros com status NULL.

  Classificação
Tipo: Bug
Categoria: Controle de acesso
Severidade: Alta

  Bug Report
  Título: Usuários cadastrados com status NULL
  Resultado Atual:
 Sistema permite cadastro sem definição de status
  Resultado Esperado:
 Campo status deve ser obrigatório e possuir valor padrão
  Impacto:
 Possível falha de controle de acesso


