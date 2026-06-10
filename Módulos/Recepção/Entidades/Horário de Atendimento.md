#entidade
## Entidade:
```mermaid
erDiagram
HORARIO_ATENDIMENTO {
	uuid id PK
	uuid medico_id FK
	date hora_entrada
	date hora_saida
}
```

---

## Entidades que se relaciona:
- [[Médico]]