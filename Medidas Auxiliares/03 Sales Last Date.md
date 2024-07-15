# Medida: Sales Last Date

**Descrição:** Calcula a data da última venda no ano selecionado.

**Fórmula DAX:**
```DAX
SalesLastDate = 
CALCULATE(
    LASTDATE(dim_calendario[Date]);
    REMOVEFILTERS(dim_calendario[Date])
)
