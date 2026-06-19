#entidade
## Arquivos:
- PACIT.DAT
- PACIT2.DAT
- PACIT3.DAT
- IBGE.DAT
- CIDADES.DAT
- CLAS.DAT

---

## Entidade:
```mermaid
erDiagram
PACIENTE {
	int codigo PK "PACIT.DAT | registro"
	string nome "PACIT.DAT | nome"
	string endereco "PACIT.DAT | endereco"
	string cidade "PACIT.DAT | cidade"
	string estado "PACIT.DAT | uf"
	
}
```
