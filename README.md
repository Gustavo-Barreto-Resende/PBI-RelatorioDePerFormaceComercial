📊 Relatorio de performance Comercial

📝 Visão Geral do Projeto
Este projeto foi desenvolvido para resolver um desafio real de uma empresa de varejo: a falta de clareza sobre o retorno real das promoções. O objetivo foi transformar dados brutos em uma ferramenta de decisão que identifica quais descontos geram receita incremental e quais estão apenas corroendo a margem de lucro.

🛠️ Tecnologias Utilizadas
Power BI (Power Query, DAX, RLS, Mobile Layout).

🏗️ Arquitetura e Modelagem
A solução utiliza o modelo SnowFlake para garantir performance e escalabilidade:

Tabelas Dimensão: dProdutos, dLojas, dCalendário dCategoriaProdutos, dIconeProdutos, dPromocoes, dSubCategoriaProdutos e dLocalidades. 
Fato: fVendas.

🧠Inteligência de Dados (DAX)
Foram implementadas métricas avançadas divididas em 4 pilares:

Core Business: Vendas Brutas, Líquidas, Quantidade e Custo Total.

Análise de Descontos: % de Desconto sobre faturamento para medir agressividade comercial.

Time Intelligence: Vendas LY (Ano Anterior) e % Crescimento YoY para análise de sazonalidade.

Eficiência: Margem e % Margem por categoria de produto.

Análise de Pareto: % de Participação por categoria para identificar os produtos "Curva A".

🔐 Segurança e Governança (RLS)

Para garantir a privacidade dos dados entre diferentes regiões, foi implementado o RLS (Row-Level Security) Dinâmico:

Filtro aplicado na tabela dLocalidades utilizando a função USERPRINCIPALNAME(), garantindo que cada gestor visualize apenas os dados do seu país de atuação.

🎨 Visualização e UX
O dashboard foi construído focando no Data Storytelling para o nível executivo:

Navegação: Uso de botões de navegação para alternar entre visões.

<img width="1424" height="786" alt="image" src="https://github.com/user-attachments/assets/56d35ab2-3db3-4513-a103-d108e0fcd932" />
