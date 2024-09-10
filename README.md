# clean-arch-exercises

# Cadastro de Usuário

**Objetivo**: Implementar um CRUD básico de usuário, seguindo os princípios da Clean Architecture.

**Descrição**: Crie uma aplicação que permita adicionar, editar, listar e excluir usuários. Estruture a aplicação com camadas de **entidades**, **use cases**, **interfaces** (controladores e gateways), e **frameworks and drivers** (infraestrutura).

**Passos**:
1. Defina a entidade `User` com os atributos básicos (e.g., `id`, `name`, `email`).
2. Crie um **use case** para adicionar um usuário, garantindo que os campos obrigatórios sejam preenchidos.
3. Crie o repositório que simula a persistência dos dados (em memória ou um banco de dados simples).
4. Implemente os controladores e gateways que interagem com o use case e a camada de infraestrutura.

---

# Simulação de Pagamento

**Objetivo**: Implementar uma simulação de processamento de pagamento usando Clean Architecture.

**Descrição**: Crie um sistema de pagamento simples que aceite um pagamento de um cliente e, após isso, atualize o status de um pedido.

**Passos**:
1. Crie a entidade `Payment` com atributos como `orderId`, `amount`, `paymentMethod`, `status`.
2. Crie o **use case** para processar o pagamento e alterar o status do pedido.
3. Implemente uma interface de pagamento externo (como simular uma integração com uma API de pagamento).
4. Teste o fluxo completo de pagamento e atualização do pedido.

---

# Autenticação de Usuários

**Objetivo**: Implementar um sistema de login/logout usando Clean Architecture.

**Descrição**: Crie uma aplicação que permita o login e logout de usuários, garantindo que a lógica de autenticação siga o princípio de separação de camadas.

**Passos**:
1. Crie a entidade `User` com os atributos necessários para autenticação (e.g., `email`, `password`).
2. Crie o **use case** para autenticação (validação de credenciais).
3. Implemente a lógica de geração de token de sessão ou JWT no framework de infraestrutura.
4. Adapte o controlador para lidar com as requisições de login/logout.

---

# Gestão de Produtos

**Objetivo**: Criar um sistema de gerenciamento de produtos, focando na organização por categorias.

**Descrição**: Implemente um sistema que permita adicionar, editar e listar produtos, com a possibilidade de associá-los a categorias.

**Passos**:
1. Crie as entidades `Product` e `Category`, onde um produto pode pertencer a uma ou mais categorias.
2. Crie **use cases** para adicionar produtos e categorias, além de listar produtos por categoria.
3. Implemente o repositório para armazenar e recuperar produtos e categorias.
4. Desenvolva os controladores e gateways para realizar as operações de produtos e categorias.
