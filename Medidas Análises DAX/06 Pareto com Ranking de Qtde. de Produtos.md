# Medida: Pareto com Ranking de Qtde. de Produtos

**Descrição:** Calcula o ranking dos produtos com base na quantidade vendida.

**Fórmula DAX:**
```DAX
Pareto com Ranking de Qtde. de Produtos = 
VAR qtdeprod =
MAXX(
    ALLSELECTED(dim_material[MATERIAL_ID]);
    [Rank Produto ALLSELECTED]
)
RETURN
DIVIDE(
    [Rank Produto ALLSELECTED];
    qtdeprod
)
