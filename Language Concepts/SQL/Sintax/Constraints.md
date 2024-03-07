
Constraints (restrição) são restrições de informações, impedindo que haja mais erros e bugs na DB. São usadas para especificar regras na coluna (ou conjunto) de uma tabela

Existem muitos tipos de constraints, como:

# PRIMARY KEY (Chave Primaria)
Usadas para identificar exclusivamente cada registro numa tabela (uma tabela só pode ter UMA primary key)

```sql
CREATE TABLE user(
	id INTEGER PRIMARY KEY,
	name TEXT,
	second_name TEXT 
)
```