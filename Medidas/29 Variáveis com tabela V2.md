# Medida: Variáveis com tabela

**Descrição:** Cria uma variável que calcula a média das vendas para os anos e meses abreviados na tabela.

**Fórmula DAX:**
```DAX
Variáveis com tabela V2 = 
VAR MY_TBL =
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
)
RETURN
AVERAGEX(
    MY_TBL;
    [Sales]
)
