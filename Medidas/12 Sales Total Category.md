# Medida: Sales Total Category

**Descrição:** Calcula o total de vendas por categoria de produto.

**Fórmula DAX:**
```DAX
Sales Total Category = 
CALCULATE(
    [01 Sales];
    ALL(dim_material[CAT_ID])
)
