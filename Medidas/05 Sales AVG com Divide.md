# Medida: Sales AVG com Divide

**Descrição:** Calcula a média das vendas utilizando a função `DIVIDE` para evitar divisão por zero.

**Fórmula DAX:**
```DAX
05 Sales AVG com Divide = 
DIVIDE([01 Sales]; [04 Distinct Orders Quantity])
