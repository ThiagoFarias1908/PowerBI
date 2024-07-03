# Medida: Orders Quantity with revenue < 0

**Descrição:** Calcula a quantidade de pedidos com receita menor que zero.

**Fórmula DAX:**
```DAX
Orders Quantity with revenue < 0 = 
COUNTX(
    fat_sales;
    IF(
        fat_sales[Revenue] > 0;
        fat_sales[Revenue]
    )
)
