# Exercício 4 — Testes de sistema 
Elabore pelo menos quatro cenários completos, executados pela interface do 
sistema. 

## Cenário A — Atendimento completo 
1. Cadastrar um paciente. 
2. Localizar o paciente pela pesquisa. 
3. Realizar um agendamento. 
4. Fazer o check-in. 
5. Registrar a evolução da sessão. 
6. Lançar a receita. 
7. Conferir o relatório financeiro.

## ATENDIMENTO COMPLETO
PRÉ-CONDIÇÕES | DADOS ULTILIZADOS | PASSOS | RESULTADO ESPERADO | RESULTADO OBTIDO | SITUAÇÃO | EVIDÊNCIA | JUSTIVICATIVA DA CLASSIFICAÇÃO
--------------|-------------------|--------|--------------------|------------------|----------|-----------|-------------------------------
TER ACESSO AO SISTEMA ESTA LOGADO COM LOGIN E SENHA |NOME: RODRIGO GOMES SANTIAGO EMAIL: RODRIGO@GMAIL.COM CPF:12345678601 TEL81988888888| CADASTRAR PACIENTE / NOVO REGISTRO / DADOS DO PACIENTE / SALVAR REGISTRO / REALIZAR PESQUISA CHECK-IN / | PACIENTE CADASTRADO E REGISTRADO PARA CHECK-IN | PACIENTE CADASTRADO NÃO IDENTIFICADO PARA CHECK-IN |REPROVADO| PRINT DA TELA |SISTEMA NÃO LOCALIZA PACIENTE PARA REALIZAR CHECK-IN
TER ACESSO AO SISTEMA ESTA LOGADO COM LOGIN E SENHA |NOME: RODRIGO GOMES SANTIAGO EMAIL: RODRIGO@GMAIL.COM CPF:12345678601 TEL81988888888| CADASTRAR PACIENTE / NOVO REGISTRO / DADOS DO PACIENTE / SALVAR REGISTRO / REALIZAR NOVO CHECK-IN / | PACIENTE CADASTRADO E LOCALIZADO PARA CHECK-IN | PACIENTE CADASTRADO PARA CHECK-IN | APROVADO | PRINT DA TELA |SISTEMA REALIZA NOVO CHECK-IN DE AGENDAMENTO COM SUCESSO
TER ACESSO AO SISTEMA ESTA LOGADO COM LOGIN E SENHA |NOME: RODRIGO GOMES SANTIAGO EMAIL: RODRIGO@GMAIL.COM CPF:12345678601 TEL81988888888| CAMPO EVOLUÇÃO DE SESSÃO | RECEITA CADASTRADA | EVOLUÇÃO DE SESSÃO CADASTRADA | APROVADO | PRINT DA TELA | SISTEMA REALIZA REGISTRO DE EVOLUÇÃO DE SESSÃO COM SUCESSO
TER ACESSO AO SISTEMA ESTA LOGADO COM LOGIN E SENHA | SEM DADOS | CAMPO RECEITAS | DADOS CADASTRADOS  | REGISTRO DE RECEITA CADASTRADA | APROVADO | PRINT DA TELA | SISTEMA REALIZA REGISTRA LANÇAMENTO DA RECEITA COM SUCESSO
TER ACESSO AO SISTEMA ESTA LOGADO COM LOGIN E SENHA | SEM DADOS | CAMPO RELATÓRIO FINANCEIRO | REGISTRO DO RELATORIO E CAMPO DE IMPRESSÃO | RELATORIO DISPONIVEL | APROVADO | PRINT DA TELA | SISTEMA FORNECE RELATORIO FINANCEIRO COM SUCESSO



## Cenário B — Reagendamento 
1. Criar um agendamento. 
2. Reagendar a consulta. 
3. Verificar a liberação do horário anterior. 
4. Verificar a ocupação do novo horário. 
5. Conferir os dados apresentados na agenda.
## REAGENDAMENTO
PRÉ-CONDIÇÕES | DADOS ULTILIZADOS | PASSOS | RESULTADO ESPERADO | RESULTADO OBTIDO | SITUAÇÃO | EVIDÊNCIA | JUSTIVICATIVA DA CLASSIFICAÇÃO
--------------|-------------------|--------|--------------------|------------------|----------|-----------|-------------------------------
   
## Cenário C — Controle de estoque 
1. Cadastrar um produto. 
2. Registrar uma entrada. 
3. Registrar uma saída. 
4. Verificar a quantidade final. 
5. Verificar o alerta de estoque mínimo. 
## Cenário D — Controle de acesso 
1. Criar perfis com diferentes permissões. 
2. Entrar como recepcionista. 
3. Tentar acessar prontuários. 
4. Entrar como psicólogo. 
5. Verificar se o acesso autorizado funciona. 
Para cada cenário, os alunos devem registrar: 
● pré-condições; 
● dados utilizados; 
● passos; 
● resultado esperado; 
● resultado obtido; 
● situação: aprovado ou reprovado; 
● evidência; 
● justificativa da classificação. 
O teste é de sistema porque avalia o sistema completo, por meio de um fluxo 
semelhante ao realizado pelo usuário final. 
