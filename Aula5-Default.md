# Constraint default
* Assume um valor padrão caso omita um valor
```sql
    ALTER TABLE Produtos ADD DEFAULT GETDATE() FOR DataCadastro
```