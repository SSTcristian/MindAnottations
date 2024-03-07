
Constraints (restrição) são restrições de informações, impedindo que haja mais erros e bugs na DB. São usadas para especificar regras na coluna (ou conjunto) de uma tabela

Existem muitos tipos de constraints, como:

# PRIMARY KEY (Chave Primaria)
Usadas para identificar exclusivamente cada registro numa tabela (uma tabela só pode ter UMA primary key)

```sql
CREATE TABLE pessoa(
	cpf TEXT PRIMARY KEY,
	nome TEXT,
	sobrenome TEXT
);
```

# FOREIGN KEY (Chave Estrangeira)
Estabelece uma relacao entre duas tabelas, garantindo que uma coluna seja igual a outra que é a chave primaria de outra tabela. Ela mantem a integridade dos dados referenciados 

```sql
CREATE TABLE cars(
	PlacaId INT PRIMARY KEY,
	DonoCPF TET,
	Fabricacao DATE,
	FOREIGN KEY (DonoCPF) REFERENCES pessoa(cpf)
);
```


# Links
https://www.w3schools.com/sql/sql_constraints.asp