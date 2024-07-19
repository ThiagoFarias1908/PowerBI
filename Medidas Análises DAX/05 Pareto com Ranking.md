# Medida: Pareto com Ranking

**Descrição:** Calcula a porcentagem acumulada das vendas em relação ao total, juntamente com o ranking das vendas.

**Fórmula DAX:**
```DAX
Pareto com Ranking = 
VAR ranking = [Rank Produto ALLSELECTED]
VAR TotalVendas = CALCULATE([Sales]; ALLSELECTED(fat_sales))
VAR Acumulado =
            CALCULATE(
                [Sales];
                FILTER(
                    ALLSELECTED(dim_material[MATERIAL_ID]);
                    [Rank Produto ALLSELECTED] <= ranking
                )
            )
RETURN
DIVIDE(
    Acumulado;
    TotalVendas
)
