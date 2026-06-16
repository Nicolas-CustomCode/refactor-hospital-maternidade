#entidade
## Entidade:
```mermaid
erDiagram
INTERNACAO_DIAGNOSTICO {
	uuid id PK
	uuid internacao_id FK
	uuid diagnostico_id FK
}
```