## Paciente

```mermaid
erDiagram
PACIENTE {
	int id PK
    int registro "UNIQUE"
    string func
    string nome
    string endereco
    string cidade
    string uf
    string cep
    date nascimento
    string telefone
    string celular
    string sexo
    string estado_civil
    string cor
    string religiao
    string profissao
    string pai
    string mae
    int convenio_id FK
    string rg "UNIQUE"
    string uf_rg
    date data_emissao_rg
    string naturalidade
    string cpf "UNIQUE"
    string ibge
    int responsavel_id FK
    string sispre
    date ultimo_internamento
    date obito
}
```

---

## Médico

```mermaid
erDiagram
MEDICO {
	int id PK
	int codigo "UNIQUE"
	string nome
	string celular
	string endereco
	string cidade
	string estado
	string cep
	string crm "UNIQUE"
	string cns "UNIQUE"
	string cbo
}

HORARIO_ATENDIMENTO {  
	int id PK
	int medico_id FK
	int especialidade_id FK
	int dia_semana
	time hora_inicio
	time hora_fim
}
```

---

## Setor

```mermaid
erDiagram
SETOR {
	int id PK
	string nome
}
```

---

## Quarto

```mermaid
erDiagram
QUARTO {
	int id PK
	int setor_id FK
	string numero
	string tipo
}
```

---

## Leito

```mermaid
erDiagram
LEITO {
	int id PK
	string codigo "UNIQUE"
	int quarto_id FK
	string status
}
```

---

## Especialidade

```mermaid
erDiagram
ESPECIALIDADE {
	int id PK
	string codigo "UNIQUE"
	string nome
	string descricao
	string tipo
	string status
}
```
---

## Internamento

```mermaid
erDiagram
INTERNAMENTO {
	int id PK
	string ordem
	int paciente_id FK
	string celular
	string responsavel
	string celular_responsavel
	date data_entrada
	string documento_aprovacao
	string encaminhamento
	int convenio_id FK
	int especialidade_id FK
	int medico_id FK
	int leito_id FK
	string segurado
	string tipo
}
```

---

## Convênio

```mermaid
erDiagram
CONVENIO {
	int id PK
	string codigo
	string nome
	string tipo
	string status
}
```

```mermaid
erDiagram
PACIENTE_CONVENIO {
	int id PK
	int paciente_id FK
	int convenio_id FK
	string carteirinha
	date validade
}
```

---

## Estado Geral

```mermaid
erDiagram
ESTADO_GERAL {
	int id PK
	string ordem
	string registro
	int leito_id FK
	string estado
}
```

---

## Alta

```mermaid
erDiagram
ALTA {
	int id PK
	string ordem "UNIQUE"
	int internamento_id FK
	string motivo
	date data_alta
}
```

---

## Responsável

```mermaid
erDiagram
RESPONSAVEL {
	int id PK
	string nome
	string celular
	string cep
	string cidade
	string uf
	string bairro
	string logradouro
	string numero
	string complemento
	string documento
	string obs
}
```

---

## Atendimento Clínico

```mermaid
erDiagram
CLINICO {
	int id PK
	int paciente_id FK
	int medico_id FK
	int especialidade_id FK
	int convenio_id FK
	int diagnostico_id FK
	date data_atendimento
	stirng observacao
	string status
}
```

---

## Emergência

```mermaid
erDiagram
EMERGENCIA {
	int id PK
	string senha
	int paciente_id FK
	date entrada
	string tipo
	string classificacao_risco
	string sintomas
	string status
	int medico_id FK
	int leito_id FK
	date saida
	string destino
}
```

---

## Diagnóstico

```mermaid
erDiagram
DIAGNOSTICO {
	int id PK
	string codigo "UNIQUE"
	string nome
	string cid "UNIQUE"
}
```

```mermaid
erDiagram
INTERNAMENTO_DIAGNOSTICO {
	int id PK
	int internamento_id FK
	int diagnostico_id FK
	string tipo
}
```

---

## Procedimento

```mermaid
erDiagram
PROCEDIMENTO {
	int id PK
	string codigo "UNIQUE"
	string nome
	string amb
	string ssm
	int porte
	int auxiliares
	string tipo
}
```

```mermaid
erDiagram
INTERNAMENTO_PROCEDIMENTO {
	int id PK
	int internamento_id FK
	int procedimento_id FK
	date data_procedimento
	int quantidade
}
```

---
