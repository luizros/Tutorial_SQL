## DCL - DATA TRANSACTION LANGUAGE

BEGIN 

COMIIT

ROLLBACK


```SQL
CREATE TABLE 'tipos_produto'(codigo INT PRIMARY KEY, descricao VARCHAR(50));
BEGIN TRANSACTION; --COMEÇAMOS A TRANSAÇÃO
    INSERT INTO tipos_produtoos VALUES('Notebook');
    INSERT INTO tipos_produtos  VALUES('Nobreak');
COMMIT; -- as inserções das linhas acima foram desfeitas
```

Aqui fazemos a transação e finalizamos com o commit

```SQL
CREATE TABLE 'tipos_produto'(codigo INT PRIMARY KEY, descricao VARCHAR(50));
BEGIN TRANSACTION; --COMEÇAMOS A TRANSAÇÃO
    INSERT INTO tipos_produtoos VALUES('Notebook');
    INSERT INTO tipos_produtos  VALUES('Nobreak');
COMMIT; -- as inserções das linhas acima foram desfeitas
```
Aqui desfazemos a operação anterior