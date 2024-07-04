# Medida: Sales Total Material ALL

**Descrição:** Calcula o total de vendas de materiais, ignorando qualquer filtro aplicado.

**Fórmula DAX:**
```DAX
Sales Total Material ALL = 
CALCULATE(
    [01 Sales];
    ALL(dim_material)
)
