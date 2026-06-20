#entidade
## Arquivos:
- PROD.DAT
- GRUP.DAT ([[Grupo (GRUP.DAT)]])
- SUBGRUP.DAT ([[Subgrupo (SUBGRUP.DAT)]])
- FORN.DAT ([[Fornecedor (FORN.DAT)]])

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
	decimal quantidade "PROD.DAT | quantidade"
	int custo_medio "PROD.DAT | medio"
	int grupo FK "GRUP.DAT | codigo"
	int subgrupo FK "SUBGRUP.DAT | codigo"
	int controlado "PROD.DAT | controlado"
	int tabela_compras "PROD.DAT | tipo_compra"
	int ultimo_fornecedor FK "FORN.DAT | codigo"
	date ultima_compra "PROD.DAT | ultdata"
	decimal custo_medio "--CAMPO NÃO ENCONTRADO--"
	decimal proeps "PROD.DAT | unitario"
	decilam brasindice "PROD.DAT | pbrasindice"
	decimal reposicao "--CAMPO NÃO ENCONTRADO--"
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
