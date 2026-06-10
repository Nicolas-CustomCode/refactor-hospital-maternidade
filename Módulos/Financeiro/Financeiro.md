#módulo
## Fluxo
1. Paciente chega
2. Realiza atendimento/admissão
3. Verifica convênio ou particular
4. Internação é aberta

5. Durante a internação:
	1. Registra procedimentos
	2. Registra medicamentos
	3. Registra materiais
	4. Registra taxas
	5. Registra diárias
	6. Registra uso de equipamentos
	7. Registra honorários médicos

6. Paciente recebe alta

7. Auditoria da conta
	1. Conferência dos lançamentos
	2. Correções
	3. Glosas internas

8. Faturamento
	1. Geração da conta hospitalar
	2. Geração do lote de faturamento
	3. Envio ao convênio ou cobrança ao paciente

9. Financeiro
	1. Recebimento do pagamento
	2. Conciliação bancária
	3. Controle de inadimplência
	4. Recurso de glosas
	5. Baixa financeira

---

## Requisitos:
O sistema deve:
### Contas:
- Cadastrar [[Conta]]
- Consultar [[Conta]]
- Alterar informações de [[Conta]] abertas
- Vincular [[Conta]] a [[Internação]]
### Exames:
- Cadastrar [[Exame]]
- Consultar [[Exame]]
- Alterar informações de [[Exame]]
- Vincular [[Exame]] a [[Itens da Conta]]
### Itens da Conta:
- Cadastrar [[Itens da Conta]]
- Consultar [[Itens da Conta]]
- Alterar [[Itens da Conta]]
- Vincular [[Itens da Conta]] a [[Conta]]

---

## Entidades:
- [[Exame]]
- [[Exames por Convênio]]
- [[Conta]]
- [[Itens da Conta]]