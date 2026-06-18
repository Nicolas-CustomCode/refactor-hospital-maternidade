#entidade
## Arquivos:
- PROD.DAT
- GRUP.DAT ([[Grupo (GRUP.DAT)]])
- SUBGRUP.DAT ([[Subgrupo (SUBGRUP.DAT)]])

---

## Entidade:
```mermaid
erDiagram
PRODUTO {
	int codigo PK
	string nome
	string unidade
	string observacao
	int padrao
	
	int grupo FK "GRUP.DAT | codigo"
	int subgrupo FK "SUBGRUP.DAT | campo1"
	
	int produto_controlado
	int tabela_compras
}
```

### Valores predefinidos
#### produto_controlado
- 0 = Nao
- 1 = P. 27
- 2 = P. 28 A
- 3 = P. 28 B
- 4 = Antimi.
- 5 = Outros
