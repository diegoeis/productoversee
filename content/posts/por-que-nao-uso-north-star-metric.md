---
type: post
title: Por que não uso em North Star Metric
excerpt: Quando falamos de se apoiar em uma métrica que talvez indique tudo o
  que precisamos saber do sucesso do produto, estamos limitando nossa visão
  sobre impactos do produto.
authors: Diego Eis
date: 2020-12-21
publishDate: 2020-12-21
image: https://i.imgur.com/wdrj9E7.jpg
categories:
  - Indicadores e Dados
tags:
  - métricas
---
Quando estudamos sobre métodos e frameworks para definir métricas e indicadores de produtos, nós esbarramos em um conceito bastante difundido chamado North Star Metric. Na verdade, a North Star Metric está muito atrelado ao One Metric That Matters, que foi falado primeiramente no livro [Lean Analytics](https://amzn.to/32nwcDL). Logo essa ideia virou moda entre os produteiros do mundo todo. Aí o conceito de ter uma North Star Metric ganhou força. A North Star Metric é aquela métrica que toda empresa ou produto pode resumir seu sucesso. É aquele indicador que melhor descreve o “core value” que seu produto entrega para os usuários. 

## O que é a North Star Metric e por que não gosto dela?

Esse framework inclui e unifica uma série de fatores e métricas iniciais de produto e negócio, que expressam o valor e o sucesso, criando assim uma North Star Metric. Dessa forma o time pode influenciar esses fatores e essas métricas iniciais testando hipóteses, implementando novas funcionalidades e fazendo melhorias no produto, que por sua vez irão influenciar a North Star Metric, que por sua vez move os ponteiros de indicadores de negócio.

<iframe width="560" height="315" src="https://www.youtube.com/embed/bijLsIvhAys?start=79" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Quando falamos de ter apenas uma métrica ou indicador que talvez indique tudo o que precisamos saber do sucesso do produto, limitamos nossa visão sobre impactos que podem influenciar pontos diferentes do produto. Ter apenas uma métrica não pode ser saudável, dado que o momento da empresa, do mercado, do time, do negócio, dos usuários, mudam o tempo inteiro  e se alternam em prioridades.

## Primeiro a diferença entre Métricas e Indicadores
Uma explicação rápida para gente entender melhor o que vamos conversar agora. Todo mundo confunde métricas e indicadores. Pra definir rapidamente de uma maneira fácil: [métricas formam indicadores](https://diegoeis.com/parte1-metricas-indicadores-e-comportamento-do-usuario/). 

Um indicador como o Life Time Value (LFT) é formado pelo **Valor do Ticket Médio** e **Tempo de retenção do cliente**. O LFT indica quanto os usuários gastam no serviço durante o tempo que eles são clientes. Ou o **Stickness**, que mede a porcentagem de usuários mensais que retornam ao seu produto diariamente, é formado pelo DAU (Daily Active Users) e o MAU (Monthly Active Users).

Então, tenha em mente que Métricas são a menor parte de um indicador. Então, a North Star Metric, já não é exatamente uma métrica, mas um indicador.

## Comportamento do usuário, gera Input Metrics, que gera output metrics
Um produto ou um serviço pode ser medido por diversos indicadores que mostrarão se os usuários estão extraindo e percebendo todo o valor que serviço e/ou produto se pretende a entregar. Vamos chamar esses indicadores macro de Output Metrics ou de Focus Metrics. Você vai achar na internet explicações usando os dois nomes. Aqui vou usar o termo Output Metrics, ok?

As Output Metrics são indicadores (ops, foi mal, todo mundo usa o termo Metrics em inglês… pois é… era para ser lago como Output Indicators, mas né? Coisas desse mercado maluco…) que estão mais perto dos indicadores de negócio. São indicadores que você pode movimentar e acionar por meio de diversas métricas. Por exemplo, **engajamento** pode ser uma Output Metric. O engajamento é medido por diversas formas de comportamento e uso dos usuários dentro do seu produto, e vai depender de cada empresa definir o que é engajamento dentro do seu produto, por isso, não há uma maneira igual para todos os produtos modificarem o Indicador de Engajamento. 

> Focus metrics should be the top priority, not the sole priority, and improving the focus metric should not be accomplished at the expense of harming other KPIs. — Mixpanel Guide to Product Metrics, https://discover.mixpanel.com/rs/461-OYV-624/images/Guidetoproductmetrics-Mixpanel.pdf

As Output Metrics (ou Focus Metrics), são modificadas e acionadas por Input Metrics. As Input Metrics são métricas, geralmente geradas pelo comportamento de uso dos usuários dentro do seu produto. As Input Metrics podem alterar uma ou mais Output Metrics.

Uma Input Metric basicamente é gerada por “usuários ativos”. Um usuário ativo é aquele que vai além do login, do download do app, do cadastro. É o usuário que interage, que “engaja” no seu produto, ou seja, que usa e experiencia de forma uma ampla seu produto, executando core tasks do produto, procurando resolver suas necessidades, problemas e desejos. 

Cada produto/empresa tem uma definição do que é um usuário ativo. Geralmente um usuário, pra ser ativo, precisa executar várias tarefas dentro do sistema, não apenas uma. O Twitter, por exemplo, [considera que um usuário ativo](http://www.investopedia.com/terms/m/monthly-active-user-mau.asp) é aquele que segue pelo menos 3 contas, que tem pelo menos um follow-back e se logou no último mês. 

Essa **definição de usuário ativo** é bastante importante para que empresas mostrem para o mercado indicadores de saúde e crescimento. É também importante entender o que é um usuário ativo, para identificar formas de fortalecer os comportamentos e hábitos desses usuários, além de replicar mais usuários desse tipo.

## Como eu trato indicadores de produto
A única forma que consegui assimilar produto e negócio foi entender como essas duas pontas se conectam. Digo, qualquer linha de código  criada - que é o pedaço mais granular de um produto - no produto deve deixar a empresa mais perto da sua missão. Se isso não acontece, nós estamos perdendo tempo. Por isso, todos os esforços, tanto de análise quanto de execução dos times de produtos (e das empresas) devem ser direcionadas para como podemos deixar a empresa mais próxima do alcance da missão.

Essa proposição também deve ser aplicada à métricas e indicadores de produto. Por isso, os indicadores importantes no produto, devem se relacionar com os indicadores de negócio que nos mostram quando e se a empresa está cumprindo com sua missão. 

![](https://i.imgur.com/WUwr77e.jpg)

O uso de OKRs, KPIs, Opportunity Solution Tree ou qualquer outro método usado (inclusive North Star Metric) para controlar e monitorar indicadores e métricas, deve nos dizer se estamos conseguindo cumprir com a missão ou não. Esses indicadores são os faróis que nos dizem se o caminho está correto ou errado.

O encadeamento que eu faço, usando OKRs (mas essa analogia pode ser adaptada com qualquer outro método) é mais ou menos o que se mostra na imagem abaixo.

![](https://i.imgur.com/lWV80Pb.jpg)

![](https://i.imgur.com/ZmebwVq.jpg)

![](https://i.imgur.com/LXk0Dfp.jpg)

Exemplos totalmente hipotéticos, para servir apenas como exemplo.

Veja que é necessário existir uma ligação direta entre soluções / hipóteses com a missão e causa justa da empresa. Você pode [ler mais sobre causa justa aqui](https://simonsinek.com/discover/great-leaders-organizations-advance-a-just-cause/).

Tendo em vista esse encadeamento, as métricas de produtos devem estar ligadas exatamente com esses indicadores, servindo como sinais de alavancas de crescimento. Vamos pegar o exemplo do KEY RESULT “**Aumentar o número de programas de podcasts disponíveis de X para Y**”. Indicadores importantes aqui seriam:

- Taxa de crescimento de publicação de podcasts na plataforma que tem pelo menos um episódio ouvido [em um intervalo X ou ouvido por no mínimo Y minutos]. Mostra a velocidade de crescimento de novos episódios e shows dentro da plataforma, que poderá mostrar tendencia de ganho de market share de podcasts;
- Minutos ouvidos de podcasts. Mostra velocidade de crescimento de ouvintes e engajamento;
- Intervalo de publicação de novos episódios. Mostra que temos podcasters ativos. É necessário aqui entender e definir um tempo específico, talvez personalizado por clusters de similaridade de podcasts por frequência de publicação;

Abaixo segue um diagrama um pouco mais completo com o encadeamento entre tático e estratégico.

![](https://i.imgur.com/LLTeEyQ.jpg)

## Não consigo medir o sucesso vendo apenas um indicador

O sucesso de uma feature, de um produto, de um negócio não dá para ser resumido em apenas uma métrica (melhor seria a palavra indicador). cada indicador é movido de forma independente, mas assim pode ser influenciado por outros indicadores. 

Eu não estou invalidando o uso do NSM, pelo contrário, acho que é mais um método que pode ser usado se isso for conveniente para o seu produto e também para sua empresa. Eu não gostei quando experimentei porque senti muita dificuldade, pelos motivos já explicados acima, de tentar resumir tudo em um número ou em uma métrica/indicador que pudesse me dizer se o caminho está certo ou errado. Geralmente eu tinha que verificar outros indicadores e ainda fazer análises para entender melhor o comportamento e hábito dos usuários e do mercado que mudaram para  saber com mais clareza e menos incerteza o que estava acontecendo de estranho no sistema.

Em outro momento quero abordar um formato que me agrada muito mais, chamado de Constelação de Métricas, ou Input e Output Metrics, que pode ser usado como um método alternativo ao NSM.

## Referências:
- [Don’t Let Your North Star Metric Deceive You](https://www.reforge.com/blog/north-star-metric-growth)
- [What are the main differences between metrics and indicators?](https://www.opservices.com/differences-between-metrics-and-indicators/)
- [One Metric That Matters (OMTM) Clear explaination - Agile Parrot](https://agileparrot.com/metrics/one-metric-that-matters-omtm/)
- [What is a North Star Metric?](https://blog.growthhackers.com/what-is-a-north-star-metric-b31a8512923f)
- [North Star Metric ou Métrica da Estrela Guia](https://blog.vindi.com.br/north-star-metric-estrela-guia/)
- [Finding Your Product’s North Star Metric](https://www.youtube.com/watch?v=bijLsIvhAys)
- [Don't Become a Victim of One Key Metric](https://caseyaccidental.com/one-key-metric-victim)
- [Every Product Needs a North Star Metric: Here's How to Find Yours](https://amplitude.com/blog/2018/03/21/product-north-star-metric)
- [SaaS Product Metrics Pyramid](https://www.productplan.com/saas-product-metrics-pyramid/)

