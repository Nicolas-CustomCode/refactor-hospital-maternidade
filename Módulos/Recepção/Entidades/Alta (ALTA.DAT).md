#entidade
## Arquivos:
- ALTA.DAT
- INTER.DAT
- PACIT.DAT
- CONSU.DAT
- CLAS.DAT

---

## Entidade:
```mermaid
erDiagram
ALTA {
	int numero_ordem PK
	int paciente FK "PACIT.DAT | registro"
}
```
 