## DQL - DATA QUERY LANGUAGE

No subgrupo DQL temos apenas 1 comando SQL: Select

Este comando é utilizado para realizar consulta no banco de dados

tipos_produto

|Código  |Descrição  |
|---------|---------|
|1     |    Computador     |
|2     |    Impressora     |


```sql
SELECT * FROM tipos_produto
```
Neste exemplo acima, estamos selecionando todos os dados da tabela 'tipos_produto'. O asterisco indica que quermos os dados de todos os campos da tabela.

Outra forma de executar o mesmo comando


```sql
SELECT código, descrição * FROM tipos_produto
```
Aqui estamos trazendo as colunas código e descrição da tabela tipos_produto.  

Podemos também fazer um apelido para cada campo da tabela


```sql
SELECT tp.código AS cd, tp.descrição AS descr * FROM tp.tipos_produto
```
Será retornado uma tabela com os campos modificados conforme o nome dado para os apelidos. 


```sql
SELECT tp.código AS cd, tp.descrição AS descr * FROM tp.tipos_produto
```