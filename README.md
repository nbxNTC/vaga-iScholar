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
1 - var arr1 = "john".split('');
2 - var arr2 = arr1.reverse();
3 - var arr3 = "jones".split('');
4 - arr2.push(arr3);
5 - console.log("array 1: length=" + arr1.length + " last=" + arr1.slice(-1));
6 - console.log("array 2: length=" + arr2.length + " last=" + arr2.slice(-1));
```

#### Resposta: 
```
array 1: length=5 last=j,o,n,e,s
array 2: length=5 last=j,o,n,e,s
```
Os arrays 1 e 2 ficaram deste jeito
```
array 1: ["n", "h", "o", "j", Array(5)]
array 2: ["n", "h", "o", "j", Array(5)]
```
<p style='text-align: justify;'>
 Irá retornar os tamanhos dos arrays arr1 e arr2, que no caso é 5 para os dois e também 
 vai retornar a última posição de cada um destes arrays, que no caso é o próprio array  
 arr3 que foi inserido no final do arr1 e arr2 na linha 4. O arr3 foi inserido no final 
 do arr2, porém, por causa da linha 2, no qual o array 1 foi passado por referência para 
 o arr2, essa inserção ocorre no arr1 também.
</p>

