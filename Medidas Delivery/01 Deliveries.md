# Medida: Deliveries

**Descrição:** Determina o número de entregas com base na data de entrega.

**Fórmula DAX:**
```DAX
Deliveries = 
CALCULATE(
    COUNT(fat_sales[Order Id]);
    USERELATIONSHIP(
        fat_sales[Actual Delivered Date];
        dim_calendario[Date]
    )
)
