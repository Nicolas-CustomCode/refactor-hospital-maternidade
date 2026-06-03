## Entidade
```mermaid
erDiagram
INTERNACAO_CONVENIO {
	uuid id PK
	uuid internacao_id FK
	uuid convenio_id FK
}
```

---

## Entidades que se relaciona
- [[Internação]]
- [[Convênio]]