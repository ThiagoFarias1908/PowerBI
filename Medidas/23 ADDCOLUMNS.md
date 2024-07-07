# Medida: ADDCOLUMNS

**Descrição:** Adiciona uma coluna calculada, que calcula a média de lucro para cada mês.

**Fórmula DAX:**
```DAX
ADDCOLUMNS = 
AVERAGEX(
    ADDCOLUMNS(
        VALUES(dim_calendario[Mes abrev]);
        "Sales";
        [01 Sales]
    );
    [Sales]
)
