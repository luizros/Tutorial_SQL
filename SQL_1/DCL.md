## DCL - DATA CONTROL LANGUAGE

Este subgrupo controla os aspectos de autorização de dados e licenças de usuários para controlar quem tem acesso para manipular dados dentro do banco de dados.

GRANT - 
REVOKE

```SQL
GRANT SELECT ON tipos_produto TO geek;
```

No exemplo acima, estamos dando permissão de consulta na tabela tipos_produto para o usuario 'geek'.


```SQL
REVOKE CREAT TABLE FROM geek;
```

Estamos tirando a permissao de criação de tabelas no banco de dados do usuário 'geek'.