# Medida: CALCULATE + ALL

**Descrição:** Calcula a receita líquida total das categorias.

**Fórmula DAX:**
```DAX
CALCULATE(
    SUM(fat_sales[Revenue]);
    ALL(dim_material[CAT_ID])
)
