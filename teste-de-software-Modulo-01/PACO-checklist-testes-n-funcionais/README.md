# A Plataforma (PACO) é um sistema web que permite que usuários realizem o agendamento de consultas médicas de forma simples e segura, enquanto administradores gerenciam horários e atendimentos.

**Integrações**
- Sistema acessado via navegador web
- Usuários podem acessar por desktop, tablet ou celular
- Uso simultâneo por múltiplos usuários durante horários de pico

**Regras de negócio**
- Usuários devem estar autenticados para agendar consultas
- Não é permitido agendar dois horários simultâneos para o mesmo usuário
- Cancelamentos só podem ocorrer até 24h antes da consulta
- Dados pessoais devem ser protegidos conforme boas práticas de segurança

**Funcionalidades principais**
- Cadastro e autenticação de usuários
- Consulta de especialidades e profissionais disponíveis
- Agendamento, cancelamento e visualização de consultas
- Notificações de confirmação de agendamento
- Área administrativa para gestão de horários
---
## Dado um sistema proposto, os alunos deverão elaborar um checklist de testes não funcionais, cobrindo obrigatoriamente:
1. Performance
2. Segurança
3. Usabilidade
4. Compatibilidade

**Cada item do checklist deve indicar o que será verificado e qual o risco associado.**
---

**CHECKLIST DE TESTES NÃO FUNCIONAIS**
VERIFICADO | TESTE | RISCO
------|------------|------
Sistema Acessado via navegador web | Compatibilidade | Pode não funcionar corretamente via navegador web especifico
Usuários podem acessar por desktop, tablet ou celular | Compatibilidade| Sistema pode não funcionar corretamente ou apresentar erro em determinado dispositivo ou resolução de tela.
Usuários simultâneos | Performance | Queda, Lentidão, Sobrecarga
Usuários devem estar autenticados para agendar consultas | Segurança | Acesso ao sistema de pessoas não autorizadas
Dados pessoais devem ser protegidos conforme boas práticas de segurança | Segurança | Vazamento de dados
Cadastro e autenticação de usuários| Usabilidade / Segurança | Facilidade no cadastro de usuários e proteção contra falhas de cadastros ou cadastros indevidos
Consulta de especialidades e profissionais disponíveis | Usabilidade | Dificuldade ou erro em busca de um especialista ou profissional
Agendamento, cancelamento e visualização de consultas | Usabilidade | Erros ou nao localização de funções ou falhas de funcinalidades
Área administrativa para gestão de horários | Usabilidade | Falhas e conflitos de horários de atendimento ou escala de trabalho.
