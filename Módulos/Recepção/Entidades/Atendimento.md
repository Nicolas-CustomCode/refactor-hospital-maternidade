#entidade
## Entidade:
```mermaid
erDiagram
ATENDIMENTO {
	uuid id PK
	uuid paciente_id FK
	uuid medico_id FK
	enum tipo
	date hora_entrada
	date hora_saida
}
```

---

## Entidades que se relaciona:
- [[Paciente]]
- [[Médico]]