Atividade Avaliativa :
Praticar a criação, diferenciação e análise de casos de teste de sistema e de aceitação, utilizando uma estrutura padronizada e justificando tecnicamente cada escolha.  
---
## ETAPA 1 - Compreensão do Cenário um sistema bancário permite que usuários realizem login, acessem sua conta e visualizem seu saldo atual.  
---
**Tarefa:**
- **IDENTIFICAR:**

1. **FUNCIONALIDADES ENVOLVIDAS:**
- TELA DE LOGIN
- LOGIN COM AS CREDENCIAIS DO USUÁRIO (CPF) E SENHA
- LOGIN COM BIOMETRIA DO USUÁRIO
- CADASTRO DE NOVO USUÁRIO
- REDEFINIR SENHA DO USUÁRIO
- TROCAR USUÁRIO
- ÍCONE DE DÚVIDAS

2. **FLUXO PRINCIPAL:**
- F01 - ACESSO A DE TELA LOGIN
- F02 - INSERIR USUÁRIO E SENHA VALIDOS
- F03 - USUÁRIO VÁLIDADO
- F03 - USUÁRIO É DIRECIONADO PARA TELA INICIAL
- F04 - USUÁRIO TEM ACESSO A TELA INICIAL E VIZUALIZA SALDO

3. **VARIAÇÕES DE FLUXO:**
- F01 - LOGIN: USUÁRIO E SENHA INCORRETAS
- F02 - LOGIN: USUÁRIO AGENCIA/CONTA E SENHA DO INTERNET BANK
- F02 - USUÁRIO E SENHA INVALIDOS MAIS DE 3 VEZES USUÁRIO PRECISARA REALIZAR RECONHECIMENTO FACIAL, AGUARDAR 30 MINUTOS OU ENTRAR EM CONTATO COM A CENTRAL DO BANCO
- F02 - SISTEMA INDISPONIVEL
- F03 - USUÁRIO NÃO IDENTIFICADO EM CADASTRO BIOMETRICO
- F05 - USUÁRIO COM SALDO OCULTO
- ---

## ETAPA 2 - Escrever Testes de Sistema  
- 2 testes de fluxo principal (caminho feliz)
- 2 testes de fluxo alternativo
 
**Estrutura obrigatória**
- ID, Título, Pré-condições, Passos, Resultado esperado

**Orientações**  
- Foco no funcionamento do sistema
- Validar Integração entre telas
- Não validar regras de negócio complexas

## FLUXO PRINCIPAL (caminho feliz)  
## ID: TESTE01  

- **TÍTULO:** LOGIN COM CREDENCIAIS VALIDAS  

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO ESTAR CADASTRADO NA BASE DO SISTEMA COM LOGIN E SENHA VÁLIDO
02. USUÁRIO ESTAR COM ACESSO AO APLICATIVO OU INTERNET BANK

- **PASSOS DO TESTE:** 
01. **PASSO01:** INSERIR DADOS DE USUÁRIO VÁLIDO (CPF)
02. **PASSO02:** INSERIR SENHA VÁLIDA
03. **PASSO03:** CLICAR EM ENTRAR
04. **PASSO04:** AGUARDAR SISTEMA CARREGAR TELA INICIAL
05. **PASSO05:** SALDO VIZIVEL NA TELA INICIAL

- **RESULTADO ESPERADO:** USUÁRIO AUTORIZADO E SALDO DISPONIVEL NA TELA INICIAL
---
## ID: TESTE02  

- **TÍTULO:** LOGIN COM BIOMETRIA

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO ESTAR CADASTRADO NA BASE DO SISTEMA COM LOGIN E SENHA VÁLIDO
02. USUÁRIO ESTAR CADASTRADO COM BIOMETRIA 
03. USUÁRIO ESTAR COM ACESSO AO APLICATIVO OU INTERNET BANK

- **PASSOS DO TESTE:** 
01. **PASSO01:** INSERIR DADOS DE USUÁRIO VÁLIDO (CPF)
02. **PASSO02:** INSERIR DADOS BIOMETRICOS
04. **PASSO03:** AGUARDAR SISTEMA CARREGAR TELA INICIAL
05. **PASSO04:** SALDO VIZIVEL NA TELA INICIAL

- **RESULTADO ESPERADO:** SISTEMA DA ACESSO AO USUÁRIO AUTORIZADO VIA BIOMETRIA E SALDO DISPONIVEL NA TELA INICIAL

## FLUXO ALTERNATIVO

## ID: TESTE01  

- **TÍTULO:** LOGIN COM ID DE USUÁRIO VÁLIDO E SENHA INVÁLIDA

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO ESTAR CADASTRADO NA BASE DO SISTEMA COM LOGIN E SENHA VÁLIDO
02. USUÁRIO ESTAR COM ACESSO AO APLICATIVO OU INTERNET BANK

