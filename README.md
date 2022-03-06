## Tera Clustering Ifood Challenge

- WIP

### Variables Documentation:

#### Orders

| order_id             | ID único para pedido                                                                                                                                                                |
|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| order_shift          | 0 - 4:59h - weekday/weekend dawn 5 - 9:59h - weekday/weekend breakfast 10 - 14:59h - weekday/weekend lunch 15 - 16:59h - weekday/weekend snack 17 - 23:59h - weekday/weekend dinner |
| order_origin         | Tipo do Merchant: STORE (loja), QUICKLY_MEAL (refeição rápida e barata), RESTAURANT (restaurante)                                                                                   |
| delivery_fee         | Taxa de entrega paga pelo cliente                                                                                                                                                   |
| scheduled            | Booleano que indica se o pedido foi agendado                                                                                                                                        |
| total_amount         | Valor total pago pelo cliente (em Unidades Monetárias UM)                                                                                                                           |
| subsidy_amount       | Subsídio, desconto dado no pedido (em Unidades Monetárias UM) - (para o valor final total do pedido: total_amount + subsidy)                                                        |
| device_platform      | Plataforma (sistema operacional) utilizado para fazer o pedido (ANDROID, DESKTOP, etc)                                                                                              |
| device_type          | Canal de origem do pedido (SITE, MOBILE, etc)                                                                                                                                       |
| device_app_version   | Versão do aplicativo do iFood que fez o pedido                                                                                                                                      |
| centroid_id          | Id da centroide do clientes                                                                                                                                                         |
| state_label          | Sigla da UF do cliente                                                                                                                                                              |
| city                 | Cidade do cliente                                                                                                                                                                   |
| district             | Bairro do cliente                                                                                                                                                                   |
| customer_long        | Longitude do cliente (até 2ª casa decimal) - ~1km                                                                                                                                   |
| customer_lat         | Latitude do cliente (até 2ª casa decimal) - ~1km                                                                                                                                    |
| restaurant_id        | Identificador do restaurante                                                                                                                                                        |
| dish_type            | Tipo de cozinha                                                                                                                                                                     |
| group_id             | Se o restaurante fizer parte de um grupo, essa é a identificação do grupo                                                                                                           |
| merchant_centroid_id | Id da centroide                                                                                                                                                                     |
| merchant_state       | Sigla do UF do Merchant                                                                                                                                                             |
| merchant_city        | Cidade do Merchant                                                                                                                                                                  |
| merchant_district    | Distrito do Merchant                                                                                                                                                                |
| merchant_zipcode     | CEP do Merchant                                                                                                                                                                     |
| merchant_long        | Longitude do Merchant (até 2ª casa decimal)                                                                                                                                         |
| merchant_lat         | Latitude do Merchant (até 2ª casa decimal)                                                                                                                                          |
| has_free_delivery    | Booleano que indica se o pedido foi entrega gratis                                                                                                                                  |
| confirmed_date       | Data que o pedido foi confirmado pelo restaurante                                                                                                                                   |
| concluded_date       | Data em que o pedido foi concluído                                                                                                                                                  |
| lag_last_order       | Tempo em dias entre o pedido atual e o último pedido do cliente                                                                                                                     |
| account_id           | ID do usuário                                                                                                                                                                       |