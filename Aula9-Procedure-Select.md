# Store Procedure com select
* alem de insert update e delete também é possível colocar um select
```sql
--criando procedure
    CREATE PROCEDURE ObterProdutosPorTamanho
        @Tamanho varchar(5)

    AS

    SELECT * FROM Produtos WHERE Tamanho = @Tamanho
    --Obtendo pelo tamannho
    EXEC ObterProdutosPorTamanho 'M'
    
    --Procedures sem parametros
    CREATE PROCEDURE ObterTodosProdutos
    AS
    SELECT * FROM Produtos WHERE Tamanho = @Tamanho

```
