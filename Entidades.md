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
    int convenio FK
    string numero_carteirinha
    string rg "UNIQUE"
    string uf_rg
    date data_emissao_rg
    string naturalidade
    string cpf "UNIQUE"
    string ibge
    string responsavel
    string endereco_responsavel
    string cidade_responsavel
    string uf_responsavel
    string telefone_responsavel
    string complemento_responsavel
    string documento_responsavel
    string numero_responsavel
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
	int clinica_id FK
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
	string codigo
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
	string cid
	string ssm
	string amb
	string numero_ch
	int porte
	int auxiliares
}
```

---

## Internamento
```mermaid
erDiagram
INTERNAMENTO {
	int id PK
	string ordem
	string paciente_id FK
	string responsavel_legal
	string celular
	date data_entrada
	string documento_aprovacao
	string encaminhamento
	string classificacao_id FK
	string diag
	string clinica_id FK
	string medico_id FK
	string leito_id FK
	string segurado
	int guia_id
	string tipo
}
```

---

## Convênio
```mermaid
erDiagram
CONVENIO {
	int id PK
	string nome
	string tipo
	string status
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
	string ordem
	int internamento_int FK
	int paciente_id FK
	int convenio_id FK
	int quarto_id FK
	string motivo
	date data_alta
}
```

---

## 