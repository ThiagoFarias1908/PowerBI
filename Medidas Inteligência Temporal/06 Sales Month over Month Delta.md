# Medida: Sales Month over Month Delta

**Descrição:** Calcula a diferença entre as vendas do mês atual e as vendas do mesmo mês no ano anterior.

**Fórmula DAX:**
```DAX
Sales Month over Month Delta = 
VAR DELTA =
[Sales] - [Sales Month over Month]
RETURN
IF(
    [Sales Month over Month];
    DELTA
)
