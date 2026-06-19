#entidade
## Arquivos:
- MED.DAT
- CLI.DAT ([[Especialidade (CLI.DAT)]])

---

## Entidade:
```mermaid
erDiagram

MEDICO {
	int codigo PK "MED.DAT | codigo"
	string nome "MED.DAT | nome"
	string endereco "MED.DAT | endereco"
	string cidade "MED.DAT | cidade"
	string estado "MED.DAT | uf"
	int cep "MED.DAT | cep"
	string res
	string com "MED.DAT | fone"
	int crm "MED.DAT | doc"
	int cpf "MED.DAT | doc"
	int atendimento "MED.DAT | obs"
	int cns "MED.DAT | numA"
	int cbo "MED.DAT | numB"
	
	int clinicas1 FK "CLI.DAT | codigo"
	int clinicas2 FK "CLI.DAT | codigo"
}
```

### Obs:
- `crm` é os 5 primeiros dígitos de `MED.DAT/doc`
- `cpf` é a partir do 6º dígito de `MED.DAT/doc`
