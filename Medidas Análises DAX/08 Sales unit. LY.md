# Medida: Sales unit. LY

**Descrição:** Calcula o valor médio de venda por unidade no mesmo período do ano passado.

**Fórmula DAX:**
```DAX
Sales unit. LY = 
VAR salesunitLY =
    CALCULATE(
        [Sales unit.];
        SAMEPERIODLASTYEAR(dim_calendario[Date])
    )
RETURN
IF(
    [Sales unit.];
    salesunitLY
)
