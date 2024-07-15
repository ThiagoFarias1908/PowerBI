# Medida: Deliveries On Time

**Descrição:** Calcula o número de entregas realizadas dentro do prazo.

**Fórmula DAX:**
```DAX
Deliveries On Time = 
CALCULATE(
    [Deliveries];
    FILTER(
        VALUES(fat_sales[Delivery Status]);
        fat_sales[Delivery Status] = "On Time"
    )
)
