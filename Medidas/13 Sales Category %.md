# Medida: Sales Category %

**Descrição:** Calcula a porcentagem de vendas por categoria em relação ao total de vendas.

**Fórmula DAX:**
```DAX
Sales Category % = 
DIVIDE(
    [01 Sales];
    [12 Sales Total Category]
)
