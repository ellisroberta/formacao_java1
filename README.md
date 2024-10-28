# Sistema de Pedidos em Java

Este projeto demonstra a aplicação de enumerações e serialização para um sistema de pedidos em Java.

## Funcionalidades

- Definição de estados do pedido usando Enum.
- Classe `Order` com serialização e deserialização.
- Registro de dados de clientes e itens de pedidos. 
- Cálculo de subtotal por item e total do pedido. 
- Exibição de um resumo do pedido com detalhes completos

## Exemplo de Funcionamento

Ao executar o programa, o usuário deverá inserir os dados conforme o exemplo abaixo:

``` Enter cliente data:
Name: Alex Green
Email: alex@gmail.com
Birth date (DD/MM/YYYY): 15/03/1985

Enter order data:
Status: PROCESSING
Enter #1 item data:
Product name: TV
Product price: 1000.00
Quantity: 1

Enter #2 item data:
Product name: Mouse
Product price: 40.00
Quantity: 2

ORDER SUMMARY:
Order moment: 28/10/2024 09:56:05
Order status: PROCESSING
Client: Alex Green (15/03/1985) - alex@gmail.com
Order Items:
TV, $1000.00, Quantity: 1, Subtotal: $1000.00
Mouse, $40.00, Quantity: 2, Subtotal: $80.00
Total price: $1080.00
```

## Estrutura de Classes

As classes são organizadas da seguinte forma:

- *Order*: Armazena informações sobre o pedido, incluindo data, status e itens.
- *Client*: Contém informações do cliente, como nome, e-mail e data de nascimento.
- *OrderItem*: Representa cada item do pedido e está associado a um produto.
- *Product*: Define o nome e o preço do produto.
- *OrderStatus*: Enum que contém os possíveis estados do pedido (PENDING_PAYMENT, PROCESSING, SHIPPED, DELIVERED).

## Como Executar

1. Certifique-se de ter o Java instalado.
2. Compile os arquivos `.java` usando `javac`.
3. Execute a classe `Program` para ver o exemplo de funcionamento.

## Dependências

- Java 17 ou superior
