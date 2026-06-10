#entidade
## Entidade:
```mermaid
erDiagram
RESPONSAVEL {
	uuid id PK
	string nome
	string cpf
	string telefone
	string cep
	string estado
	string cidade
	string bairro
	string rua
	string numero
}
```

---

## Entidades que se relaciona:
- [[Responsáveis do Paciente]]