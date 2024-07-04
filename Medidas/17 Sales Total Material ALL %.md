# Medida: Sales Total Material ALL %

**Descrição:** Calcula o percentual das vendas totais de materiais em relação ao total geral das vendas, independentemente de quaisquer filtros aplicados.

**Fórmula DAX:**
```DAX
Sales Total Material ALL % = 
DIVIDE(
    [01 Sales];
    [16 Sales Total Material ALL]
)
