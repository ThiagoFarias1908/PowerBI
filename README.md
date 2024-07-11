# Power BI

## Descrição
Repositório para armazenar estudos e projetos em Power BI.

## Estrutura
- **Medidas:** Documentação das medidas DAX.
- **Datasets:** Conjunto de dados utilizados nos projetos.
- **Projetos:** Projetos ou estudos de caso que envolvem a aplicação prática de Power BI em cenários mais realistas.

## Medidas
1. [Sales](Medidas/01%20Sales.md): Calcula o total das vendas.
2. [Sales AVG](Medidas/02%20Sales%20AVG.md): Calcula a média das vendas.
3. [Orders Quantity](Medidas/03%20Orders%20Quantity.md): Conta o número total de pedidos.
4. [Distinct Orders Quantity](Medidas/04%20Distinct%20Orders%20Quantity.md): Calcula a quantidade distinta de pedidos.
5. [Sales AVG com Divide](Medidas/05%20Sales%20AVG%20com%20Divide.md): Calcula a média das vendas utilizando a função DIVIDE para evitar divisão por zero.
6. [Sales AVGX](Medidas/06%20Sales%20AVGX.md): Calcula a média ponderada das vendas utilizando a função AVERAGEX, considerando apenas valores de receita maiores que zero.
7. [Sales SUMX](Medidas/07%20Sales%20SUMX.md): Calcula o total de vendas usando a função SUMX.
8. [Orders Quantity with revenue < 0](Medidas/08%20Orders%20Quantity%20with%20revenue%20<%200.md): Calcula a quantidade de pedidos com receita menor que zero.
9. [CALCULATE + ALL](Medidas/09%20CALCULATE%20%2B%20ALL.md): Calcula a receita líquida total das categorias.
10. [Porcetagem Categoria](Medidas/10%20Porcetagem%20Categoria.md): Calcula a porcentagem de vendas por categoria.
11. [Porcetagem Ano](Medidas/11%20Porcentagem%20Ano.md): Calcula a porcentagem de vendas em relação ao ano.
12. [Sales Total Category](Medidas/12%20Sales%20Total%20Category.md): Calcula o total de vendas por categoria de produto.
13. [Sales Category %](Medidas/13%20Sales%20Category%20%25.md): Calcula a porcentagem de vendas por categoria em relação ao total de vendas.
14. [Sales Total Category ALLSELECTED](Medidas/14%20Sales%20Total%20Category%20ALLSELECTED.md): Calcula o total de vendas por categoria, considerando a seleção feita no relatório (ALLSELECTED).
15. [Sales Category ALLSELECTED %](Medidas/15%20Sales%20Category%20ALLSELECTED%20%25.md): Calcula a porcentagem das vendas por categoria, considerando o contexto de seleção atual utilizando a função ALLSELECTED.
16. [Sales Total Material ALL](Medidas/16%20Sales%20Total%20Material%20ALL.md): Calcula o total de vendas de materiais, ignorando qualquer filtro aplicado.
17. [Sales Total Material ALL %](Medidas/17%20Sales%20Total%20Material%20ALL%20%25.md): Calcula o percentual das vendas totais de materiais em relação ao total geral das vendas, independentemente de quaisquer filtros aplicados.
18. [Sales Total CA06](Medidas/18%20Sales%20Total%20CA06.md): Calcula o total das vendas para a categoria CA06.
19. [Sales Category Diff.](Medidas/19%20Sales%20Category%20Diff.md): Calcula a diferença entre as vendas de duas categorias específicas.
20. [Sales Total CA06 V2](Medidas/20%20Sales%20Total%20CA06%20V2.md): Calcula o total das vendas para a categoria CA06 de outra maneira.
21. [Sales Sorocaba](Medidas/21%20Sales%20Sorocaba.md): Calcula o total das vendas realizadas na cidade de Sorocaba.
22. [Performance AVGX](Medidas/22%20Performance%20AVGX.md): Calcula a performance média das entregas com base na data de entrega.
23. [ADDCOLUMNS](Medidas/23%20ADDCOLUMNS.md): Adiciona uma coluna calculada, que calcula a média de lucro para cada mês.
24. [CROSSJOIN](Medidas/24%20CROSSJOIN.md): Calcula a média de lucro das vendas por mês e ano.
25. [SUMMARIZE](Medidas/25%20SUMMARIZE.md): Cria uma tabela resumida que calcula o média de lucro das vendas por mês e ano.
26. [ADDCOLUMNS + SUMMARIZE](Medidas/26%20ADDCOLUMNS%20%2B%20SUMMARIZE.md): Calcula a média de vendas por mês e ano.
27. [Variáveis com um valor](Medidas/27%20Variáveis%20com%20um%20valor.md): Cria duas variáveis que retornam a soma do ano e do mês máximos.
28. [Variáveis com tabela](Medidas/28%20Variáveis%20com%20tabela.md): Cria uma variável que encontra o ano máximo entre os anos únicos da tabela.
29. [Variáveis com tabela V2](Medidas/29%20Variáveis%20com%20tabela%20V2.md): Cria uma variável que calcula a média das vendas para os anos e meses abreviados na tabela.
30. [SELECTEDVALUE YEAR](Medidas/30%20SELECTEDVALUE%20YEAR.md): Cria uma variável que calcula o ano máximo presente na coluna e retorna o valor do ano selecionado.
31. [USERELATIONSHIP Orders delivered quantity](Medidas/31%20USERELATIONSHIP%20Orders%20delivered%20quantity.md): Calcula a quantidade de pedidos entregues usando o relacionamento especificado entre as tabelas.

