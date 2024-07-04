# Medida: Sales Total CA06 V2

**Descrição:** Calcula o total das vendas para a categoria CA06 de outra maneira.

**Fórmula DAX:**
```DAX
Sales Total CA06 V2 = 
CALCULATE(
    [01 Sales];
    dim_material[CAT_ID] = "CA06"
)
