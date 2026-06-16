#entidade
## Entidade:
```mermaid
erDiagram
INTERNACAO_CONVENIO {
	uuid id PK
	uuid internacao_id FK
	uuid convenio_id FK
	decimal valor
}
```

---

## Entidades que se relaciona:
- [[Internação]]
- [[Convênio]]