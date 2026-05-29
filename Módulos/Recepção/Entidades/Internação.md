## Entidade
```mermaid
erDiagram
INTERNACAO {
	uuid id PK
	uuid paciente_id FK
	uuid responsavel_id FK
	uuid medico_id FK
	uuid leito_atual_id FK
	bigint codigo
	datetime data_entrada
	datetime data_encerramento
}
```

---

## Entidades que se Relaciona
- [[Paciente]]
- [[Responsável]]
- [[Médico]]
- [[Leito]]