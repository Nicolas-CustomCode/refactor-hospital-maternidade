## Entidade:
```mermaid
erDiagram
PACIENTE {
	uuid id PK
	string nome
	date data_nascimento
	string sexo
	string nome_mae
	string cpf
	string telefone
	string cartao_sus
	string cep
	string logradouro
	string numero
	string complemento
	string bairro
	string cidade
	string estado
}
```

---

## Entidades que se relaciona
- [[Convênios do Paciente]]
- [[Responsáveis do Paciente]]