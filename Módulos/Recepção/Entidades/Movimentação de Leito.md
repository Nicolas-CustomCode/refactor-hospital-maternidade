#entidade
## Entidade:
```mermaid
erDiagram
LEITO_MOVIMENTACAO {
	uuid id PK
	uuid internacao_id FK
	uuid leito_id FK
	uuid novo_leito_id FK
	string codigo
}
```

Incompleto