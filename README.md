
# Desafio Metrito - 2023.1

<img src="https://metrito-public.s3.sa-east-1.amazonaws.com/metrito-white-vector.svg" height="35">

## Descrição do desafio
Neste desafio de programação, você terá que construir um aplicativo web que irá consultar a API da Hotmart e trazer dados de pedidos. Em seguida, esses dados serão normalizados para um determinado esquema e disponibilizados em uma API criada em Node.js. O aplicativo web poderá ser construído com qualquer tecnologia de front-end de sua preferência (React é uma opção) e o back-end deverá ser escrito em Node.js . 

Além disso, será necessário realizar o deploy da aplicação web e da API em um serviço de hospedagem em nuvem como o Heroku, AWS ou outro de sua preferência.

## Objetivo
O objetivo do desafio é avaliar a qualidade do código, especialmente no back-end. Portanto, será importante que você demonstre suas habilidades em escrever código limpo e organizado. No entanto, suas habilidades em front-end também serão avaliadas e levadas em consideração, portanto, uma bom front-end pode ser um diferencial e lhe trazer alguma vantagem.


## Etapas

- Consulta da API da Hotmart:
Você deverá criar uma aplicação em Node.js para consultar a API da Hotmart, usando as credenciais fornecidas. A consulta deverá trazer dados de pedidos, como nome do cliente, email, data do pedido, valor do pedido, etc.

- Normalização dos dados:
Os dados trazidos pela API da Hotmart precisam ser normalizados para um determinado esquema. Você deverá criar uma função em Node.js para fazer a normalização desses dados. O esquema que os dados devem ser normalizados será fornecido.

- API em Node.js:
Você deverá criar uma API em Node.js para disponibilizar os dados normalizados. Essa API deverá receber requisições de um aplicativo web e retornar os dados normalizados em formato JSON.

- Aplicativo web:
Você deverá criar um aplicativo web com a tecnologia de front-end de sua preferência (React é uma opção). O aplicativo deverá fazer uma requisição para a API criada em Node.js e exibir os dados normalizados para o usuário final.

- Deploy:
Você deverá fazer o deploy da aplicação web e da API em um serviço de hospedagem em nuvem como o Heroku, AWS ou outro de sua preferência.

## Dados de referência

Link da documentação da API utilizada no projeto:
[documentação da Hotmart API](https://developers.hotmart.com/docs/en/)

Período de seleção dos dados: 01/04/2021 a 30/05/2021 (A API retornará dados de compras nesse período)

Credenciais:
- client_id: ``dc02c371-8cd9-4067-821f-ae296dfdbadc``
- client_secret: ``81b20d9c-14dc-4fa5-9833-8694d2a8019b`` 
- token: (Basic): ``ZGMwMmMzNzEtOGNkOS00MDY3LTgyMWYtYWUyOTZkZmRiYWRjOjgxYjIwZDljLTE0ZGMtNGZhNS05ODMzLTg2OTRkMmE4MDE5Yg==``

Esquema desejado após normalização dos dados:
```
[
    {
          "identification": {
            "data_source": "HOTMART",
            "order_id": "String"
          },
          "transaction": {
            "status": "failed",
            "created_date": "2023-01-13T20:48:39Z",
            "updated_date": "2023-01-13T20:48:39Z",
            "value": 19700,
            "discount_value": Number,
            "freight": Number,
            "freight_type": String,
            "payment_type": "credit_card",
            "payment_card_brand": String,
            "payment_line": String,
            "payment_bar_code": String,
            "payment_url": String,
            "billet_url": String,
            "pix_qrcode": String,
            "pix_emv": String,
            "pix_ref": String,
            "pix_expiration_date": String,
            "pix_creation_date": String,
            "pix_url": String,
            "is_upsell": String
          },
          "product": {
            "bundles": [
              {
                "id": "or_m4AO7q5hbHbnjbzl",
                "name": "Pedido teste 2",
                "quantity": 1,
                "price": Number,
                "products": [
                  {
                    "id": "oi_VvqX66t1qIy5Xla0",
                    "name": "Pedido teste 2",
                    "quantity": Number,
                    "price": Number
                  }
                ]
              }
            ]
          },
          "producer": {
            "name": String,
            "document": String,
            "email": String,
            "tel": String
          },
          "customer": {
            "id": "cus_VQYMNj8tvdudgMp0",
            "name": "Matheus Barbosa",
            "email": "matheus@metrito.com",
            "telephone": String,
            "document": String
          },
          "comission": {
            "comissions_list": Array,
            "co_production_commission": Array
          },
          "metadata": {
            "affiliate_id": String,
            "utm_source": String,
            "utm_medium": String,
            "utm_campaign": String
          }
        }
      ]
```
Observação: caso a API não retorne dados para algum campo especificado, o campo deverá ser 'null'.


## Critérios de avaliação:

- Organização e qualidade do código no back-end.
- Qualidade do código no front-end.
- Capacidade de normalizar os dados de acordo com um esquema fornecido.
- Capacidade de criar uma API em Node.js para disponibilizar os dados normalizados.
- Capacidade de fazer deploy para ambiente de produção
- Capacidade de realizar o deploy da aplicação web e da API em um serviço de hospedagem em nuvem.

## Dica:

Certifique-se de documentar seu código e fornecer instruções claras para executar o projeto.
Procure se diferenciar, adicionando funcionalidades extras e recursos adicionais.
Boa sorte e divirta-se com o desafio! 😉🚀
