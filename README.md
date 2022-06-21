Financeiro Pessoal

Intuíto de controle financeiro mensal com acompanhamentos e possiblidade de Adições, Edições e Exclusões de lançamentos realizados nos Débitos e Créditos.

Composição: 

    1 - Regra:
        > Utilizado PHP 8.1^
        > Laravel 9.1^
        > Lançamentos de Receitas e Despesas mensais, com controle de pagamentos dos lançamentos.
            * Adicionar, Editar, Remover Receitas
            * Adicionar, Editar, Remover Despesas
        > Relatório dos lançamentos separadamente ( Receitas e Despesas )
        > Relatório do mensal previsto ( [Total de Receitas] - [Total de Despesas] )
        > Relatório do mensal real ( [Total de Receitas Recebidas] - [Total de Despesas Pagas] )
        > Banco de Dados MySQL ou SQLite

    2 - Tabelas: 
        > Lancamentos_Receitas
            * ID => int
            * Receitas_Competencia => date 
            * Receitas_Tipo => string
            * Receitas_Detalhes => string
            * Receitas_Valor => double 
            * Receitas_Recebida => boolean
            * Receitas_DataRecebimento => date

        > Lancamentos_Despesas
            * ID => int
            * Despesas_Competencia => date
            * Despesas_Tipo => string
            * Despesas_Detalhes => string
            * Despesas_Valor => double 
            * Despesas_Pago => boolean
            * Despesas_DataPagamento => date