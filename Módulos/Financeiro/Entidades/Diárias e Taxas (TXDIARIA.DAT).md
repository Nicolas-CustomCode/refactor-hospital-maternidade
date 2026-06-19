#entidade
## Arquivos:
- TXDIARIA.DAT
- NDIARIA.DAT

---

## Entidade:
```mermaid
erDiagram

TAXA_DIARIA {
	int codigo PK "TXDIARIA.DAT | campo1"
	string descricao "TXDIARIA.DAT | campo2"
	int tipo "TXDIARIA.DAT | tipo"
	decimal valor_sanepar "TXDIARIA.DAT | valor1"
	decimal valor_copel "TXDIARIA.DAT | valor2"
	decimal valor_ipe "TXDIARIA.DAT | valor3"
	decimal valor_unimed "TXDIARIA.DAT | valor4"
	decimal valor_bradesco "TXDIARIA.DAT | valor5"
	decimal em_branco "TXDIARIA.DAT | valor6"
	decimal valor_furnas "TXDIARIA.DAT | valor7"
	decimal valor_coamo "TXDIARIA.DAT | valor8"
	decimal valor_pam "TXDIARIA.DAT | valor9"
	decimal valor_sas "TXDIARIA.DAT | valor10"
}
```

### Valores predefinidos:
#### tipo
- 0 = Diária
- 1 = Taxa
