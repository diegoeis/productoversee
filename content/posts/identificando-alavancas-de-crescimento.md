---
type: post
title: Identificando alavancas de crescimento
excerpt: Entenda como desdobrar o GMV
authors: Diego Eis
date: 2021-03-22
publishDate: 2021-03-22
image: https://i.imgur.com/0Lv0pQf.png
categories:
  - Estratégia
  - Dados & Indicadores
tags:
  - negócio
  - mercado
  - métricas
sponsor: Nenhum
---
Indicadores de produtos são um assunto recorrente. Isso acontece porque todo mundo acha que indicadores são difíceis de dominar ou de entender, mas na verdade, tudo o que ouvimos sobre indicadores são tentativas de abstrações pra deixar isso mais perto da sua realidade. O que eu quero dizer é que cada empresa e cada produto tem seus próprios indicadores e métricas e que mesmo que eles tenham nomes iguais, por exemplo Churn, são calculados de formas diferentes. Por isso, é importante que você entenda do negócio, ou seja, como sua empresa perde e ganha dinheiro, em qual o momento estratégico e tático ela se encontra e principalmente quais os mecanismos que regem o mercado no qual o seu negócio se encontra.

Além disso, é bastante incomum encontrar times de produtos que conseguem conectar diretamente os indicadores de produto com os indicadores de negócio. Geralmente encontramos times tentando movimentar ponteiros especificamente de produto e que na  maioria das vezes são bem difíceis de conectar com as principais alavancas financeiras ou de crescimento da empresa.

Todas as empresas têm mecanismos claros que impulsionam seu crescimento e mantém saudável o fluxo de dinheiro. Essas alavancas quase sempre podem ser conectadas de forma direta ou indireta com os indicadores e os planejamentos táticos de Produto.

Nesse texto mostro como podemos encontrar alavancas de crescimento desdobrando um dos principais indicadores de mercado, o GMV. 

## GMV - Gross Merchandise Value

O GMV é basicamente a medida do valor total das vendas da sua empresa dentro de um período de tempo. Basicamente é como sua empresa faz dinheiro. 

