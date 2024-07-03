# Medida: Porcetagem Categoria

**Descrição:** Calcula a porcentagem de vendas por categoria.

**Fórmula DAX:**
```DAX
DIVIDE(
    [01 Sales]; 
    [09 CALCULATE + ALL]
)
