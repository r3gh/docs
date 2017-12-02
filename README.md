# DevOps
- Criação de canal no Slack para compartilhamento de ideias
- Integração GitHub-Slack para acompanhamento de progresso paralelo
- Automação do Deployment
- Criação de ferramental para automatização de deployment, com o objetivo de agilizar a instanciação e deployment dos módulos
  - Um único script que cria os seguintes recursos na nuvem:
     - Key Pair
     - Security Group
     - Network
     - Subnet
     - Router
     - Router Interface
     - Instance 
   

# Componentes:
-	BD
-	Crawlers:
    -	Tweets estático de usuários que postam sobre violência
    -	Crawler de dados de APPs
-	Streamers:
    - Para pegar os tweets em tempo real
    - Para pegar dados dos apps
-	Integrador dos dados
    - NLP para estruturar os dados do Twitter
    -	Geolocalizacão reversa para anotar todos os incidentes com (Lat, Long)
    -	Limpeza dos dados
    -	Remoção de redundâncias
-	Módulo ML
    - KDE
    - Regressão
- Dashboard

# Desafios Atacados
-	HeatMap 
- Twitter Bot ao mesmo tempo 
- Vários outros bonus

# Público Alvo
-	Apoio à tomada de decisão para o COR (dashboard)
-	Dados disponíveis abertamente para a sociedade civil. Novos apps e visualizações podem ser criados 

# Motivação
-	Muitos crimes não são documentados
-	Não podem ser utilizados em tempo real para prevenção e melhor utilização de recursos de segurança pública
-	Apesar de haver diversos Apps que têm os dados, os dados não são estruturados, são desintegrados, indisponíveis para consulta (estruturada) pública via API

# Proposta de Valor:
###	Banco de Dados:	
-	Integrar dados de incidente de segurança pública da cidade do Rio a partir de **diferentes fontes** em tempo real:
    -	Twitter de usuários que postam frequentemente sobre incidente de segurança
    - App do OTT
    - App do Onde Fui Roubado
     - Dados do DataRio
- O banco de dados é facilmente extensível
-	Dados estruturados e curados disponíveis publicamente via API

###	Inteligência Artificial usando o banco de dados
-	Auxiliar a tomada de decisão para otimizar de alocação de recursos de segurança pública
-	Como? 
    -	Análise visual da mancha criminal plotando um heat map com KDE
    -	Quanto mais quente indica que aquele lugar é mais propenso de ocorrer novas incidências
- Predição de incidentes usando Regressão
    -	Input: Bairro, Tipo de crime
    - Output: Dia da semana e faixa de horário em que o tipo de crime deve acontecer


