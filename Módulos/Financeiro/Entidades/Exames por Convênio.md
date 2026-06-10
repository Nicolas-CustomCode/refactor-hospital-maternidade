#entidade 
## Entidade:
```mermaid
erDiagram
EXAMES_CONVENIO {
	uuid id PK
	uuid exame_id FK
	uuid convenio_id FK
	decimal valor
}
```

---

## Entidades que se relaciona:
- [[Exames da Conta]]
- [[Exame]]
- [[Convênio]]