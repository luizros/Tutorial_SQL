## DQL - DATA DEFINITION LANGUAGE

Este comando é utilizado para criar, alterar e excluir bancos de dados, tabelas e elementros associados como índice e visão. 

CREATE - USADO PARA CRIAR BANCO DE DADOS, TABELA E OUTROS OBJETOS EM UM BANCO DE DADOS
ALTER  - USADO PARA ALTERAR A ESTRUTURA DE TABELAS OU OUTRO OBJETO EM UM BANDO DE DADOS
DROP   - USADO PARA APAGAR BANCO DE DADOS, TABELAS E OUTROS OBJETOS;

```sql
CREATE DATABASE financeiro
```
Aqui criamos um banco de dados chamado 'financeiro'

```sql
CREATE TABLE tipos_produto(codigo INT PRIMARY KEY, descricao, VARCHAR(50));
```
Teremos com o comando acima uma tabela com dois campos: codigo e descrição.

```sql
ALTER TABLE tipos_produto ADD peso DECIMAL(8,2);
```

Com o comando acima estamos criando mais um campo na tabela chamado 'peso'. 


```sql
DROP TABLE tipos_produto;
```
No exemplo acima estamos excluindo a tabela tipos_produto

```sql
DROP DATABASE financeiro;
```

No exemplo acima, excluímos o banco de dados 'financeiro' e qualquer tabela que ele possui.


