# Medida: Rank Produto ALLSELECTED

**Descrição:** Calcula o ranking dos produtos com base no valor total das vendas, respeitando os filtros aplicados ao relatório.

**Fórmula DAX:**
```DAX
Rank Produto ALLSELECTED = 
VAR RNK =
    RANKX(
        ALLSELECTED(dim_material);
        [Sales];;
        DESC
    )
RETURN
IF(
    [Sales];
    RNK
)
