# Medida: Deliveries Late

**Descrição:** Calcula o número de entregas atrasadas.

**Fórmula DAX:**
```DAX
Deliveries Late = 
CALCULATE(
    [Deliveries];
    FILTER(
        VALUES(fat_sales[Delivery Status]);
        fat_sales[Delivery Status] = "Late"
    )
)
