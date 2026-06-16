#entidade 
## Entidade:
```mermaid
erDiagram
MATERIAL_CONVENIO {
	uuid id PK
	uuid material_id FK
	uuid convenio_id FK
	decimal valor
}
```

---

## Entidades que se relaciona:
- [[Material]]
- [[Convênio]]
- [[Item da Conta]]