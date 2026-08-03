# Atividade Avaliativa

- Dado um relatório de teste de performance, analise-o responder às seguintes questões:  
1. O sistema pode ser considerado aprovado?
2. Quais métricas indicam problemas de performance?
3. Quais possíveis gargalos podem existir?
4. Esse cenário se aproxima mais de Carga, Stress ou Capacidade?
5. O que você recomendaria ao time técnico?
---
### RELATORIO TESTE DE PERFORMANCE TELA DE LOGIN E TELA INICIAL   

**PROJETO:** NOVO SOFTWARE SISTEMA BANCARIO  
**FASE DO PROJETO:** TELA DE LOGIN / TELA INICIAL  
**OBJETIVO:** AVALIAÇÃO DO SISTEMA EM CONDIÇÃO NORMAL DE USO E CAPACIDADE MAXIMA SUPORTADA ULTILIZANDO PROGRESSIVAMENTE O LIMITE MAXIMO DE ATÉ 50 USUÁRIO SIMULTÂNEOS E IDENTIFICANDO OS NIVEIS ACEITÁVEIS DE ULTILIZAÇÃO NOS TESTES INICAIS DE PERFORMANCE.  

**TEMPO DE RESPOSTA:** DURANTE OS TESTES O SISTEMA SUPORTOU COM QUALIDADE ACESSOS SIMULTÂNEOS ATÉ 25 USUÁRIO REALIZANDO A TRANSIÇÃO DE SOLICITAÇAÕ DAS FUNCIONALIDADES EM ATÉ 1 SEGUNDO. ACIMA DESSE NÚMERO ENTRE 26 E 35 USUÁRIO ESSE TEMPO AUMENTOU PARA 1,5 SEGUNDOS E ENTRE 35 E 50 USUÁRIO O TEMPO FICOU ENTRE 2 E 3,5 SEGUNDOS, ACIMA DO LIMITE ESPERADO DE 2 SEGUNDOS.  
**USO DA MEMÓRIA:** O CONSUMO DA MEMORIA SE MANTEVE ENTRE 45% E 55% DURANTE O USU SIMULTÂNEO ENTRE 20 E 35 USUÁRIOS, NO INSTANTE EM QUE O SISTEMA TEVE UM ACESSO SIMULTÂNEO ENTRE 40 E 50 USUÁRIOS O USO DA MEMORIA ATINGIU 97% OCASIONANDO TRAVAMENTO E NÃO FUNCIONAMENTO DE REQUISIÇÃO.  

**TAXA DE ERRO:** O SISTEMA REALIZOU COM BOA ESTABILIDADE QUANDO ATÉ 25 USUÁRIOS SIMULTÂNEOS REALIZANDO REQUISIÇÕES COM TAXA DE ERRO 0,4% E QUANDO ACIMA DE 26 USUÁRIOS AO LIMITE DE 50 USUÁRIOS SIMULTANEOS A TAXA DE ERROS FICOU ENTRE 2,7% E 4,5% DEMONSTRANDO UM LIMITE DE ACEITAÇÃO.  

Responder:  
- O sistema pode ser considerado aprovado?  
Pode ser parcialmente considerado aprovado, com pontos de melhoria o sistema precisa ainda de melhoramentos para suportar mais acessos simultâneos entre 30 e 50 usuários com qualidade.

- Quais métricas indicam problemas de performance?  
O tempo de resposta, o uso da memória e a taxa de erro quando acima de 35 acessos simultâneos indicam problemas de performance.

- Quais possíveis gargalos podem existir?  
Erros na transição de telas, problemas na identificação de dados de login, falhas em exibição de funcionalidades, lentidão.
 
- Esse cenário se aproxima mais de Carga, Stress ou Capacidade?  
Capacidade porque tentou testar o sistema ate sua capacidade máxima suportada ate esse momento da fase do projeto.

- O que você recomendaria ao time técnico?  
Realizar melhorias na capacidade de memoria suportada, simplificar interface da tela inicial.
