# Medida: Variáveis com tabela

**Descrição:** Cria uma variável que encontra o ano máximo entre os anos únicos da tabela.

**Fórmula DAX:**
```DAX
Variáveis com tabela = 
VAR MYTBL =
    SUMMARIZE(
        dim_calendario;
        dim_calendario[Ano]
    )
RETURN 
MAXX(
    MYTBL;
    dim_calendario[Ano]
)
