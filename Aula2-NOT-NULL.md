# Constraint NOT NULL
* Selecionando a tabela e apertando alt+F1
* a coluna preço foi omitida sendo notnull
```sql
    INSERT INTO Produtos(nome,Cor,Tamanho,Genero,DataCadastro)
    VALUES('Nome','Cor', 'G','M',GETDATE())
```
* na omissão o seguinte output é gerado quando é tentado executar a query
```console
    Não é possível inserir o valor NULL na coluna 'Preco', tabela 'ExemploDB.dbo.Produtos'; a coluna não permite nulos. Falha em INSERT.
```

