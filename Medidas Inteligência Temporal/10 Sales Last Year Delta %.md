# Medida: Sales Last Year Delta %

**Descrição:** Calcula a diferença percentual das vendas em relação ao ano anterior.

**Fórmula DAX:**
```DAX
Sales Last Year Delta % = 
DIVIDE(
    [Sales Year over Year Delta];
    [Sales Year over Year]
)
