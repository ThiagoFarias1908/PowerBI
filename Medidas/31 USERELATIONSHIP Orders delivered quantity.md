# Medida: USERELATIONSHIP Orders delivered quantity

**Descrição:** Calcula a quantidade de pedidos entregues usando o relacionamento especificado entre as tabelas.

**Fórmula DAX:**
```DAX
USERELATIONSHIP Orders delivered quantity = 
CALCULATE(
    [03 Orders Quantity];
    USERELATIONSHIP(
        fat_sales[Actual Delivered Date];
        dim_calendario[Date]
    )
)
