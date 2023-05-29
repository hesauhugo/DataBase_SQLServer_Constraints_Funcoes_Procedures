# Constraint Unique

* Garante o que o nome seja único
```sql
    ALTER TABLE Produtos ADD UNIQUE(Nome)
```
* Exibe mensagem que não pode existir produtos com nome duplicado