# Funcions

* built functions, do próprio banco 
* a function precisa retornar um valor
* a sore procedure não é obrigatório retornar um valor


```sql

    CREATE FUNCTION CalcularDesconto(@Preco Decimal(13,2), @Porcentagem INT)
    RETURNS DECIMAL(13,2) --TIPO DO RETORNO DA FUNÇÃO
    BEGIN
        RETURN @Preco - @Preco/100*@Porcentagem --O RETORNO DA FUNÇÃO EM SI
    END


    SELECT 
        Nome,
        Preco,
        dbo.CalcularDesconto(Preco,50) PrecoComDesconto
    FROM Produtos WHERE	Tamanho = 'M'

```