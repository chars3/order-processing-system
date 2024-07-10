# OrderProcessingSystem

## Plano de Trabalho

### Atividades

1. **Configuração do Ambiente**
   - Configurar Docker para MySQL, Node.js e RabbitMQ.
2. **Desenvolvimento da Aplicação**
   - Criar projeto Node.js.
   - Implementar serviço de consumo de mensagens do RabbitMQ.
   - Criar a base de dados no MySQL.
   - Modelar e implementar a base de dados.
3. **Desenvolvimento de Micro Serviço**
   - Criar micro serviço para consumir dados da fila RabbitMQ.
   - Processar e armazenar dados no MySQL.
4. **Desenvolvimento da API REST**
   - Implementar endpoints para:
     - Consultar valor total do pedido.
     - Consultar quantidade de pedidos por cliente.
     - Listar pedidos realizados por cliente.
5. **Testes**
   - Testar serviço de consumo de mensagens.
   - Testar API REST.
6. **Elaboração do Relatório Técnico**
   - Documentar implementação.
   - Explicar arquitetura e decisões técnicas.

## Instruções para Rodar o Projeto

### Estrutura do Projeto

Certifique-se de que a estrutura do seu projeto está organizada da seguinte forma:

```
OrderProcessingSystem/
│
├── docker-compose.yml
├── package.json
├── index.js
├── consumer.js
└── sql/
    └── init.sql
```

### Arquivo `docker-compose.yml`

Crie o arquivo `docker-compose.yml` na raiz do projeto com a configuração necessária para MySQL, Node.js e RabbitMQ.

### Arquivo `package.json`

Crie o arquivo `package.json` com as dependências e scripts necessários para o projeto Node.js.

### Arquivo `index.js`

Crie o arquivo `index.js` para iniciar o servidor Express.

### Arquivo `consumer.js`

Crie o arquivo `consumer.js` para consumir as mensagens do RabbitMQ e processar os pedidos.

### Arquivo `sql/init.sql`

Crie um diretório `sql` na raiz do projeto e dentro dele um arquivo `init.sql` com a estrutura do banco de dados.

### Rodando o Projeto

Para iniciar os serviços, execute o comando:

```bash
docker-compose up
```
