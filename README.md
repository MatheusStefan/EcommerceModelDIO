# DataBase Experience - Desafio de projeto - Refinando um projeto de Banco de Dados E-commerce
### Este projeto foi desenvolvido em parceria com a DIO. O objetivo é refinar um modelo de banco de dados de uma loja de e-commerce fictícia, previamente planejada.
Pontos que foram refinados:
- Cliente PJ e PF – Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
- Pagamento – Pode ter cadastrado mais de uma forma de pagamento;
- Entrega – Possui status e código de rastreio;

## Explicação das minhas escolhas
- Cliente PJ e PF : decidi criar instâncias para cada tipo de cliente. Embora o cliente possa ter os dois tipos de conta(PJ e PF), uma não pode ser vinculada à outra, criando assim uma relação 1:1.
- Pagamento: como podem existir várias formas de pagamento, decidi criar instâncias para cada tipo de pagamento que a loja aceitaria(cartão, boleto e dinheiro).
- Entrega : optei por criar uma instância para entrega e relacionar com o pedido e não o cliente, pois como o pedido já puxa os dados do cliente, eu só preciso recuperar as informações do cliente.

## A seguir o modelo desenhado

![Ecommerce ModelDIO](https://user-images.githubusercontent.com/86742293/192140974-7088b633-4811-4a64-b746-666800239eae.png)