*Dessa forma, o GMV é um indicador usado para calcular o volume bruto das mercadorias de uma loja virtual, inseridas no segmento e-commerce. — Vindi, [O que é GMV? Tudo sobre o Gross Merchandise Volume](https://blog.vindi.com.br/o-que-e-gmv/)*

Você pode achar um pouco estranho falar de GMV em serviços e produtos digitais, já que esse indicador é bastante usado em negócios que vendem produtos físicos, contudo, esse conceito pode ser usado em empresas comuns, sobretudo aquelas que têm seus modelos de negócio baseados em marketplace, onde existem dois lados: oferta e demanda.

A fórmula do GMV é a seguinte:  *GMV* = **Preço de venda x Unidades Vendidas**

Exemplos: 

* No **Mercado Livre**, a unidade vendida é o produto vendido (e não o pedido. O pedido é o conjunto de vários produtos comprados);
* No **AirBnb**, a unidade vendida é a diária (e não a estadia. A estadia é um conjunto de diárias);
* No **iFood** é a refeição (e não o pedido. O pedido é um conjunto de refeições);

## Quebrando o GMV em 3 partes: Core, Oferta e Demanda

Existem 3 dimensões que surgem com a criação de uma árvore de GMV:

1. **Core:** é onde quebramos a estrutura inicial básica da fórmula do GMV, com os dois primeiros elementos de Preço de venda e Unidades vendidas;
2. **Oferta:** onde dividimos as partes responsáveis pela criação de oferta para os clientes consumidores. São os elementos que estimulam e mantém a abundância de oferta ativa;
3. **Demanda:** onde dividimos as partes que representam a demanda interessada pela oferta distribuída. São as empresas e/ou pessoas que compram e usam seu serviço/produto. Basicamente para quem a proposta de valor é destinada;

Essa é a imagem completa dessa árvore de GMV:

![](https://lh4.googleusercontent.com/uK1ukOl9s9_U1r_dVImdRtzyM0hCoeM4ZrKogT9VnmemFH9uhIXefoI9wd-2VaY4Ae3fNG5ehAqPPH9RMGA5LutIAf93ckySq-JWWMylSVUwMrBQdOB6z8H2z--v_q_EIUiL8FvK)

Vamos tentar passar por cada uma dessas fases e entender melhor como o core é desdobrado em vários elementos controláveis pela empresa e pelo produto.

Nesse texto, para facilitar, vou usar o exemplo simplificado de um serviço de transporte por aplicativo.

## O início

Relembrando: o GMV é formado por uma multiplicação simples entre **Preço de Venda** pela **unidades vendidas**.  

*GMV* = **Preço de venda x Unidades Vendidas**

Lembrando que estamos usando o exemplo de um serviço de transporte via aplicativo. O GMV desse serviço é formado pela multiplicação do **valor da viagem**, pela quantidade de **viagens finalizadas**. A viagem (algo intangível) entra no lugar da mercadoria (se fossemos comparar com um mercado, por exemplo). 

Como padrão nesse tipo de serviço, o preço da venda cobrado dos passageiros é variável, então, usaremos o **ticket médio** como sendo o **preço de venda** de cada viagem finalizada. Se quiser ler mais sobre isso, basta procurar sobre AOV (Average Order Value).

Sendo assim, vamos desdobrar esses dois eixos nas dimensões de oferta e demanda.  Vamos quebrar o texto em duas grandes partes: 

1. A primeira parte explica o cálculo do **preço vendido**, que é o valor que as viagens seriam vendidas. Se fosse um produto físico, seria o valor deste produto;
2. A segunda parte explica o cálculo do volume de **unidades vendidas**, nesse nosso caso, a viagem. Em um caso normal, seria a quantidade total de produtos vendidos;


## Preço vendido = valor da viagem / viagem finalizada

O preço vendido, nesse caso, é o ticket médio do valor pago nas viagens. 

Preço / viagem finalizada = **(Viagem / Passageiro) x (Valor da viagem / Passageiro)**

![](https://lh6.googleusercontent.com/w4qfxj4yLqKohTDneeaqKLuZ9P3MN7IwRcEsaLYEKjW905wAOsfbIfYf_4xIikkQqEIUJy9k5rynBCJ_RmQ2dV0lfXukcEmj8in9Qg11aUKg0O3_9G9s-hrnsglEA5G90Er9GpoE)

Esse calculo é feito dividindo dois outros valores:

* **Viagem / Passageiro:** é quantidade de viagens que cada passageiro fez. Pegamos o total das viagens feitas e dividimos pela quantidade de passageiros. Nesse caso, pegamos todos os passageiros ativos. O que é um passageiro (ou um usuário) ativo, vai depender da empresa e do time. Vale um estudo de período versus compra do serviço;
* **Valor da Viagem / Passageiro:** é o valor que cada passageiro paga nas viagens que realiza. Pegamos o montante gerado e dividimos pela quantidade pagante de passageiros ativos.

## Viagens por Passageiro

Vamos desdobrar então, como calculamos a variável de oferta **viagens / passageiro**.

Ela é formada pela multiplicação entre **Total de Viagens** e **Total de Passageiros**.

![](https://lh5.googleusercontent.com/OV3j5q-1ebAFRS74jl7poY04VSGZRKi9xcBSQQKAjfnYfKRdVLRY4D__TCeJiho1tKl1d6rEVDZwa4DXYVVomHSZjqNCl25YI79z60XpzgnCusMT5IWnMPkQAJpsTjfc8EdJfOwv)

* **Total de Viagens:** é a subtração do total de chamados com os chamados cancelados. Esses chamados cancelados são quaisquer chamados que o motorista recebeu, mas foi cancelado por ele ou por outro motivo. Podemos quebrar isso depois para virar outros indicadores importantes, por exemplo: diminuição de pedidos cancelados pelos motoristas;
* **Total de passageiros:** é a soma de novos passageiros que fizeram pelo menos uma viagem paga, passageiros ativos que já estão na base e fizeram pelo menos uma viagem paga, menos os passageiros inativos. Nesse caso, a empresa decide o que é um passageiro inativo (não utilização do serviço dentro de um período de tempo, por exemplo);

## Valor da Viagem / Passageiro

A outra variável que monta o Ticket Médio por Viagem é o **Valor da Viagem / Passageiro**. Ela é calculada pela multiplicação entre o **total de passageiros** e o **valor da viagem**.

![](https://lh5.googleusercontent.com/VIhG_GTRVCnS8Sjf0kTuTOnqibVImvq_bHCJKMW-XRd0LmjfCQlPnj0l7nWkmwOzvugAMLvDDAqz_WPtFbMlQPoFvbb2F2zb7K6hcatd42GViGZ_OphUtpcbQ6iIGDsBAFOUhgt_)

* **Valor da Viagem:** O valor da viagem é a cobrança feita pelo aplicativo para o passageiro. Essa cobrança é feita levando em consideração uma série de fatores e restrições, chuto que o Uber tenha algo como valor mínimo base da “bandeirada”, mais o algoritmo de precificação (tá chovendo, bateria está acabando, muito trânsito, distância etc) e alguma taxa ou seja lá o que mais for cobrar;
* **Total de passageiros:** é a soma de novos passageiros que fizeram pelo menos uma viagem paga, passageiros ativos que já estão na base e fizeram pelo menos uma viagem paga, menos os passageiros inativos. Nesse caso, a empresa decide o que é um passageiro inativo (não utilização do serviço dentro de um período de tempo, por exemplo);

![](https://lh6.googleusercontent.com/6qD2SiZ1304MECLd7PYhuCfjDn-JhBUGXiGkfefAKITg5GF2VxL2TBDqZojXohF4wwvVe0ZDIU5ghsHQTu8lcsIxRUyUuhUigAapI35UGBUISveLMz7X8zlOFuhNMGELVepYBCcp)

Esse seria o desdobramento completo da geração do ticket médio por viagem do serviço. Vamos desdobrar agora a segunda parte da conta, que é a quantidade total de viagens finalizadas, representando a unidade vendida. 

## Unidade vendida = # viagens finalizadas

Essa é uma parte relativamente simples. Nós precisamos calcular a quantidade total de viagens pagas feitas pelos motoristas. A estrutura do total de **viagens finalizadas** é a multiplicação das variáveis de motoristas e **viagens / motoristas**.

![](https://lh4.googleusercontent.com/579Vx2VvH2Dx7TqJntP267ozZzrGQitiA1UqwoAvaquP9exmiAV__aveNoP6obdExK2_mAaac1GS_uqfDWrAvcUODoX6cdj0NdaR7qGF960vxcEosyDjwTQ1SJtw9u18cabbkWED)

Viagens finalizadas é a multiplicação das variáveis **Total de motoristas** e **Viagem por Motorista**. A fórmula seria mais ou menos essa:

Viagens finalizadas = **Total motoristas x (viagens / motoristas)**

**Total Motoristas:** para fazer viagens, precisamos de motoristas. Logo, a quantidade de viagens depende da quantidade total de motoristas que finalizaram viagens. A variável de Total de Motoristas é composta pela soma da quantidade dos motoristas novos com os motoristas já ativos na base, subtraindo os motoristas inativos. Novamente, o que é um motorista ativo, novo e inativo, vai depender da interpretação da empresa e seus times. 

**Viagens / motoristas:** a segunda parte é entender quantas viagens cada motorista finalizou. Esse elemento é calculado tendo como base o total de viagens que os motoristas já fizeram. Isso é feito pegando o total de pedidos e subtraindo o total de pedidos cancelados. Dentro desses pedidos cancelados podemos quebrar mais, adicionando pedidos cancelados pelo usuário por algum motivo.

## As alavancas de crescimento e o impacto nos times

Com esse desdobramento finalizado, você entende quais são as variáveis que diretamente ou indiretamente controlam seu GMV. A partir daqui, os times de toda a empresa conseguem desdobrar para si, cada uma dessas alavancas, entendendo como eles podem, de acordo com as suas especialidades, influenciá-las.

Já é claro que:

* Na parte de **Oferta**, os times do **comercial, customer success e produto** têm grandes responsabilidades para manipular os fatores que fazem a oferta aumentar, mantendo a abundância da disponibilização dos serviços
* Na parte de **Demanda**, os times de **marketing, branding e produtos** (cadastro, onboarding, retenção, conversão, etc) conseguem entender como funcionam os movimentos e momentos do seu público, criando um processo melhor de atração, aquisição, onboarding, uso, engajamento e recomendação.

Já a partir da árvore que montamos, conseguimos ter os seguintes indicadores para influenciar no produto:

* **Oferta** 
  * **Viagem / Passageiro:** Como fazer com que os passageiros façam mais viagens?
  * **Preço / Passageiro:** Como aumentar o ticket médio pago por cada passageiro?
  * **Viagem / Motorista:** Como fazer com que os motoristas façam mais viagens?
  * **Total de Motoristas:** Como aumentar a quantidade de motoristas disponíveis no serviço?
* **Demanda**
  * **Passageiros:** Como aumentar a quantidade de passageiros? 
  * **Valor da viagem:** Como conseguimos criar preços atrativos?
  * **Total de pedidos:** Como aumentamos a quantidade de pedidos que os motoristas recebem?
  * **Total de pedidos cancelados:** Como diminuímos a quantidade de pedidos que são cancelados ou que impedem de ter sucesso?

Esses pontos também conseguem ser desdobrados em OKRs. A partir daí, os times conseguem criar oportunidades e estudar hipóteses que podem movimentar esses indicadores diretamente ou entender quais indicadores do produto são proxy para a movimentação desses ponteiros. 

## Colocando isso em OKR ou qualquer outro modelo

Facilmente desdobrar esses indicadores em OKR ou qualquer outro modelo. Veja que interessante que fica:

* **Objetivo:** Aumentar a média de “viagens feitas por passageiro”
   * **KR 1:** Aumentar de X para Y o total de viagens
     * **Task:** Diminuir o total de cancelamentos de viagens pelo passageiro oferecendo incentivos para manter a viagem;
     * **Task:** Diminuir o total de cancelamentos de viagens pelo motorista
   * **KR 2:** Reativar X% dos passageiros inativos
     * **Task:** oferecer cupom de desconto progressivo para passageiros que não fizeram viagens nos últimos X meses;

Veja que é possível modificar uma série de alavancas a partir de produtos ou iniciativas de outras áreas. É uma maneira de o time de produtos influenciar diretamente os indicadores que causam impacto imediato no negócio, aliando iniciativas que entreguem valor para o usuário.

## Conclusão

Não é aconselhável olhar o GMV de forma solitária. Esse indicador sozinho não dá muitas respostas e desconsidera uma série de outros fatores como LTV, CAC, Churn e Conversão, só para citar alguns. Por isso, fazer esse desdobramento pode abrir um pouco mais o leque de oportunidades. 

Eu sei que a primeira vista esse estudo pode ser parecer medonho, contudo, sugiro que você faça esse exercício no produto em que está agora. Durante esse processo, você com certeza vai adquirir mais conhecimento sobre o negócio da empresa e como ela consegue se manter de pé. Esse exercício fica mais interessante se você tiver parceiros de outras áreas ajudando, como comercial, negócios e dados.

Aproveito para agradecer ao Pedro Beloti por revisar a árvore e se certificar que eu não estava falando tanta besteira assim. ;-)

## Referências:



* [How to avoid mistakes while calculating the GMV of an international marketplace? | by Yurgen Bashkatov | Lalafo | Medium](https://medium.com/lalafo-engineering/how-to-avoid-mistakes-while-calculating-the-gmv-of-an-international-marketplace-e9171e11bd1a)
* [What’s Uber Really Worth? | Trefis](https://dashboards.trefis.com/no-login-required/qvzJvTzt?fromforbesandarticle=breaking-down-ubers-valuation-interactive-analysis)
* [Breaking Down Uber’s Valuation: An Interactive Analysis](https://www.forbes.com/sites/greatspeculations/2018/02/22/breaking-down-ubers-valuation-an-interactive-analysis/?sh=72f9ee8a4785)
* [What Is GMV and How It’s Important for Marketplaces | by Victor Maia | Medium](https://medium.com/@victormaiam/what-is-gmv-and-how-its-important-for-marketplaces-fa1bdf8808ce)