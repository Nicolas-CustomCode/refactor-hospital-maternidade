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
	int cidade FK "--COLUNA NÃO ENCONTRADA NO CIDADES.DAT--"
	string cep "--COLUNA NÃO ENCONTRADA NO CIDADES.DAT--"
	date data_nascimento "PACIT.DAT | nascimento"
	string(2) estado "--COLUNA NÃO ENCONTRADA NO CIDADES.DAT--"
	int telefone "PACIT2.DAT foner"
	int celular "PACIT2.DAT fonec"
	int sexo "PACIT.DAT | cod"
	int estado_civil "PACIT.DAT | cod"
	int cor "PACIT.DAT | cod"
	int religiao "PACIT.DAT | cod"
	string profissao "PACIT.DAT | profissao"
	string pai "PACIT.DAT | pai"
	string mae "PACIT.DAT | mae"
	int convenio FK "CLAS.DAT | codigo"
	int tipo_documento "PACIT2.DAT | doc"
	int numero_documento "PACIT2.DAT | numdoc"
	int rg "PACIT3.DAT | campo1"
	string(2) uf "PACIT3.DAT | campo2"
	date data_emissao ""
	string naturalidade ""
	string cpf "PACIT3.DAT | campo3"
	int ibge FK "PACIT2.DAT/ibge"
	string responsavel_nome "PACIT2.DAT | responsavel"
	string responsavel_endereco "PACIT2.DAT | endereco"
	int reponsavel_codigo_cidade FK "PACIT2.DAT/cidade | Referencia CIDADE.DAT/codigo"
	string(2) responsavel_estado "PACIT2.DAT | estado | Referencia CIDADE.DAT"
	int responsavel_telefone "PACIT2.DAT | fonerr"
	int responsavel_celular "PACIT2.DAT | fonec"
	int responsavel_tipo_documento "PACIT2.DAT | docr"
	int responsavel_numero_documento "PACIT2.DAT | numdocr"
	int sispre ""
	int ultima_internacao ""
	date obito ""
}
```

### Valores predefinidos:
#### sexo
- 1 = Masculino
- 2 = Feminino
#### estado_civil
- 1 = Casado
- 2 = Solteiro
- 3 = Viuvo
- 4 = Menor
- 5 = Separado
- 6 = Divorciado
#### religiao
- 1 = Catolico
- 2 = Evangelico
- 3 = Espirita
- 4 = T. Jeova
- 5 = Outros
#### documento
- 0 = Sem Doc.
- 1 = PIS/PASEP
- 2 = RG
- 3 = Cer. Nasc.
- 4 = CPF
- 5 = N. saude
- 6 = Outros

### Obs:
- `sexo`, `estado_civil`, `cor` e `religiao` estão juntos em `PACIT.DAT/cod`, nessa ordem