# Medida: Sales Year over Year Delta

**Descrição:** Calcula a diferença entre as vendas em relação ao ano anterior.

**Fórmula DAX:**
```DAX
Sales Year over Year Delta = 
VAR DELTA =
[Sales] - [Sales Year over Year]
RETURN
IF(
    [Sales Year over Year];
    DELTA
)