## Medidas Inteligência Temporal
1. [Sales](Medidas%20Inteligência%20Temporal/01%20Sales.md): Calcula o total das vendas.
2. [Sales Last Month](Medidas%20Inteligência%20Temporal/02%20Sales%20Last%20Month.md): Calcula o total de vendas do mês anterior.
3. [Sales Last Month Delta](Medidas%20Inteligência%20Temporal/03%20Sales%20Last%20Month%20Delta.md): Calcula a diferença entre as vendas do mês atual e as vendas do mês anterior.
4. [Sales Last Month Delta %](Medidas%20Inteligência%20Temporal/04%20Sales%20Last%20Month%20Delta%20%25.md): Calcula a variação percentual das vendas em relação ao mês anterior.
5. [Sales Month over Month](Medidas%20Inteligência%20Temporal/05%20Sales%20Month%20over%20Month.md): Calcula o total de vendas do mesmo mês no ano anterior.
6. [Sales Month over Month Delta](Medidas%20Inteligência%20Temporal/06%20Sales%20Month%20over%20Month%20Delta.md): Calcula a diferença entre as vendas do mês atual e as vendas do mesmo mês no ano anterior.
7. [Sales Month over Month Delta %](Medidas%20Inteligência%20Temporal/07%20Sales%20Month%20over%20Month%20Delta%20%25.md): Calcula a variação percentual das vendas do mês atual em comparação com o mesmo mês do ano anterior.
8. [Sales Last Year](Medidas%20Inteligência%20Temporal/08%20Sales%20Last%20Year.md): Calcula o total de vendas do ano anterior.
9. [Sales Last Year Delta](Medidas%20Inteligência%20Temporal/09%20Sales%20Last%20Year%20Delta.md): Calcula a diferença entre as vendas em relação ao ano anterior.
10. [Sales Last Year Delta %](Medidas%20Inteligência%20Temporal/10%20Sales%20Last%20Year%20Delta%20%25.md): Calcula a diferença percentual das vendas em relação ao ano anterior.
11. [Sales Year to Date](Medidas%20Inteligência%20Temporal/11%20Sales%20Year%20to%20Date.md): Calcula as vendas acumuladas no ano até a data atual.
12. [Sales Year to Date Last Year](Medidas%20Inteligência%20Temporal/12%20Sales%20Year%20to%20Date%20Last%20Year.md): Calcula as vendas acumuladas do ano até a data do ano anterior.
13. [Sales Year to Date Last Year Delta](Medidas%20Inteligência%20Temporal/13%20Sales%20Year%20to%20Date%20Last%20Year%20Delta.md): Calcula a diferença entre as vendas acumuladas até a data deste ano e as vendas acumuladas até a mesma data no ano passado.
14. [Sales Year to Date Last Year Delta %](Medidas%20Inteligência%20Temporal/14%20Sales%20Year%20to%20Date%20Last%20Year%20Delta%20%25.md): Calcula a diferença percentual das vendas acumuladas no ano em relação ao ano anterior.
15. [Sales Month to Date](Medidas%20Inteligência%20Temporal/15%20Sales%20Month%20to%20Date.md): Calcula o total de vendas acumuladas no mês até a data atual.
16. [Sales Month to Date Last Month](Medidas%20Inteligência%20Temporal/16%20Sales%20Month%20to%20Date%20Last%20Month.md): Calcula o total das vendas acumuladas até a data do mês passado.
17. [Sales Month to Date Last Month Delta](Medidas%20Inteligência%20Temporal/17%20Sales%20Month%20to%20Date%20Last%20Month%20Delta.md): Calcula a diferença entre as vendas acumuladas até o momento no mês atual e as vendas acumuladas até o mesmo dia no mês anterior.
18. [Sales Month to Date Last Month Delta %](Medidas%20Inteligência%20Temporal/17%20Sales%20Month%20to%20Date%20Last%20Month%20Delta.md): Calcula a variação percentual das vendas acumuladas até o mês passado em comparação com o mesmo período do mês anterior.

