# Medida: CROSSJOIN

**Descrição:** Calcula o total das vendas por mês e ano.

**Fórmula DAX:**
```DAX
CROSSJOIN = 
AVERAGEX(
    FILTER(
        ADDCOLUMNS(
            CROSSJOIN(
                VALUES(dim_calendario[Ano]);
                VALUES(dim_calendario[Mes abrev])
            );
            "Sales"; [01 Sales]
        );
        NOT(ISBLANK([Sales]))
    );
    [Sales]
)
