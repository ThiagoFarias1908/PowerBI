# Medida: Sales SUMX

**Descrição:** Calcula o total de vendas usando a função SUMX.

**Fórmula DAX:**
```DAX
Sales SUMX = 
SUMX(
    fat_sales;
    IF(
        fat_sales[Revenue] > 0;
        fat_sales[Revenue]
    )
)
