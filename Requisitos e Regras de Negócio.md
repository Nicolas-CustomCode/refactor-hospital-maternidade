## Requisitos Funcionais

### 👤 Pacientes

- RF01 - O sistema deve permitir cadastrar pacientes usando seus dados básicos
- RF02 - O sistema deve permitir consultar pacientes
- RF03 - O sistema deve permitir atualizar dados cadastrais de pacientes
- RF04 - O sistema deve permitir pesquisar pacientes por nome, CPF ou registro
- RF05 - O sistema deve exibir histórico de internações do paciente

---

### 🩺 Médicos e Especialidades

- RF06 - O sistema deve permitir cadastrar médicos
- RF07 - O sistema deve permitir vincular médicos a especialidades
- RF08 - O sistema deve permitir consultar médicos cadastrados
- RF09 - O sistema deve permitir manter especialidades médicas

---

### 🏥 Setores e Leitos

- RF10 - O sistema deve permitir cadastrar setores hospitalares
- RF11 - O sistema deve permitir cadastrar leitos
- RF12 - O sistema deve permitir consultar situação dos leitos
- RF13 - O sistema deve permitir bloquear leitos indisponíveis
- RF14 - O sistema deve permitir visualizar leitos ocupados e livres

---

### 🛏️ Internação

- RF15 - O sistema deve permitir registrar internamentos
- RF16 - O sistema deve permitir vincular pacientes a leitos
- RF17 - O sistema deve permitir transferir pacientes entre leitos
- RF18 - O sistema deve permitir transferir pacientes entre setores
- RF19 - O sistema deve permitir consultar pacientes internados
- RF20 - O sistema deve permitir registrar motivo da internação
- RF21 - O sistema deve permitir consultar o total de internamentos por convênios

---

### ✅ Alta Hospitalar

- RF22 - O sistema deve permitir registrar alta hospitalar
- RF23 - O sistema deve liberar automaticamente o leito após alta
- RF24 - O sistema deve registrar data e hora da alta
- RF25 - O sistema deve permitir consultar histórico de altas

---

### 🚑 Emergência

- RF26 - O sistema deve permitir cadastrar atendimentos de emergência/urgência
- RF27 - O sistema deve permitir consultar histórico de atendimentos de emergência/urgência
- RF28 - O sistema deve permitir cadastrar laudos para solicitação de autorização de internação hospitalar (AIH)
- RF29 - O sistema deve permitir consultar laudos para solicitação de autorização de internação hospitalar (AIH)
- RF30 - O sistema deve permitir registrar atendimento ambulatorial
- RF31 - O sistema deve permitir consultar histórico de atendimento ambulatorial

---

### 💊 Clínica

- RF32 - O sistema deve permitir registrar consultas clínicas
- RF33 - O sistema deve permitir consultar histórico de consultas clínicas

---

### 💰 Financeiro

- RF34 - O sistema deve permitir registrar faturas
- RF35 - O sistema deve permitir consultar histórico de faturas
- RF36 - O sistema deve permitir registrar contas de consultas
- RF37 - O sistema deve permitir consultar histórico de contas de consultas

---














## Regras de Negócio

- RN01 – Um leito não pode possuir mais de um paciente simultaneamente
- RN02 – Apenas pacientes internados podem receber alta
- RN03 – O CPF do paciente deve ser único
- RN04 – Um leito bloqueado não pode receber internações
- RN05 – A transferência deve liberar automaticamente o leito anterior







### 💰 Financeiro

- RF25 - O sistema deve permitir registrar despesas hospitalares
- RF26 - O sistema deve permitir registrar cobranças de internação
- RF27 - O sistema deve gerar relatórios financeiros
- RF28 - O sistema deve permitir consultar faturamentos por período

---

### 📦 Estoque / Materiais

- RF29 - O sistema deve permitir cadastrar itens de estoque
- RF30 - O sistema deve registrar entradas de materiais
- RF31 - O sistema deve registrar saídas de materiais
- RF32 - O sistema deve informar quantidade disponível em estoque
- RF33 - O sistema deve alertar sobre estoque mínimo

---

### 📊 Relatórios e Estatísticas

- RF34 - O sistema deve gerar relatório de internações
- RF35 - O sistema deve gerar relatório de ocupação de leitos
- RF36 - O sistema deve gerar relatório de altas hospitalares
- RF37 - O sistema deve permitir consultar estatísticas hospitalares

---

### 🔐 Usuários e Acesso

- RF38 - O sistema deve permitir autenticação de usuários
- RF39 - O sistema deve permitir cadastrar usuários do sistema
- RF40 - O sistema deve permitir definir permissões de acesso
- RF41 - O sistema deve registrar logs de operações realizadas