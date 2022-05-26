# 	:woman_technologist: Project Docker Todo List

Esse projeto contém uma série de informações sobre o que eu aprendi aqui na Trybe ao longo  do curso de desenvolvimento web da Trybe. <br>
Esse projeto contém uma série de desafios com diferentes níveis de complexidade que devem ser resolvidos cada um em seu arquivo próprio, usando query de MySQL.

## :rocket:Começando
Esse projeto foi proposto pelo curso de desenvolvimento web da Trybe.
### Desenvolvimento
Esse proejto foi desenvolvido no bloco de back-end, usei query de MySQL.
### Commits
Os commits foram feitos de acordo grupo de arquivos de testes: filteringChallenges.spec, initialChallenges.spec e tableManipulationChallenges.spec.
### Branch
Todo o projeto foi feita na branch 'juliana-oliveira-project-all-for-one', isso por conta da exigência do curso.
### Instalação
Antes de realizar o projeto, precisei instalar as dependências usando npm install, dentro do container. Usei o comando docker exec -it all_for_one bash, depois dei npm install.
### Testes
Os testes usando foram feitos através dos **comandos**, feitos dentro do container docker: <br>
* Primeiro fiz docker exec -it all_for_one bash
* Depois fiz npm test
### Autores
Esse foi um projeto individual,que desenvolvido somente por Juliana Oliveira.
### Ferramentas usadas
Foi usado Visual Studio Code, além do Trello que auxiliou na organização das tarefas.
### Framework usado
Nenhum.
### Banco de Dados
O banco de dados usado foi o northwind, que pode ser copiado através desse arquivo:<br>
https://github.com/jsfoliveira/Project-All-For-One/blob/juliana-oliveira-project-all-for-one/northwind.sql
### Informações Importantes
Na raiz do projeto, foram criados os arquivos desafio1.sql até desafio27.sql. Nele contém todas as querys que serão usadas nos testes. Para fazer todos os arquivos de uma vez só, usei o seguinte comando:
* touch desafio{1..27}.sql
<br>
**Não é necessário colocar no início dos arquivos** `USE northwind` ou `SET SQL_SAFE_UPDATES = 0;` <br>
Após a execução dos teste locais, o banco de dados `northwind` é deletado.<br>
Antes de começar, seu docker-compose precisa estar na versão 1.29 ou superior. 

## :footprints:Requisitos
### Metodologia usada
No trabalho do desenvolvimento de software a gente sempre tem prazos, muitas vezes os prazos são apertados.<br>
Por outro lado, eu não quero criar algo que não entendo perfeitamente, como também fazer códigos rápidos pode levar a erros que podem demorar muito pra corrigir.<br>
Por isso, usei e sempre uso o método Baby Steps, que é uma estratégia de abordar o desafio passo à passo, defensivamente.<br>
Baby steps é um termo em inglês que quer dizer passos de bebê. Refere-se a fazer as coisas, quaisquer que sejam, devagar, com calma, passo a passo.
#### :footprints:Requisito 1-  Exiba apenas os nomes dos produtos na tabela `products`.

  ---
  
#### :footprints:Requisito 2 - Exiba os dados de todas as colunas da tabela `products`.

  ---
  
#### :footprints:Requisito 3 - Escreva uma query que exiba os valores da coluna que representa a primary key da tabela `products`.

  ---
  
#### :footprints:Requisito 4 - Conte quantos registros existem na coluna `product_name` da tabela `products`.

  ---
  
#### :footprints:Requisito 5 - Monte uma query que exiba os dados da tabela `products` a partir do quarto registro até o décimo terceiro.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Tanto o quarto quanto o décimo terceiro registros, precisam aparecer na consulta;

  - Não use `where` ou `order by`.

  <br />
</details>

  ---
  
#### :footprints:Requisito 6 - Exiba os dados das colunas `product_name` e `id` da tabela `products` de maneira que os resultados estejam em ordem alfabética dos nomes.

  ---
  
#### :footprints:Requisito 7 - Mostre apenas os ids dos 5 últimos registros da tabela `products` (a ordernação deve ser baseada na coluna `id`).

  ---
  
#### :footprints:Requisito 8 - Faça uma consulta que retorne três colunas, respectivamente, com os nomes 'A', 'Trybe' e 'eh', e com valores referentes a soma de '5 + 6', a string 'de', a soma de '2 + 8'.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Na primeira coluna, exiba a soma de `5 + 6` (essa soma deve ser realizada pelo SQL);
  
  - Na segunda coluna deve haver a palavra \"de\";
  
  - E por fim, na terceira coluna, exiba a soma de `2 + 8` (essa soma deve ser realizada pelo SQL);
  
  - A primeira coluna deve se chamar \"A\", a segunda coluna deve se chamar \"Trybe\" e a terceira coluna deve se chamar \"eh\";
  
  - Não use colunas pré-existentes, apenas o que for criado na hora.

  <br />
