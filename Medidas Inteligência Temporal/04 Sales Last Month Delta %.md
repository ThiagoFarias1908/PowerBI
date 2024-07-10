# Medida: Sales Last Month Delta %

**Descrição:** Calcula a variação percentual das vendas em relação ao mês anterior.

**Fórmula DAX:**
```DAX
Sales Last Month Delta % = 
DIVIDE(
    [Sales Last Month Delta];
    [Sales Last Month]
)