- **PASSOS DO TESTE:** 
01. **PASSO01:** INSERIR DADOS DE USUÁRIO VÁLIDO (CPF)
02. **PASSO02:** INSERIR SENHA INVÁLIDA
03. **PASSO03:** CLICAR EM ENTRAR
04. **PASSO04:** SISTEMA SUGERE CADASTRO DE BIOMETRIA
05. **PASSO05:** AGUARDAR RESPOSTA DO SISTEMA
06. **PASSO06:** SISTEMA INFORMA DADOS INVÁLIDOS

- **RESULTADO ESPERADO:** SISTEMA NÃO É AUTORIZA ACESSO E TELA EXIBE MENSAGEM DADOS DO USUÁRIO INVÁLIDOS

- ## ID: TESTE02  

- **TÍTULO:** LOGIN COM ID DE USUÁRIO VÁLIDO, SENHA INVÁLIDA E DADOS BIOMETRICOS VALIDO CADASTRADO

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO ESTAR CADASTRADO NA BASE DO SISTEMA COM LOGIN E SENHA VÁLIDO
02. USUÁRIO ESTAR CADASTRADO NA BASE DO SISTEMA COM DADOS BIOMETRICO
03. USUÁRIO ESTAR COM ACESSO AO APLICATIVO OU INTERNET BANK

- **PASSOS DO TESTE:** 
01. **PASSO01:** INSERIR DADOS DE USUÁRIO VÁLIDO (CPF)
02. **PASSO02:** INSERIR SENHA INVÁLIDA
03. **PASSO03:** CLICAR EM ENTRAR
04. **PASSO04:** SISTEMA SUGERE ACESSO COM DADOS BIOMETRICO
05. **PASSO05:** USUÁRIO USA OS DADOS BIOMETRICO
04. **PASSO05:** AGUARDAR RESPOSTA DO SISTEMA
05. **PASSO05:** SALDO DISPONIVEL NA TELA INICIAL

- **RESULTADO ESPERADO:** SISTEMA DA ACESSO AO USUÁRIO COM SENHA INCORRETA, MAS COM CADASTRO BIOMETRICO VÁLIDO E SALDO FICA DISPONIVEL NA TELA INICIAL
- ---
## ETAPA 3 - Escrever Testes de Aceitação  
 **Foco em valor para usuário e expectativa do negócio**  
- 2 testes de fluxo principal (caminho feliz)
- 2 testes de fluxo alternativo
 
**Estrutura obrigatória**
  - ID, Título, Pré-condições, Passos, Resultado esperado
  
 **Orientações**
- Resultado esperado focado em valor entregue
- Critérios claros de aceitação
## FLUXO PRINCIPAL (caminho feliz)  
## ID: TESTE01  

- **TÍTULO:** LOGIN COM ACESSSO RÁPIDO E CLARO AO SALDO DISPONIVEL 

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO ESTAR CADASTRADO NA BASE DO SISTEMA COM LOGIN E SENHA VÁLIDO  

- **PASSOS DO TESTE:** 
01. **PASSO01:** INSERIR DADOS DE USUÁRIO (CPF) OU AGÊNCIA E CONTA E SENHA VÁLIDA
02. **PASSO03:** CLICAR EM ENTRAR PARA CONFIRMAR ACESSO
03. **PASSO05:** ACESSO A TELA INICIAL DO USUÁRIO E SALDO VIZIVEL

- **RESULTADO ESPERADO:** USUÁRIO TEM ACESSO A CONTA E O SALDO VIZIVELMENTE NA TELA INICIAL
---
## ID: TESTE02  

- **TÍTULO:** OCUTAÇÃO DA EXIBIÇÃO DO SALDO NA TELA INICIAL

- **PRÉ-CONDIÇÕES:**
01. **PASSO01:** INSERIR DADOS DE USUÁRIO (CPF) OU AGÊNCIA E CONTA E SENHA VÁLIDA
02. **PASSO03:** CLICAR EM ENTRAR PARA CONFIRMAR ACESSO
03. **PASSO05:** ACESSO A TELA INICIAL DO USUÁRIO E SALDO VIZIVEL

- **PASSOS DO TESTE:** 
01. **PASSO01:** USUÁRIO OPTA POR OCULTAR SALDO NA TELA INICIAL USANDO ICONE DE OLHO FECHADO
02. **PASSO02:** USUÁRIO TEM ACESSO A TELA INICIAL COM SALDO OCUTO

- **RESULTADO ESPERADO:** SISTEMA DA ACESSO AO USUÁRIO DEIXANDO O SALDO DA CONTA OCULTO FORNECENDO PRIVACIDADE AO USUÁRIO

## FLUXO ALTERNATIVO

## ID: TESTE01  

- **TÍTULO:** BLOQUEIO DO ACESSO DEVIDO ERRO DE SENHA

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO ESTAR COM ACESSO AO APLICATIVO OU INTERNET BANK NA TELA DE LOGIN  

