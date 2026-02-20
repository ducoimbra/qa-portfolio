Descrição: Consultas utilizadas para identificar inconsistências


-- BUG ID-01: Email NULL

SELECT COUNT(*) AS total_email_null
FROM users
WHERE email IS NULL;

-- BUG ID-02: Idade inválida

SELECT COUNT(*) AS total_idade_invalida
FROM users
WHERE age <= 0;

-- BUG ID-03: Status NULL

SELECT COUNT(*) AS total_status_null
FROM users
WHERE status IS NULL;
