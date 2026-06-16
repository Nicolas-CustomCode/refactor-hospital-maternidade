#entidade 
## Entidade
```mermaid
erDiagram
MEDICAMENTO_CONVENIO {
	uuid id PK
	uuid medicamento_id FK
	uuid convenio_id FK
	decimal valor
}
```

---

## Entidades que se relaciona:
- [[Medicamento]]
- [[Convênio]]
- [[Item da Conta]]