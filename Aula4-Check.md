# Constraint Check
* Faz uma validação de acorndo com certas condiçoes
```sql
    ALTER TABLE Produtos ADD CONSTRAINT CHK_ColunaGenero CHECK(Genero='U' OR Genero='M' OR Genero='F')
```
