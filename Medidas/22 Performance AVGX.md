# Medida: Performance AVGX

**Descrição:** Calcula a performance média das entregas com base na data de entrega.

**Fórmula DAX:**
```DAX
Performance AVGX = 
AVERAGEX(
    fat_sales;
    DATEDIFF(
        fat_sales[Expected Delivery Date];
        fat_sales[Actual Delivered Date];
        DAY
    )
)
