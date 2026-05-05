# PontoEletronico
Aplicação web front-end para controle de horas trabalhadas com suporte a múltiplos usuários e armazenamento persistente.
# Sistema de Ponto Eletrônico Web

Aplicação web para controle de jornada de trabalho de analistas, com registro de horários, validação por assinatura, armazenamento local e integração com Google Sheets.

**Acesse o sistema:**  
https://pontoeletronicor.netlify.app/

---

## Funcionalidades

### Gestão de registro de ponto
- Registro de:
  - Entrada
  - Saída para almoço
  - Retorno do almoço
  - Saída
- Fluxo guiado (não permite pular etapas)
- Controle de registro por dia

### Validação por assinatura
- Código individual por analista
- Validação obrigatória antes do início
- Sessão válida por 24h

### Armazenamento local
- Dados salvos no `localStorage`
- Continuidade do registro mesmo após fechar o navegador
- Limpeza automática de registros antigos (30 dias)

### Resumo automático
- Cálculo de:
  - Horas trabalhadas
  - Tempo de almoço

### Gestão de registros
- Visualização dos registros do dia
- Filtros por:
  - Nome
  - Status (completo/incompleto)
- Exportação em CSV
- Exclusão de registros

### Integração com Google Sheets
- Envio automático ao finalizar registro
- Sincronização manual
- Uso de Google Apps Script como API

---

## Tecnologias utilizadas

- **HTML5**
- **CSS3**
- **JavaScript (Vanilla)**
- **LocalStorage (persistência de dados)**
- **Google Apps Script (integração com planilhas)**
- **Netlify (deploy)**

---

## Lógica implementada

- Controle de fluxo sequencial de ações
- Gerenciamento de estado da aplicação (sessão atual)
- Persistência local com recuperação de sessão
- Validação de autenticação simples
- Manipulação dinâmica do DOM
- Cálculo de tempo com base em timestamps
- Integração com API externa (Google Sheets)

---

