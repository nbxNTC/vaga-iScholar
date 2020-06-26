# Processo Seletivo iScholar
 
## Atividade 1

Todos os arquivos pedidos estão na pasta Atividade 1.

## Atividade 2

### Questão 1

Considere o seguinte pedaço de código
```
<?php
 $arr = array(3 => "Primeiro", 2 => "Segundo", 1 => "Terceiro");
 list (, $result) = $arr;
?>
```
Depois de rodá-lo, o valor de $result deverá ser

#### Resposta: 

C. Terceiro

### Questão 2

Quais das instruções a seguir estão corretas? 

- A. time() + 60*60*100 Retorna a data e hora atuais mais uma hora
- B. time() + 24*60*60 Retorna a data e hora atuais mais um dia 
- C. time() + 24*60*60*100 Retorna a data e hora atuais mais um dia

#### Resposta: 

B

### Questão 3

Dada as seguintes tabelas

```
sql> SELECT * FROM runners;
+----+--------------+
| id | name         |
+----+--------------+
|  1 | John Doe     |
|  2 | Jane Doe     |
|  3 | Alice Jones  |
|  4 | Bobby Louis  |
|  5 | Lisa Romero  |
+----+--------------+

sql> SELECT * FROM races;
+----+----------------+-----------+
| id | event          | winner_id |
+----+----------------+-----------+
|  1 | 100 meter dash |  2        |
|  2 | 500 meter dash |  3        |
|  3 | cross-country  |  2        |
|  4 | triathalon     |  NULL     |
+----+----------------+-----------+
```
Qual será o resultado da consulta abaixo?

```
SELECT * FROM runners WHERE id NOT IN (SELECT winner_id FROM races)
```

#### Resposta: 

```
+----+--------------+
| id | name         |
+----+--------------+
|  1 | John Doe     |
|  4 | Bobby Louis  |
|  5 | Lisa Romero  |
+----+--------------+
```
