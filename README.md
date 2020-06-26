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

- A. time() + 60\*60\*100 Retorna a data e hora atuais mais uma hora
- B. time() + 24\*60\*60 Retorna a data e hora atuais mais um dia 
- C. time() + 24\*60\*60\*100 Retorna a data e hora atuais mais um dia

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

### Questão 4

Qual é a sintaxe javascript correta para alterar o conteúdo do elemento HTML abaixo?
```
<p id="demo">Isto é uma demonstração</p>
```
```
A. document.getElementByName("p").innerHTML = "Olá Mundo!";
B. document.getElementById("demo").innerHTML = "Olá Mundo!";
C. #demo.innerHTML = "Olá Mundo!";
D. document.getElement("p").innerHTML = "Olá Mundo!";
```

#### Resposta: 

```
B. document.getElementById("demo").innerHTML = "Olá Mundo!";
```

### Questão 5

O que o código javascript abaixo irá retornar no console do navegador, e por que?
```
var arr1 = "john".split('');
var arr2 = arr1.reverse();
var arr3 = "jones".split('');
arr2.push(arr3);
console.log("array 1: length=" + arr1.length + " last=" + arr1.slice(-1));
console.log("array 2: length=" + arr2.length + " last=" + arr2.slice(-1));
```

#### Resposta: 
