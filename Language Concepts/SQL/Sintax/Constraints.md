
Constraints são restrições de informações, impedindo que haja mais erros e bugs na DB. Sao usadas para especificar regras nos dados de uma tabela.

Por exemplo, se temos um campo para preencher o CPF

```sql
CREATE TABLE user(
	id INTEGER PRIMARY KEY,
	name TEXT,
	cpf 
)
```