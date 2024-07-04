# Medida: Sales Total CA06

**Descrição:** Calcula o total das vendas para a categoria CA06.

**Fórmula DAX:**
```DAX
Sales Total CA06 = 
CALCULATE(
    [01 Sales];
    FILTER(
        ALL(dim_material[CAT_ID]);
        dim_material[CAT_ID] = "CA06"
    )
)
