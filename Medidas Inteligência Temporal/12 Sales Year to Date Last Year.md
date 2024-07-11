# Medida: Sales Year to Date Last Year

**Descrição:** Calcula as vendas acumuladas do ano até a data do ano anterior.

**Fórmula DAX:**
```DAX
Sales Year to Date Last Year = 
CALCULATE(
    [Sales Year to Date];
    DATEADD(
        dim_calendario[Date];
        -1;
        YEAR
    )
)
