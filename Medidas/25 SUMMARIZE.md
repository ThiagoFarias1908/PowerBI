# Medida: SUMMARIZE

**Descrição:** Cria uma tabela resumida que calcula o média de lucro das vendas por mês e ano.

**Fórmula DAX:**
```DAX
SUMMARIZE = 
AVERAGEX(
    FILTER(
        SUMMARIZE(
            dim_calendario;
            dim_calendario[Ano];
            dim_calendario[Mes abrev];
            "Sales"; [01 Sales]
        );
        NOT(ISBLANK([Sales]))
    );
    [Sales]
)
