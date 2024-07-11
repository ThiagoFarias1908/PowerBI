# Medida: Sales Month to Date Last Month Delta %

**Descrição:** Calcula a variação percentual das vendas acumuladas até o momento no mês atual em comparação com o mesmo período do mês anterior.

**Fórmula DAX:**
```DAX
Sales Month to Date Last Month Delta % = 
DIVIDE(
    [Sales Month to Date Last Month Delta];
    [Sales Month to Date Last Month]
)
