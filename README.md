# Curso Full Cycle 3.0 - Clean Architecture

## Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes tecnologias:

- **Node.js**: Ambiente de execução de JavaScript no servidor.
- **TypeScript**: Superset do JavaScript que adiciona tipagem estática ao código.
- **Sequelize**: ORM para Node.js que facilita a interação com o banco de dados.
- **Express**: Framework web minimalista para construir a API.
- **Jest**: Framework de testes para JavaScript, utilizado para realizar testes unitários e de integração.
- **Supertest**: Biblioteca para fazer testes de APIs HTTP.
- **SWC**: Transpilador TypeScript altamente eficiente.
- **Nodemon**: Utilitário para reiniciar a aplicação automaticamente durante o desenvolvimento.

## Desafio 1. Use Cases para Product

#### Descrição

Implemente as operações de criação, busca, listagem e atualização para a entidade `Product`, de forma semelhante ao que foi feito para a entidade `Customer`. Cada operação deve ser estruturada como um *use case* e deve ser implementada de maneira clara e concisa. Após implementar os *use cases*, escreva testes de unidade e integração para garantir que as operações funcionem corretamente.

#### Requisitos

- Criar os *use cases* para as operações: `create`, `find`, `list`, `update` para a entidade `Product`.
- Implementar testes de unidade e integração para cada operação.
- Garantir que todos os testes passem com sucesso.

---

## Desafio 2. API de Products

#### Descrição

Implemente uma API para listar os produtos da base de dados, similar à implementação realizada para a listagem de `Customers`. A API deve ser capaz de retornar os produtos armazenados no banco de dados, respeitando boas práticas de design de APIs. Além disso, implemente um teste end-to-end para garantir que a API funcione corretamente.

#### Requisitos

- Implementar uma rota de API para a listagem de `Products`.
- Implementar testes automatizados end-to-end para garantir que a API de listagem funcione corretamente.
- A API deve retornar os produtos corretamente do banco de dados.

---

## Desafio 3. Notification Pattern em Products

#### Descrição

O padrão de notificação (Notification Pattern) é utilizado para acumular erros de forma centralizada, evitando a criação excessiva de exceções. Neste desafio, aplique esse padrão na entidade `Product`. Em vez de lançar exceções para erros de validação ou negócios, o padrão de notificação permite que você colete todos os erros e os retorne ao final do processo. Desenvolva testes automatizados para garantir que o padrão de notificação funcione corretamente, incluindo um teste que acumule dois erros ao mesmo tempo.

#### Requisitos

- Aplicar o padrão de notificação na entidade `Product` para lidar com erros de validação e de negócios.
- Criar um teste que simule dois erros acumulados ao mesmo tempo.
- Garantir que todos os erros sejam coletados corretamente pelo padrão de notificação.
- Implementar testes automatizados para garantir o bom funcionamento do padrão.

---

## Desafio 4. Validação de Products

#### Descrição

Implemente um processo de validação para a entidade `Product`, garantindo que o domínio esteja minimamente acoplado e que a validação seja executada de forma eficiente. A validação deve ser modular e fácil de integrar com outros componentes da aplicação, como repositórios e serviços. Após a implementação, execute todos os testes para garantir que a validação funcione corretamente.

#### Requisitos

- Implementar a validação de dados na entidade `Product`, incluindo as regras de negócio relevantes.
- Garantir que a validação seja desacoplada do restante do domínio.
- Verificar se todos os testes automatizados continuam passando após a implementação da validação.

---

## Como Rodar o Projeto
1. **Instalação de Dependências**<br>
  Para instalar as dependências. No terminal, no diretório do projeto, execute:
    
    ```bash
    npm install
    ```

2. **Rodar os Testes**<br>
  Para rodar os testes e garantir que tudo está funcionando corretamente, execute o seguinte comando:
    
    ```bash
    npm test
    ```

3. **Compilar o Projeto**<br>
  Para compilar o código TypeScript para JavaScript, execute:
    
    ```bash
    npm run tsc
    ```
