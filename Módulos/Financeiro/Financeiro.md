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
- Cadastrar [[Fatura]]
- Consultar [[Fatura]]
- Alterar informações de [[Fatura]] abertas
- Vincular [[Fatura]] a [[Internação (INTER.DAT)]]
### Exames:
- Cadastrar [[Exame (EXAME.DAT)]]
- Consultar [[Exame (EXAME.DAT)]]
- Alterar informações de [[Exame (EXAME.DAT)]]
- Vincular [[Exame (EXAME.DAT)]] a [[Item da Conta]]
### Itens da Conta:
- Cadastrar [[Item da Conta]]
- Consultar [[Item da Conta]]
- Alterar [[Item da Conta]]
- Vincular [[Item da Conta]] a [[Fatura]]

---

## Entidades:
- [[Exame (EXAME.DAT)]]
- [[Exame por Convênio]]
- [[Fatura]]
- [[Item da Conta]]