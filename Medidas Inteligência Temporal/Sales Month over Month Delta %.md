# Medida: Sales Month over Month Delta %

**Descrição:** Calcula a variação percentual das vendas do mês atual em comparação com o mesmo mês do ano anterior.

**Fórmula DAX:**
```DAX
Sales Month over Month Delta % = 
DIVIDE(
    [Sales Month over Month Delta];
    [Sales Month over Month]
)
