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
	int codigo PK "PROD.DAT | codigo"
	string nome "PROD.DAT | nome"
	string unidade "PROD.DAT | unidade"
	string observacao "PROD.DAT | observacao"
	int padrao "PROD.DAT | padrao"
	int minimo "PROD.DAT | minimo"
	int maximo "PROD.DAT | maximo"
	int custo_medio "PROD.DAT | medio"
	int grupo FK "PROD.DAT | grupo"
	int subgrupo FK "SUBGRUP.DAT | subgrupo"
	int controlado "PROD.DAT | controlado"
	int tabela_compras "PROD.DAT | tipo_compra"
}
```

### Valores predefinidos
#### controlado
- 0 = Nao
- 1 = P. 27
- 2 = P. 28 A
- 3 = P. 28 B
- 4 = Antimi.
- 5 = Outros
