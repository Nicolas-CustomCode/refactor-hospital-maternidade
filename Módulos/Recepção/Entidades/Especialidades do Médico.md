## Entidade
```mermaid
erDiagram
MEDICO_ESPECIALIDADE {
	uuid id PK
	uuid medico_id FK
	uuid especialidade_id FK
}
```

---

## Especialidades que se relaciona
- [[Médico]]
- [[Especialidade]]