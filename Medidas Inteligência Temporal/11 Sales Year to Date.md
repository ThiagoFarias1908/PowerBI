# Medida: Sales Year to Date

**Descrição:** Calcula as vendas acumuladas no ano até a data atual.

**Fórmula DAX:**
```DAX
Sales Year to Date = 
TOTALYTD(
    [Sales];
    dim_calendario[Date]
)
