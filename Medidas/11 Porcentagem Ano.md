# Medida: Porcetagem Ano

**Descrição:** Calcula a porcentagem de vendas em relação ao ano.

**Fórmula DAX:**
```DAX
Porcentagem Ano = 
CALCULATE(
    DIVIDE(
        [01 Sales];
        CALCULATE(
            [01 Sales];
            ALL(dim_calendario[Ano])
        )
    )
)
