# Medida: Sales AVGX

**Descrição:** Calcula a média ponderada das vendas utilizando a função `AVERAGEX`, considerando apenas valores de receita maiores que zero.

**Fórmula DAX:**
```DAX
Sales AVGX = AVERAGEX(fat_sales; IF(fat_sales[Revenue] > 0 ; fat_sales[Revenue]))
