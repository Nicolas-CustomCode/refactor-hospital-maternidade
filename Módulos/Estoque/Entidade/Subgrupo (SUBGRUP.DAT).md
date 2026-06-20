#entidade
## Arquivos:
- SUBGRUP.DAT
- GRUP.DAT ([[Grupo (GRUP.DAT)]])

---

## Entidade:
```mermaid
erDiagram
SUBGRUPO {
	int codigo_grupo FK "GRUP.DAT | codigo"
	int codigo PK "SUBGRUP.DAT | campo1"
	string nome "SUBGRUP.DAT | campo2"
}
```

---

## Obs:
- 2 primeiros dígitos de `campo1` se referem ao código do grupo e os 2 últimos se referem ao código do subgrupo
