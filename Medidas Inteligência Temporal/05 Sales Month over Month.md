# Medida: Sales Month over Month

**Descrição:** Calcula o total de vendas do mesmo mês no ano anterior.

**Fórmula DAX:**
```DAX
Sales Month over Month = 
VAR MoM =
    CALCULATE(
        [Sales];
        SAMEPERIODLASTYEAR(dim_calendario[Date])
    )
RETURN
IF(
    [Sales];
    MoM
)
