# Medida: Delivery Lead Time

**Descrição:** Calcula o tempo médio de entrega dos pedidos.

**Fórmula DAX:**
```DAX
Delivery Lead Time = 
AVERAGEX(
    fat_sales;
    fat_sales[Actual Delivered Date] - fat_sales[Sales Date]
)
