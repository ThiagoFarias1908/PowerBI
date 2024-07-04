# Medida: Sales Total Category ALLSELECTED

**Descrição:** Calcula o total de vendas por categoria, considerando a seleção feita no relatório (ALLSELECTED).

**Fórmula DAX:**
```DAX
Sales Total Category ALLSELECTED = 
CALCULATE(
    [01 Sales];
    ALLSELECTED(dim_material[CAT_ID])
)
