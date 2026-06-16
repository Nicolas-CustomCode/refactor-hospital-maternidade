#entidade 
## Entidade:
```mermaid
erDiagram
ITEM_CONTA {
	uuid id PK
	uuid conta_id FK
	uuid exame_convenio_id FK
	uuid diaria_convenio_id FK
	uuid medicamento_convenio_id FK
	uuid material_convenio_id FK
	uuid taxa_convenio_id FK
	decimal quantidade
	decimal valor_unitario
	decimal valor_total
}
```

%%
Quais tipos de item tem em uma conta hospitalar?
- [x] Exames
- [x] Diárias
- [x] Medicamentos
- [ ] Honorários
- [x] Raio-x (já se encaixa em exames no geral)
- [x] Taxas
- [x] Materiais
- [ ] Diversos
Marcar quais entidades já existem e podem ser colocadas na conta hospitalar
%%

---

## Entidades que se relaciona:
- [[Conta]]
- [[Exame por Convênio]]
- [[Diária por Convênio]]
- [[Material por Convênio]]
- [[Medicamento por Convênio]]