# 📊 Dashboard de Gestão de Vendas — Power BI

Dashboard interativo desenvolvido no **Power BI Desktop** para análise de vendas de uma rede varejista com múltiplas lojas, cobrindo faturamento, ticket médio, formas de pagamento, desempenho por produto e por unidade.

## 🎯 Objetivo

Consolidar dados de pedidos de vendas de diferentes lojas em um único painel visual, permitindo identificar rapidamente:
- Evolução do faturamento ao longo do tempo
- Desempenho comparativo entre lojas
- Produtos com maior participação na receita
- Distribuição das formas de pagamento utilizadas pelos clientes

## 🛠️ Tecnologias e ferramentas

- **Power BI Desktop** — modelagem e construção do dashboard
- **Power Query** — importação e tratamento dos dados de origem (planilhas Excel)
- **DAX** — agregações e cálculos (soma, média, percentual de participação)
- **Modelagem de dados** — relacionamento entre tabelas fato e dimensão

## 🗂️ Estrutura dos dados

O modelo é composto por duas tabelas principais, relacionadas por código da loja:

**`Registro de Vendas`** (tabela fato — pedidos)
| Coluna | Descrição |
|---|---|
| ID Pedido | Identificador único do pedido |
| Data Pedido | Data da venda |
| Código Loja | Código da unidade responsável pela venda |
| Produto | Categoria do produto vendido |
| Quantidade | Quantidade de itens no pedido |
| Preço Unitário | Valor unitário do item |
| Pagamento | Forma de pagamento (Cartão de Crédito / Transferência-PIX) |
| Valor Total Vendas | Valor total do pedido |

**`lojas`** (tabela dimensão — unidades)
| Coluna | Descrição |
|---|---|
| codigo_loja | Código único da loja |
| nome_loja | Nome da unidade (Matriz, Filial 1, Filial 2) |
| Cidade / UF | Localização da unidade |

## 📈 Visuais do dashboard

- **Cards**: Faturamento total e ticket médio
- **Gráfico de colunas**: Faturamento por mês
- **Gráfico de colunas agrupadas**: Faturamento por loja
- **Gráfico de pizza**: Distribuição por forma de pagamento
- **Tabelas**: Ranking de produtos por faturamento e participação percentual (%)

## ▶️ Como visualizar

1. Baixe o arquivo Relatorio de vendas.pbix e também o print.
2. Abra no **Power BI Desktop**
3. Explore os filtros e interações entre os visuais