- **PASSOS DO TESTE:** 
01. **PASSO01:** INSERIR DADOS DE USUÁRIO VÁLIDO (CPF), INSERE SENHA INVÁLIDA E CLIENTE NÃO POSSUI CADASTRO BIOMETRICO
02. **PASSO02:** CLICAR EM ENTRAR
03. **PASSO03:** SISTEMA INFORMA DADOS INVÁLIDOS  

- **RESULTADO ESPERADO:** SISTEMA NÃO AUTORIZA ACESSO A TELA INICIAL SEM DISPONIBILIZAR DADOS BANCARIOS DO USUÁRIO E EXIBE MENSAGEM DADOS DO USUÁRIO INVÁLIDOS SEM DEFINIÇÃO DE QUAL DADO ESTA INCORRETO

## ID: TESTE02  

- **TÍTULO:** ERRO DE INDISPONIBILIDADE DE LOGIN USUÁRIO COM DADOS VÁLIDO

- **PRÉ-CONDIÇÕES:**
01. USUÁRIO REALIZA LOGIN COM ID E SENHA VÁLIDO
02. SISTEMA COM INDISPONIBILIDADE MOMENTÂNEA

- **PASSOS DO TESTE:** 
01. **PASSO01:** USUÁRIO INSERIR DADOS DE ID E SENHA VÁLIDOS
02. **PASSO02:** CLICAR EM ENTRAR
03. **PASSO03:** SISTEMA COMUNICA POR MENSAGEM VIZIVEL INDISPONIBILIDADE MOMENTÂNEA DO SISTEMA  

- **RESULTADO ESPERADO:** SISTEMA NÃO É ENCERRADO. EXIBE MENSAGEM CLARA NA TELA DO USUÁRIO INFORMANDO INDISPONIBILIDADE MOMENTÂNEA DO SISTEMA E QUE A EQUIPE DE SUPORTE ESTA TRABALHANDO PARA O RETORNO DO SERVIÇO
---
## ETAPA 4 - Justificativa e Classificação
**Para cada caso de teste criado, deve responder:**
01. Por que este é um teste de sistema?
02. Por que este é um teste de aceitação?
- **Foco da justificativa:**  
Objetivo do teste  
Ponto de vista adotado  
Tipo de validação realizada
---
## TESTES DE SISTEMA
## FLUXO PRINCIPAL (caminho feliz)   

## ID: TESTE01  
**JUSTIFICATIVA:** É um teste de sistema pois é estruturado semelhante ao ambiente de produção aplicado a funcionalidade de login e esta sendo visto do ponto de vista do usuário, testando a funcionalidade do início ao final e seu comportamento esperado. 

## ID: TESTE02  
**JUSTIFICATIVA:** É um teste de sistema pois avalia a funcionalidade de validação biométrica demostrando o fluxo de forma estruturada pelo ponto de vista de um usuário e avalia a resposta da funcionalidade e fluxo correto.  

## TESTES DE SISTEMA
## (FLUXO ALTERNATIVO)  

## ID: TESTE01  
**JUSTIFICATIVA:** Avalia o fluxo alternativo da funcionalidade login do usuário com senha inválida integralmente pelo ponto de vista de um usuário, está sendo executado de maneira estruturada. 

## ID: TESTE02  
**JUSTIFICATIVA:** Avalia o fluxo alternativo da funcionalidade login do usuário com senha invalida e dados biométricos válido integralmente do ponto de vista de um usuário, executado de maneira estruturada e ao comportamento esperado da funcionalidade.

---  

## TESTES DE ACEITAÇÃO 
## FLUXO PRINCIPAL (caminho feliz)   

## ID: TESTE01  
**JUSTIFICATIVA:** Esse é um teste de aceitação pois demonstra a facilidade da funcionalidade para o usuário e atende a necessidade do cliente pensando na satisfação do cliente.

## ID: TESTE02  
**JUSTIFICATIVA:** Esse é um teste de aceitação pois demonstra a utilidade da funcionalidade que entrega para o usuário privacidade no uso da aplicação e atende a necessidade do cliente pensando na satisfação gerando valor ao negócio.

## TESTES DE ACEITAÇÃO 
## FLUXO ALTERNATIVO   

## ID: TESTE01  
**JUSTIFICATIVA:** Teste de aceitação que é voltado na experiência segura do usuário que utiliza a aplicação pois assegura que em casos de acessos não autorizados a aplicação demostra eficiência garantindo que os dados do cliente não ficaram expostos.

## ID: TESTE02  
**JUSTIFICATIVA:** Teste de aceitação que demonstra o comportamento do sistema em um cenário de indisponibilidade e seu comportamento diante do usuário explicando com clareza como o cliente deve se comporta diante desse comportamento do sistema.
