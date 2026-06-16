#entidade 
## Entidade:
```mermaid
erDiagram
DIARIA_CONVENIO {
	uuid id PK
	uuid diaria_id FK
	uuid convenio_id FK
	decimal valor
}
```

---

## Entidades que se relaciona:
- [[Diária]]
- [[Convênio]]
- [[Item da Conta]]