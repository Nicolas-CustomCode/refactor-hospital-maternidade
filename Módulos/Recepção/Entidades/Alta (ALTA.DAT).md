#entidade
## Arquivos:
- ALTA.DAT
- INTER.DAT ([[Internação (INTER.DAT)]])
- PACIT.DAT ([[Paciente (PACIT.DAT, PACIT2.DAT, PACIT3.DAT)]])
- CONSU.DAT ([[Consumidor (CONSU.DAT)]])
- CLAS.DAT ([[Classificação (CLAS.DAT)]])
- SET.DAT ([[Setor (SET.DAT)]])

---

## Entidade:
```mermaid
erDiagram
ALTA {
	int codigo PK "PACIT.DAT | codigo"
	int paciente FK "PACIT.DAT | codigo"
	date data_entrada "PACIT.DAT | dentrada"
	date data_alta "PACIT.DAT | dalta"
	int tipo_alta "PACIT.DAT | talta"
	int hora
	int setor FK "SET.DAT | codigo"
	int quarto FK "CONSU.DAT | codigo"
	int encaminhamento
	int classificacao FK "CLAS.DAT | codigo"
	int diagnostico FK ""
}
```
 