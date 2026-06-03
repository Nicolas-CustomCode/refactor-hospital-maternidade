## Entidade
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

## Entidades que se relaciona
- [[Especialidades do Médico]]
- [[Atendimento Clínico]]
- [[Atendimento de Emergência]]
- [[Horário de Atendimento]]