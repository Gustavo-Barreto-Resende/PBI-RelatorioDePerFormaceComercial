📊 Relatorio de performance Comercial
__________________________________________________________________________________

📝 Visão Geral do Projeto
Este projeto foi desenvolvido para resolver um desafio real de uma empresa de varejo: a falta de clareza sobre o retorno real das promoções. O objetivo foi transformar dados brutos em uma ferramenta de decisão que identifica quais descontos geram receita incremental e quais estão apenas corroendo a margem de lucro.

__________________________________________________________________________________
🛠️ Tecnologias Utilizadas
Power BI (Power Query, DAX, RLS, Mobile Layout).

__________________________________________________________________________________

🏗️ Arquitetura e Modelagem
A solução utiliza o modelo SnowFlake para garantir performance e escalabilidade:

Tabelas Dimensão: dProdutos, dLojas, dCalendário dCategoriaProdutos, dIconeProdutos, dPromocoes, dSubCategoriaProdutos e dLocalidades. 
Fato: fVendas.

__________________________________________________________________________________

🧠Inteligência de Dados (DAX)
Foram implementadas métricas avançadas divididas em 4 pilares:

Core Business: Vendas Brutas, Líquidas, Quantidade e Custo Total.

Análise de Descontos: % de Desconto sobre faturamento para medir agressividade comercial.

Time Intelligence: Vendas LY (Ano Anterior) e % Crescimento YoY para análise de sazonalidade.

Eficiência: Margem e % Margem por categoria de produto.

Análise de Pareto: % de Participação por categoria para identificar os produtos "Curva A".

__________________________________________________________________________________

🔐 Segurança e Governança (RLS)

Para garantir a privacidade dos dados entre diferentes regiões, foi implementado o RLS (Row-Level Security) Dinâmico:

Filtro aplicado na tabela dLocalidades utilizando a função USERPRINCIPALNAME(), garantindo que cada gestor visualize apenas os dados do seu país de atuação.

__________________________________________________________________________________
🎨 Visualização e UX
O dashboard foi construído focando no Data Storytelling para o nível executivo:

Navegação: Uso de botões de navegação para alternar entre visões.

___________________________________________________________________________________

<img width="1427" height="793" alt="image" src="https://github.com/user-attachments/assets/ee0b1f42-849e-4c95-9eba-e9cb64c2b14c" />

_______________________________________________________________________________________


<img width="1424" height="786" alt="image" src="https://github.com/user-attachments/assets/56d35ab2-3db3-4513-a103-d108e0fcd932" />

_______________________________________________________________________________________

<img width="1424" height="799" alt="image" src="https://github.com/user-attachments/assets/5271192f-878f-4e51-aff5-5bf2d136e0ac" />

_______________________________________________________________________________________


<img width="1424" height="786" alt="image" src="https://github.com/user-attachments/assets/985cd685-1178-4685-8bcd-12cd31f94ff7" />


