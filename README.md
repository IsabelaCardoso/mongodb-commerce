
# Habilidades
Neste projeto, foram testadas as habilidades:
  * Utilizar o método updateOne() e updateMany()
  * Utilizar os operadores $set , $mul , $inc , $min , $max e $currentDate
  * Renomear campos e remover campos
  * Incorporar dados aos documentos através de arrays
  * Utilizar os operadores $pop , $pull e $push 
  * Utilizar o operador $addToSet
  * Utilizar os operadores $each , $slice e $sort
  * Utilizar o operador $all para filtrar documentos
  * Utilizar o operador $elemMatch para filtrar documentos
  * Utilizar o operador $size para filtrar documentos pelo tamanho de arrays
  * Utilizar o operador $expr para criar expressões de agregação
  * Utilizar expressões regulares e o operador $regex para buscar documentos
  * Utilizar o índice textual e o operador $text
  * Utilizar o operador $mod

---

A ideia foi trabalhar com o banco de dados `commerce`, que contém dados do cardápio do **McDonald's**, como ingredientes, valores nutricionais e dados fictícios de vendas. 

##### Desafio 1

Inclua o campo `criadoPor` em todos os documentos, colocando `"Ronald McDonald"` no valor desse campo.

Para isso, escreva no arquivo `desafio1.js` duas queries, **nesta ordem**:

##### Desafio 2

Inclua o campo `valorUnitario` em todos os documentos em que esse campo não existe e atribua a ele o valor `"0.00"`, com o tipo `NumberDecimal`.

##### Desafio 3

Adicione o campo `avaliacao` em todos os documentos da coleção e efetue alterações nesse campo.

##### Desafio 4

Atribua a data corrente ao campo `ultimaModificacao` no sanduíche `Big Mac`.

##### Desafio 5

Adicione `ketchup` aos `ingredientes` para todos os sanduíches menos o `McChicken`, garantindo que não haja duplicidade nos `ingredientes`.

##### Desafio 6

Inclua `bacon` no final da lista de `ingredientes` dos sanduíches `Big Mac` e `Quarteirão com Queijo`.

##### Desafio 7

Remova o item `cebola` de todos os sanduíches.

##### Desafio 8

Remova o **primeiro** `ingrediente` do sanduíche `Quarteirão com Queijo`.

##### Desafio 9

Remova o **último** `ingrediente` do sanduíche `Cheddar McMelt`.

##### Desafio 10

Adicione a quantidade de vendas dos sanduíches por dia da semana.

Para isso, escreva no arquivo `desafio10.js` quatro queries, **nesta ordem**:

1. Crie uma query que inclua um _array_ com sete posições em todos os sanduíches. Cada uma delas representará um dia da semana, e cada posição iniciará em `0`. O _array_ deve se parecer como abaixo:
   ```json
   "vendasPorDia": [0, 0, 0, 0, 0, 0, 0]
   ```

- O primeiro item desse _array_ representa as vendas no **domingo**, o segundo item representa as vendas na **segunda-feira**, e assim até chegar ao último item, que representa as vendas no **sábado**.

2. Crie uma query que incremente as vendas de `Big Mac` às **quartas-feiras** em `60`.

3. Crie uma query que incremente as vendas de todos os sanduíches de carne do tipo `bovino` e `pão` aos **sábados** em `120`.

4. Crie uma query que retorne o `nome` e `vendasPorDia` de todos os documentos.

##### Desafio 11

Insira os elementos `combo` e `tasty` no _array_ `tags` de todos os sanduíches e aproveite para deixar os elementos em ordem alfabética ascendente.

##### Desafio 12

Ordene em todos os documentos os elementos do _array_ `valoresNutricionais` pelo campo `percentual` de forma descendente.

##### Desafio 13

Adicione o elemento `muito sódio` ao final do _array_ `tags` nos produtos em que o `percentual` de `sódio` seja maior ou igual a `40`.

##### Desafio 14

Adicione o elemento `contém sódio` ao final do _array_ `tags` nos produtos em que o `percentual` de `sódio` seja maior do que `20` e menor do que `40`.

##### Desafio 15

Conte quantos produtos contêm `Mc` no nome, sem considerar letras maiúsculas ou minúsculas.

##### Desafio 16

Conte quantos produtos têm `4` ingredientes.

##### Desafio 17

Conte quantos documentos contêm as palavras `frango` e `hamburguer` utilizando o operador `$text`.

##### Desafio 18

Conte quantos documentos contêm a **expressão** `feito com` utilizando o operador `$text`.

##### Desafio 19

Renomeie o campo `descricao` para `descricaoSite` em todos os documentos.

##### Desafio 20

Remova o campo `curtidas` do item `Big Mac`.

##### Desafio 21

Retorne o `nome` dos sanduíches em que o número de `curtidas` é maior que o número de sanduíches `vendidos`.

##### Desafio 22

Retorne o `nome` e a quantidade de vendas (`vendidos`) dos sanduíches em que o número de vendas é múltiplo de `5`.
