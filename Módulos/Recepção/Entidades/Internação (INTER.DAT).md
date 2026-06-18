#entidade
## Arquivos:
- INTER.DAT
- INTER5.DAT
- PACIT.DAT ([[Paciente (PACIT.DAT, PACIT2.DAT, PACIT3.DAT)]])
- PACIT2.DAT ([[Paciente (PACIT.DAT, PACIT2.DAT, PACIT3.DAT)]])
- PACIT3.DAT ([[Paciente (PACIT.DAT, PACIT2.DAT, PACIT3.DAT)]])
- CLAS.DAT ([[Classificação (CLAS.DAT)]])
- DIAG.DAT ([[Diagnóstico (DIAG.DAT)]])
- MED.DAT ([[Médico (MED.DAT)]])
- CONSU.DAT ([[Consumidor (CONSU.DAT)]])
- CLI.DAT ([[Especialidade (CLI.DAT)]])
- SET.DAT ([[Setor (SET.DAT)]])
- ALTA.DAT ([[Alta (ALTA.DAT)]])

---

## Entidade:
```mermaid
erDiagram

INTERNACAO {
	int codigo PK "INTER.DAT | codigo"
	int paciente FK "PACIT.DAT | registro"
	string responsavel FK "PACIT.DAT | responsavel"
	int data_entrada "INTER.DAT | dentrada"
	int horas "INTER.DAT | horas"
	int encaminhamento "INTER.DAT | encaminhamento"
	int classificacao FK "CLAS.DAT | codigo"
	int diagnostico FK "DIAG.DAT | codigo"
	int clinica FK "CLI.DAT | codigo"
	int medico FK "MED.DAT | codigo"
	int leito FK "CONSU.DAT | codigo"
	int tem_guia "CONSU.DAT | temguia"
}
```

### Valores predefinidos:
#### encaminhamento
- 0 = Cons.
- 1 = H.M.I.
- 2 = P. Saude
- 3 = P. Soc.
- 4 = Prefei.
- 5 = H. Iv.
- 6 = H. Fora
- 7 = Outros