</details>

## Desafios sobre filtragem de dados

#### :footprints:Requisito 9 - Mostre todos os valores de `notes` da tabela `purchase_orders` que não são nulos.

  ---
  
#### :footprints:Requisito 10 - Mostre todos os dados da tabela `purchase_orders` em ordem decrescente, ordenados por `created_by` em que o `created_by` é maior ou igual a 3.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Como critério de desempate para a ordenação, ordene também os resultados pelo `id` de forma crescente.

  <br />
</details>

  ---
  
#### :footprints:Requisito 11 - Exiba os dados da coluna `notes` da tabela `purchase_orders` em que seu valor de `Purchase generated based on Order` é maior ou igual a 30 e menor ou igual a 39.

  ---
  
#### :footprints:Requisito 12 - Mostre as `submitted_date` de `purchase_orders` em que a `submitted_date` é do dia 26 de abril de 2006.

  ---
  
#### :footprints:Requisito 13 - Mostre o `supplier_id` das `purchase_orders` em que o `supplier_id` seja 1 ou 3.

  ---
  
#### :footprints:Requisito 14 - Mostre os resultados da coluna `supplier_id` da tabela `purchase_orders` em que o `supplier_id` seja maior ou igual a 1 e menor ou igual 3.

  ---
  
#### :footprints:Requisito 15 - Mostre somente as horas (sem os minutos e os segundos) da coluna `submitted_date` de todos registros da tabela `purchase_orders`.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Chame essa coluna de `submitted_hour`.

  <br />
</details>

  ---
  
#### :footprints:Requisito 16 - Exiba a `submitted_date` das `purchase_orders` que estão entre `2006-01-26 00:00:00` e `2006-03-31 23:59:59`.

  ---
  
#### :footprints:Requisito 17 - Mostre os registros das colunas `id` e `supplier_id` das `purchase_orders` em que os `supplier_id` sejam tanto 1, ou 3, ou 5, ou 7.

  ---
  
#### :footprints:Requisito 18 - Mostre todos os registros de `purchase_orders` que tem o `supplier_id` igual a 3 e `status_id` igual a 2.

  ---
  
#### :footprints:Requisito 19 - Mostre a quantidade de pedidos que foram feitos na tabela `orders` pelo `employee_id` igual a 5 ou 6, e que foram enviados através do método(coluna) `shipper_id` igual a 2.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary><br />

  - Chame a coluna de `orders_count`.

  <br />
</details>

  ---
  
## Desafios de manipulação de tabelas

#### :footprints:Requisito 20 - Adicione à tabela `order_details` um registro com `order_id`: 69, `product_id`: 80, `quantity`: 15.0000, `unit_price`: 15.0000, `discount`: 0, `status_id`: 2, `date_allocated`: NULL, `purchase_order_id`: NULL e `inventory_id`: 129.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Obs.: o `id` deve ser incrementado automaticamente.

  <br />
</details>

  ---
  
#### :footprints:Requisito 21 - Adicione com um único `INSERT`, duas linhas à tabela `order_details` com os mesmos dados do requisito 20.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Esses dados são novamente `order_id`: 69, `product_id`: 80, `quantity`: 15.0000, `unit_price`: 15.0000, `discount`: 0, `status_id`: 2, `date_allocated`: NULL, `purchase_order_id`: NULL e `inventory_id`: 129;
  
  - O `ìd` deve ser incrementado automaticamente.

  <br />
</details>

  ---
  
#### :footprints:Requisito 22 - Atualize os dados de `discount` do `order_details` para 15. (Não é necessário utilizar o SAFE UPDATE em sua query).

  ---
  
#### :footprints:Requisito 23 - Atualize os dados da coluna `discount` da tabela `order_details` para 30, onde o valor na coluna `unit_price` seja menor que 10.0000.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Não é necessário utilizar o SAFE UPDATE em sua query.

  <br />
</details>

  ---
  
#### :footprints:Requisito 24 - Atualize os dados da coluna `discount` da tabela `order_details` para 45, onde o valor na coluna `unit_price` seja maior que 10.0000 e o id seja um número entre 30 e 40.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Não é necessário utilizar o SAFE UPDATE em sua query.

  <br />
</details>

  ---
  
#### :footprints:Requisito 25 - Delete todos os dados em que a `unit_price` da tabela `order_details` seja menor que 10.0000.

  ---
  
#### :footprints:Requisito 26 - Delete todos os dados em que a `unit_price` da tabela `order_details` seja maior que 10.0000.

  ---
  
#### :footprints:Requisito 27 - Delete todos os dados da tabela `order_details`.

---
