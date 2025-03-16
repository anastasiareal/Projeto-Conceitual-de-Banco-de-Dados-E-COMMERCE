# Projeto-Conceitual-de-Banco-de-Dados-E-COMMERCE
Desenvolvido um modelo conceitual de banco de dados para um sistema de e-commerce, refinado para incluir novos recursos. Aqui estão os principais ajustes e aprimoramentos realizados:
1. Separação de Cliente PJ e PF

Agora a tabela Cliente possui duas entidades derivadas:

    Pessoa Física (CPF e nome)
    Pessoa Jurídica (CNPJ e razão social)
    Cada cliente pode ser apenas um dos dois tipos (1:1 com Cliente).

2. Adição de Métodos de Pagamento

Criada a tabela Pagamento, que está associada a Pedido.

    Permite armazenar múltiplos métodos de pagamento para um mesmo pedido.
    Campos incluem tipo de pagamento (cartão, boleto, PIX) e detalhes adicionais.

3. Adição da Tabela de Entrega

Criada a tabela Entrega, vinculada a Pedido.

    Contém o status da entrega (ex.: "A caminho", "Entregue").
    Inclui um código de rastreio, fundamental para acompanhamento.

4. Relacionamentos e Melhorias Gerais

    Pedidos agora se relacionam com Entrega e Pagamento, permitindo um fluxo mais completo do processo de compra.
    Produtos continuam sendo gerenciados por vendedores terceiros e fornecedores, mantendo a estrutura de marketplace.
    O estoque está ligado a produtos, garantindo controle sobre a disponibilidade.
