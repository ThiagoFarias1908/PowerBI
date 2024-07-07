# Medida: Variáveis com um valor

**Descrição:** Cria duas variáveis que retornam a soma do ano e do mês máximos.

**Fórmula DAX:**
```DAX
Variáveis com um valor = 
VAR MYYEAR = MAX(dim_calendario[Ano])
VAR MYMONTH = MAX(dim_calendario[Mês])
RETURN
MYYEAR + MYMONTH
