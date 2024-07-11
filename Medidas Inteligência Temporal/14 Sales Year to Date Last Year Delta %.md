# Medida: Sales Year to Date Last Year Delta %

**Descrição:** Calcula a diferença percentual das vendas acumuladas no ano em relação ao ano anterior.

**Fórmula DAX:**
```DAX
Sales Year to Date Last Year Delta % = 
DIVIDE(
    [Sales Year to Date Last Year Delta];
    [Sales Year to Date Last Year]
)
