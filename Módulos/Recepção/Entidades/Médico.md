#entidade
## Entidade:
```mermaid
erDiagram
MEDICO {
	uuid id PK
	string nome
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
- [[Especialidade do Médico]]
- [[Atendimento]]
- [[Atendimento de Emergência]]
- [[Horário de Atendimento]]