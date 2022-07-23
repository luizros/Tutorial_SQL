## DQL - DATA MANIPULATION LANGUAGE

Este comando é utilizado para realizar inclusões de registros, atualizações de registros ou remover registros.


```sql
INSERT INTO tipos_produto(descricao) values('Notebook');
```

Neste exemplo estou inserindo o valor 'Notebook' na tabela 'tipos_produto' no campo descrição. 

tipos_produto ANTES

|Código  |Descrição  |
|---------|---------|
|1     |    Computador     |
|2     |    Impressora     |


tipos_produto DEPOIS

|Código  |Descrição  |
|---------|---------|
|1     |    Computador     |
|2     |    Impressora     |
|3     |    Notebook     |


Outra dorma de fazer o comando

```sql
INSERT INTO produtos(descricao, preco, codigo_do_tipo) values('Notebook Samsung', 4000,1);
```

tabela_produtos ANTES
|Código  |Descrição  |Preco|CodigoDoTipo|
|---------|---------|---------|---------|
|1        |Computador|1800    |    1    |
|2     |    Impressora     |300|2|
|3     |    Notebook Acer    |500|1|
|4     |Impressora Lazer|1900|2|


tabela_produtos DEPOIS
|Código  |Descrição  |Preco|CodigoDoTipo|
|---------|---------|---------|---------|
|1        |Computador|1800    |    1    |
|2     |    Impressora     |300|2|
|3     |    Notebook Acer    |500|1|
|4     |Impressora Lazer|1900|2|
|5     |Notebook Samsung|4000|1|

Existem também comando para atualizar nossa tabela


```sql
UPDATE tipos_produto set descricao = 'Nobreak' WHERE codigo = 3;
```
tipos_produto DEPOIS
|Código  |Descrição  |
|---------|---------|
|1     |    Computador     |
|2     |    Impressora     |
|3     |    Nobreak      |

O campo só infomamos uma única vez, exemplo:


```sql
UPDATE produtos set descricao = 'Nobreak', preco = 2.800 = WHERE codigo = 20;
```

Onde o código é igual a 20 alteramos o valor dos campos especificados da tabela produtos. 


Para deletar registros

```sql
DELETE FROM tipos_produto WHERE codigo = 3;
```
Este comando deleta a linha onde o codigo é zero.


