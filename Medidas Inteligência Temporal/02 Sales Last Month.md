# Medida: Sales Last Month

**Descrição:** Calcula o total de vendas do mês anterior.

**Fórmula DAX:**
```DAX
Sales Last Month = 
VAR LM = 
CALCULATE(
    [Sales];
    DATEADD(
        dim_calendario[Date];
        -1;
        MONTH
    )
)
RETURN
IF(
    [Sales];
    LM
)
