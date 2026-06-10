#entidade 
## Entidade:
```mermaid
erDiagram
CONTA {
	uuid id PK
	uuid internacao_id FK
	uuid conta_servico FK
	uuid conta_exame FK
	uuid conta_diaria FK
}
```

---

## Entidades que se relaciona:
- [[Internação]]
- [[Itens da Conta]]