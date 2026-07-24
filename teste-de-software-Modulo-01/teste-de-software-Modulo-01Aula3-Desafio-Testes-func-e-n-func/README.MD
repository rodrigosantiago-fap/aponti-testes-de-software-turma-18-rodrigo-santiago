# Exercício 5 — Testes de aceitação 
#### Elabore pelo menos cinco critérios de aceitação sob o ponto de vista da clínica ou de seus usuários. 
#### Use preferencialmente o formato: 
Dado que...  
Quando...  
Então...  

**Exemplo:**  
**Dado que** o paciente e o psicólogo estejam cadastrados,  
**quando** a recepcionista selecionar uma data e um horário disponível,  
**então** o sistema deverá registrar a consulta e exibi-la na agenda do 
psicólogo.  

Outras situações:  
- **impedir dois agendamentos para o mesmo psicólogo no mesmo horário;**   
Dado que a recepcionista selecione uma data e um horário para agendamento  
quando o sistema identificar que já existe agendamento no mesmo período para o mesmo psicólogo  
então deverá apresentar uma mensagem que informa que essa data já está atribuída para outro paciente agendado e que devera ser selecionada outra data, horário e psicólogo  

- **permitir que somente psicólogos autorizados consultem prontuários;**  
Dado que o psicólogo teve seu acesso autorizado pelo sistema  
quando realizar consulta de prontuários  
então o sistema deverá permitir acesso a consulta de prontuários de acordo com seu nível de autorização  

- **atualizar o saldo após o lançamento de receita ou despesa;**  
Dado quando for realizado lançamento de receitas ou despesas  
quando o usuário registrar esse lançamento  
então o sistema deverá realizar a atualização do saldo no fluxo financeiro  

 
- **alertar quando um produto atingir o estoque mínimo;**  
Dado um produto atingiu o estoque mínimo  
quando o sistema identificar retiradas do produto que estiver dentro do limite mínimo no estoque  
então o sistema deverá apresentar alertas sempre que esse item for retirado  

- **preservar os dados após o usuário sair e entrar novamente;**  
Dado um usuário encerre sua sessão no sistema clicando em sair  
quando o usuário optar em salvar seus dados de login apos sair e retornar ao sistema  
então o sistema deverá salvar o registro de login do usuário sendo necessário à validação com senha  

- **permitir a localização de pacientes por nome ou CPF.**  
Dado um funcionário com acesso autorizado  
quando solicitar busca usando nome ou CPF no sistema de paciente devidamente cadastrado  
então o sistema deverá apresentar registros de status de agendamentos  

A justificativa deve explicar que o teste de aceitação verifica se o sistema atende às 
necessidades do negócio e pode ser aprovado pelo cliente ou usuário responsável.
