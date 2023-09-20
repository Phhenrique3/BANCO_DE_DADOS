[imagem_ze_delivrey](https://github.com/Phhenrique3/BD/assets/127359574/67541c83-85e0-4c42-9bc1-40c929277a74) 



### Sistema de Delivery - Diagrama de Classes ### 

Este é um diagrama de classes que descreve a estrutura de um sistema de delivery de bebidas. O sistema é projetado para permitir que clientes façam pedidos, fornecedores forneçam bebidas, vendedores gerenciem o sistema e lojas físicas participem das vendas.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Classes Principais ### 
- Cliente
A classe Ciente  representa tanto os clientes quanto os vendedores do sistema.
 Atributos:
* login: O login do usuário.
* senha: A senha do usuário.
* nome: O nome do usuário.
* CPF: O CPF do usuário.
* email: O email do usuário.
* endereço: O endereço do usuário.
* telefone: O telefone do usuário.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Produto ### 

A classe Produto representa os produtos disponíveis para compra.
Atributos:
* código do produto: Identificador único do produto.
* nome do produto: Nome do produto.
* valor do produto: Valor do produto.
* valor produto de compra : Valor de produto de compra de fornecedor
* valor produto de vendas : Valor de produto de venda 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Fornecedor ### 
- A classe Fornecedor representa os fornecedores de bebidas.
Atributos:
* código do fornecedor: Identificador único do fornecedor.
* nome do fornecedor: Nome do fornecedor.
* estoque: Quantidade disponível de cada produto para entrega.
* edereço: Endereço do fornecedor 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Vendedor ### 
A classe Vendedor representa os vendedores do sistema.
Atributos: 

*  código do vendedor: Identificador único do vendedor.
*  código da loja física: Identificador da loja física associada ao vendedor.
*  código do usuário: Identificador do usuário associado ao vendedor.
*  nome do vendedor: Nome do vendedor.
*  telefone do vendedor: Telefone do vendedor.
*  ADMIN: Indica se o vendedor tem permissão de administrador.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###  FIlAL  ###  
A classe filial  representa as lojas físicas participantes do sistema.
Atributos:
*  código da loja: Identificador único da loja física.
*  nome da loja: Nome da loja física.
*  endereço da loja: Endereço da loja física.
*  telefone da loja: Telefone da loja física.
*  código do vendedor: Identificador único do vendedor.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###  Relatório Mensal de Vendas ###
A classe RelatórioMensalVendas registra informações sobre as vendas mensais.
Atributos:
*   código do relatório: Identificador único do relatório.
*   código da loja física: Identificador da loja física associada ao relatório.
*   valor total de vendas: Valor total de vendas da loja no mês.
*   data início: Data de início do período do relatório.
*   data fim: Data de término do período do relatório.
*   fomra_pagamento :  mostra as forma de pagamento recebido
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
* ### InterfaceZeDelivery  ###
 A classe InterfaceZeDelivery representa a interface de comunicação com o serviço ZeDelivery.
Atributos:
*  COD_INTERFACE_ZE_DELIVERY: Código único da interface ZeDelivery.
*  E-MAIL: Endereço de e-mail do cliente.
*  SENHA : Senha de cadastro do cliente.
*  Casdra: usuario fazer cadastro sistemas.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### PedidoVenda ## 
A classe PedidoVenda representa os pedidos de venda feitos pelos clientes.
Atributos:
*  COD_PEDIDO: Código único do pedido de venda.
*  COD_CLIENTE: Código único do cliente que fez o pedido.
*  COD_TIPO_PRODUTO: Código do tipo de produto associado ao pedido.
*  NOME_PRODUTO: Nome do produto incluído no pedido.
*  DTA_PEDIDO: Data do pedido de venda.
*  STATUS_PAGAMENTO: Status do pagamento do pedido (por exemplo, "Pago" ou "Pendente").
*  FORMA_PAGAMENTO: Forma de pagamento escolhida pelo cliente (por exemplo, "Cartão de Crédito" ou "Boleto").
*  Status_pedido_venda: Status do pedido de venda (por exemplo, "Em processamento" ou "Entregue").
*  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
* ###  ItemPedidoVenda ### 
A classe ItemPedidoVenda representa os itens individuais dentro de um pedido de venda.
Atributos:
*  COD_ITEM_PEDIDO_VENDA:  Código único do item do pedido de venda.
*  COD_PEDIDO_VENDA: Código do pedido de venda ao qual o item está associado.
*  COD_PRODUTO: Código do produto associado ao item.
*  QTD_ITEM_PEDIDO_VENDA: Quantidade de produtos incluídos no item do pedido de venda.
*  Val_total: Valor total do item do pedido
*  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  ### cotacao ### 
A classe Cotacao representa as cotações de produtos feitas por fornecedores.
Atributos:
*  COD_COTACAO: Código único da cotação.
*  COD_PRODUTO: Código do produto para o qual a cotação foi feita.
*  COD_FORNECEDOR: Código do fornecedor que fez a cotação.
*  VLR_COTACAO: Valor da cotação.
*  UNIDADE_MEDIDA: Unidade de medida relacionada à cotação (por exemplo, "quilograma" ou "litro").
   -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### ItemPedidoCompra ### 
A classe ItemPedidoCompra representa os itens individuais dentro de um pedido de compra.
Atributos:
*  COD_ITEM_PEDIDO_COMPRA: Código único do item do pedido de compra.
*  COD_PEDIDO_COMPRA: Código do pedido de compra ao qual o item está associado.
*  COD_PRODUTO: Código do produto associado ao item.
*  QTD_ITEM_PEDIDO_COMPRA: Quantidade de produtos incluídos no item do pedido de
  -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  ### ItemPedidoCompra ###
A classe ItemPedidoCompra representa os itens individuais dentro de um pedido de compra.
Atributos:
*  COD_ITEM_PEDIDO_COMPRA: Código único do item do pedido de compra.
*  COD_PEDIDO_COMPRA: Código do pedido de compra ao qual o item está associado.
*  COD_PRODUTO: Código do produto associado ao item.
*  QTD_ITEM_PEDIDO_COMPRA: Quantidade de produtos incluídos no item do pedido de compra.
 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

