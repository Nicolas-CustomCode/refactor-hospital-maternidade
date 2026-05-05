## Descrição:
Usuário pode cadastrar novo médico ou ver os médicos já cadastrados.

A tela inicia com o formulário em branco e com os atalhos: [↵](#<kbd>↵</kbd>), [F10](#<kbd>F10</kbd>) e [ESC](#<kbd>ESC</kbd>).

Se informar o código de um setor já cadastrados, exibe o registro com os atalhos [F2](#<kbd>F2</kbd>), [F5](#<kbd>F5</kbd>), [F8](#<kbd>F8</kbd>), [↑](#<kbd>↑</kbd>), [↓](#<kbd>↓</kbd>).

Ao apertar [F5](#<kbd>F5</kbd>), os campos se tornam alteráveis e exibe os atalhos [F2](#<kbd>F2</kbd>) e [F4](#<kbd>F4</kbd>).

Se informar o código de um setor não cadastrado, mantém o campo em branco e exibe os atalhos [F2](#<kbd>F2</kbd>), [F3](#<kbd>F3</kbd>), [↑](#<kbd>↑</kbd>) e [↓](#<kbd>↓</kbd>).

---

## Campos:
#### Código
- Número
- Obrigatório
#### Nome
- Texto
#### Endereço
- Texto
#### Cidade
- Texto
#### Estado
- Texto
#### CEP
- Número
#### Res.
- Texto
#### Com.
- Texto
#### Bip
- Texto
#### CRM
- Número
#### CPF
- Número
- Obrigatório
#### Clínicas
- Texto
#### CNS
- Número
- Obrigatório
#### CBO
- Número
#### Horários e Locais de Atendimento
- Texto

---

## Entidade:
```mermaid
erDiagram
MEDICO {
	int codigo PK
	string nome "NULL"
	string endereco "NULL"
	string cidade "NULL"
	string estado "NULL"
	int cep "NULL"
	string res "NULL"
	string comp "NULL"
	string bip "NULL"
	int crm "NULL"
	int cpf "NOT NULL"
	string clinicas "NULL"
	int cns "NOT NULL"
	int cbo "NULL"
	string horario_local_atendimento "NULL"
}
```

---

## Atalhos:
#### <kbd>Esc</kbd>
- Volta ao menu
#### <kbd>F2</kbd>
- Retorna
#### <kbd>F3</kbd>
- Consulta alfabética / Cadastrar
#### <kbd>F4</kbd>
- Gravar
#### <kbd>F5</kbd>
- Alterar
#### <kbd>F8</kbd>
- Apagar
#### <kbd>F10</kbd>
- Imprimir
#### <kbd>↵</kbd>
- Entre com o registro
#### <kbd>↑</kbd>
- Anterior
#### <kbd>↓</kbd>
- Próximo
