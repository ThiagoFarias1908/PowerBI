# Medida: Sales Month to Date Last Month

**Descrição:** Calcula o total das vendas acumuladas até a data do mês passado.

**Fórmula DAX:**
```DAX
Sales Month to Date Last Month = 
CALCULATE(
    [Sales Month to Date];
    DATEADD(
        dim_calendario[Date];
        -1;
        MONTH
    )
)
