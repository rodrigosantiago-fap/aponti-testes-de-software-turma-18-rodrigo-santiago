### O SGP é uma aplicação web utilizada por **clientes e administradores** para realizar e gerenciar pedidos de produtos online.
1. **Integrações**
- Integração com banco de dados de produtos
- Integração com serviço de autenticação
- Integração com serviço de pedidos

 2. **Funcionalidades principais**
- Cadastro e autenticação de usuários
- Consulta de produtos disponíveis
- Adição e remoção de itens no carrinho
- Cálculo automático do valor total do pedido
- Finalização do pedido com confirmação

3. **Regras de negócio**
- O pedido deve conter pelo menos um item
- O valor total deve considerar quantidade e preço dos produtos
- Usuários não autenticados não podem finalizar pedidos
- Após a confirmação, o pedido não pode ser alterado
---
#### Dado um sistema fictício, os alunos deverão analisar suas funcionalidades e indicar:

- **Quais testes seriam unitários:**
Testes unitários seriam realizados durante o desenvolvimento do software verificando partes do código e confirmando as entradas e saídas, esses testes podem ser realizados de forma automatizada ou manual para identificar possíveis falhas.\
**Ex:** Teste da função Cálculo automático do valor total do pedido.

- **Quais testes seriam de integração:**
  Os testes de integração seriam a combinação dos códigos desenvolvidos do software verificando a interação entre partes do sistema e para garantir as funcionalidades com segurança das aplicações.\
  **Ex:** O valor total deve considerar quantidade e preço dos produtos e Cálculo automático do valor total do pedido. Consulta de produtos disponíveis e Integração com banco de dados de produtos

- **Quais testes seriam de sistema:** Testes de sistema ocorrem após a fase de conclusão de desenvolvimento, simulando funções do sistema como ele deve e como não deve reagir de acordo com determinada solicitação de um usuário do sistema, esses testes acontecem através de validações em ambientes controlados em funcionalidades e regras do produto.\
 **Ex:** (Usuários não autenticados não podem finalizar pedidos) identificar se existe algum meio de realizar pedidos sem estar autenticado no sistema. (Finalização do pedido com confirmação) garantir a confirmação do pedido. (Adição e remoção de itens no carrinho) Identificar quantidade e valores de itens incluídos no carrinho.

- **Quais testes seriam de aceitação:** Nessa fase o teste servira para garantir a entrega de um produto de acordo como foi solicitado atendendo sua necessidade e utilização final.\
**Ex:** Realizado em colaboração com o cliente a utilização das funcionalidades do sistema para confirmar que sua entrega está de acordo com os requisitos esperados.

#### Justificar escolhas com base no objetivo e no nível do teste


