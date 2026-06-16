#entidade
## Entidade:
```mermaid
erDiagram
PACIENTE_RESPONSAVEL {
	uuid id PK
	uuid paciente_id FK
	uuid responsavel_id FK
	string relacao
}
```

---

## Entidades que se relaciona:
- [[Paciente]]
- [[Responsável]]