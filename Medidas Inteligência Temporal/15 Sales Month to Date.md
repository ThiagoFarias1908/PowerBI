# Medida: Sales Month to Date

**Descrição:** Calcula o total de vendas acumuladas no mês até a data atual.

**Fórmula DAX:**
```DAX
Sales Month to Date = 
TOTALMTD(
    [Sales];
    dim_calendario[Date]
)
