# Medida: Sales Last Year

**Descrição:** Calcula o total de vendas do ano anterior.

**Fórmula DAX:**
```DAX
Sales Last Year = 
VAR YoY =
CALCULATE(
    [Sales];
    SAMEPERIODLASTYEAR(dim_calendario[Date])
)
RETURN
IF(
    [Sales];
    YoY
)
