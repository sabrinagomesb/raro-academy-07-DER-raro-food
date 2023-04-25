# Diagrama Entidade-Relacionamento RaroFood

Atividade do curso Ruby on Rails - Raro Academy com o objetivo de praticar os conceitos vistos na Semana 07, cujo o tema foi "Modelagem de Banco de Dados".

## Objetivo

Continuar o Modelo de Entidade-Relacionamento, que foi inciado nas duas primeiras aulas da semana, implementando as novas necessidades da aplicação descritas no [enunciado](./enunciado.md) da atividade.

## Resolução de problemas

- Valor do Frete: Foi incluída a relação **contém** para ligar a entidade "Pedido" para a entidade "Valor Frete". Com a notação de 0 ou 1, já que no Pedido pode conter ou não o valor do frete. O "Valor Frete" não foi representado como atributo, pois por ser opcional ele não vai estar sempre presente na entidade Pedido.
  <br>
- Cupom de Desconto: Foi incluído como uma entidade e todos seus atributos foram detalhados. O atributo "Validade" foi notado como _composto_ contendo "Data Início" e "Data Fim". Foi estabelecido o seguinte relacionamento binário:

  - 1 Administrador **cadastra** 0 ou N Cupom.

  Um segundo relacionamento estabelecido foi entre Cliente e Cupom Desconto, já que o Cliente pode utilizar 0 ou 1 Cupom. Essa entidade foi notada ainda como um atributo na entidade Pedido.
  <br>

- Cartão de Crédito: Foi incluído como uma entidade e todos os seus atributos foram notados. O atributo "tipo" foi notado como _composto_, tendo crédito e débito. Foram estabelecidos os seguintes relacionamentos:

  - 1 Cliente **cadastra** 0 ou N Cartão;
  - 1 Cartão **contém** 0 ou 1 Pagamento (como o cartão é apenas uma das opções de pagamento do Cliente, foi representado como uma relação opcional).
    <br>

- Pagamento: Foi definido como uma entidade com os atributos: forma de pagamento, código único, valor pago e status. O atributo Forma de Pagamento foi notado como composto por PIX, boleto, cartão de crédito e cartão de débito. Como visto no item anterior, o Pagamento se relaciona com a entidade Cartão, porém de forma opcional.
