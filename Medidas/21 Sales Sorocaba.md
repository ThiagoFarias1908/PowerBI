# Medida: Sales Sorocaba

**Descrição:** Calcula o total das vendas realizadas na cidade de Sorocaba.

**Fórmula DAX:**
```DAX
Sales Sorocaba = 
CALCULATE(
    [01 Sales];
    FILTER(
        VALUES(dim_plant[Plant Name]);
        dim_plant[Plant Name] = "Sorocaba"
    )
)
