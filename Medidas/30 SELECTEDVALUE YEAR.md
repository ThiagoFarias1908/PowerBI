# Medida: SELECTEDVALUE YEAR

**Descrição:** Cria uma variável que calcula o ano máximo presente na coluna e retorna o valor do ano selecionado.

**Fórmula DAX:**
```DAX
SELECTEDVALUE YEAR = 
VAR MAXYEAR = MAX(dim_calendario[Ano])
RETURN
SELECTEDVALUE(
    dim_calendario[Ano]; 
    MAXYEAR
)
