# Medida: Sales qtde. avg -30

**Descrição:** Calcula a média da quantidade de vendas nos últimos 30 dias.

**Fórmula DAX:**
```DAX
Sales qtde. avg -30 = 
AVERAGEX(
    ADDCOLUMNS(
        DATESBETWEEN(
            dim_calendario[Date];
            MAX(fat_sales[Sales Date])-30;
            MAX(fat_sales[Sales Date])
        );
        "qtde_"; [Sales qtde.]
    );
    [qtde_]
)
