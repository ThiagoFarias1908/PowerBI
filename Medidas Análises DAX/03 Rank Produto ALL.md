# Medida: Rank Produto ALL

**Descrição:** Calcula o ranking de vendas dos produtos, considerando todas as categorias.

**Fórmula DAX:**
```DAX
Rank Produto ALL = 
VAR RNK =
    RANKX(
        ALL(dim_material);
        [Sales];;
        DESC
    )
RETURN
IF(
    [Sales];
    RNK
)
