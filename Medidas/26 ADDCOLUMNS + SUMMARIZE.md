# Medida: ADDCOLUMNS + SUMMARIZE

**Descrição:** Calcula a média de vendas por mês e ano.

**Fórmula DAX:**
```DAX
ADDCOLUMNS + SUMMARIZE = 
AVERAGEX(
    FILTER(
        ADDCOLUMNS(
            SUMMARIZE(
                dim_calendario;
                dim_calendario[Ano];
                dim_calendario[Mes abrev]
            );
            "Sales"; [01 Sales]
        );
        NOT(ISBLANK([Sales]))
    );
    [Sales]
)
