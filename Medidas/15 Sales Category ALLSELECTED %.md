# Medida: Sales Category ALLSELECTED %

**Descrição:** Calcula a porcentagem das vendas por categoria, considerando o contexto de seleção atual utilizando a função `ALLSELECTED`.

**Fórmula DAX:**
```DAX
Sales Category ALLSELECTED % = 
DIVIDE(
    [01 Sales];
    [14 Sales Total Category ALLSELECTED]
)
