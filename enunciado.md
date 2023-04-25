Prática 01 - Semana 07

Nesse exercício iremos abordar o conteúdo apresentado nas aulas 01 e 02 dessa semana.
Estruturem o Diagrama Entidade-Relacionamento considerando todos os conceitos que aprendemos.

Para facilitar utilizem a ferramenta online gratuita para desenho do diagrama Draw.io (https://app.diagrams.net/).

Problema:

A aplicação RaroFood está crescendo e precisamos evoluir a nossa modelagem.

Vamos supor que foi contratado um serviço externo responsável por calcular o valor de frete entre o endereço do chefe e o endereço selecionado pelo cliente. Consideraremos, portanto, que armazenaremos apenas o valor calculado (em reais) para cada pedido. Altere o diagrama acrescentando essa informação do valor do frete.
Vale ressaltar que, dependendo da distância entre os endereços, o valor do frete poderá ser gratuito.

Os administradores resolveram acrescentar uma nova funcionalidade para atrair cada vez mais clientes. Eles farão constantemente o cadastro de cupons de desconto. Para cada cupom deve ser armazenado: código único, código do cupom (exemplo: RAROFOOD10), nome, descrição, data de início e data de fim da validade, e, por fim, o total de desconto (em reais) que poderá ser aplicado. O valor do desconto cadastrado para cada cupom não poderá ser maior que o preço unitário dos pratos cadastrados. Cada cliente poderá ou não utilizar um dos cupons válidos para seus pedidos uma única vez. Exemplo: o cliente A utilizou o cupom válido C para o pedido 1, então o mesmo cupom C não poderá ser utilizado pelo cliente A no pedido 2. Ele também não poderá utilizar mais de um cupom em um mesmo pedido, ou seja, o cliente A não poderá utilizar os cupons válidos B e C para o pedido 1.

A RaroFood permitirá também que os clientes cadastrem cartões de crédito ou débito para que sejam utilizados no pagamento. Para cada cartão deve ser armazenado: código único, tipo do cartão, número do cartão, nome impresso, data de validade e código de segurança.

Para cada pedido o cliente realizará o pagamento escolhendo entre uma das formas sendo elas: PIX, Boleto, Cartão de Crédito ou Cartão de Débito. Uma vez escolhido Cartão de Crédito ou Cartão de Débito como forma de pagamento, o mesmo deverá ser associado ao pagamento.
Não nos preocuparemos como ocorrerá o processamento do pagamento, apenas com o armazenamento do código único, valor pago, forma de pagamento escolhida pelo cliente e status do pagamento.

Vocês poderão utilizar o arquivo der_raro_food.drawio que está na pasta materiais complementares como base para nossa prática, atualizando-o para adaptar às novas necessidades da aplicação.
Caso seja necessário, poderão reorganizar o diagrama para que possa ficar mais legível.

Link para acesso à pasta materiais complementares: https://git.raroacademy.com.br/turmas-ruby/ruby-turma1/ruby-alunos/aulas/-/tree/main/semana-07-modelagem-bd/materiais_complementares

Para entrega no classroom, vocês devem anexar 2 arquivos:

1. arquivo com extensão .drawio para o Diagrama ER;
2. arquivo com extensão .png para o Diagrama ER;
