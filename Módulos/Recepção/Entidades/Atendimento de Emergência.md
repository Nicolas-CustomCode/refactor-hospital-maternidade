## Entidade:
```mermaid
erDiagram
ATENDIMENTO_EMERGENCIA {
	uuid id PK
	uuid paciente_id FK
	uuid medico_id FK
	uuid internacao_id FK
	date hora_entrada
	date hora_saida
}
```

---

## Entidades que se relaciona
- [[Paciente]]
- [[Médico]]
- [[Internação]]