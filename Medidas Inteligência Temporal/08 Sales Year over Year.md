# Medida: Sales Year over Year

**Descrição:** Calcula o total de vendas do ano anterior.

**Fórmula DAX:**
```DAX
Sales Year over Year = 
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
