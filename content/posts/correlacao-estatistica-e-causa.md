---
title: Correlação estatística e causalidade em métricas de produto
excerpt: Como entender esses dois conceitos pode facilitar demais a vida de uma PM
authors: Pablo Silva
date: 2020-08-26
tags: [Negócios]
categories: [Indicadores e Dados]
image: https://images.unsplash.com/photo-1584472666879-7d92db132958?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2746&q=80
featured_post: false
---

A correlação estatística e o conceito de causalidade podem ser
diretamente aplicados no dia a dia de trabalho de uma PM. Identificar a
correlação que o nosso conjunto de métricas de produto tem com os
resultados que precisamos atingir, pode abrir caminho para que a gente
consiga encontrar hipóteses com um potencial maior de validação na hora
de incrementar o produto. Vamos então entender esses dois conceitos e
como aplicá-los no nosso dia a dia.

### A correlação estatística

A correlação entre duas variáveis mostra a associação que existe entre
elas, ou em outras palavras, o quanto uma variável está relacionada com
a outra. Nesse sentido, estamos falando de uma associação linear, ou
seja, conforme uma delas cresce ou diminui a outra cresce ou diminui
também em uma unidade fixa de valor.

Exemplo: taxa de juros desceu 2.5% e a inflação desceu 0.5%, taxa de
juros desceu 2.0% e a inflação cresceu 3%. Como podemos ver, as
variáveis não precisam crescer ou descer nas mesmas unidades, o que vai
nos dizer o grau da correlações são as proporções de crescimento ou
decréscimo de uma em relação a outra.

### Toda correlação tem um grau

O grau dessa associação pode ser calculado através do coeficiente de
correlação, conhecido na estatística como **r** ([correlação de
Pearson](https://www.statisticshowto.com/probability-and-statistics/correlation-coefficient-formula/))**.**
Existem três possíveis casos quando calculamos r:

-   0 \> r ≥ 1 nesse caso temos uma correlação positiva e isso acontece
    quando as duas variáveis estão crescendo ou decrescendo. É positiva
    porque as variáveis estão indo na mesma direção.

-   0 nesse caso não existe nenhuma correlação entre as variáveis

-   -1 ≥ r \> 0 nesse caso temos uma correlação negativa e isso acontece
    quando uma variável está crescendo e a outra decrescendo ou
    vice-versa. É negativa porque uma variável está influenciando a
    outra na direção oposta.

Quanto mais próximo de 1 o coeficiente for, não importando se negativo
ou positivo, mais forte é a evidência de que há uma relação entre as
duas variáveis.

### O cálculo r

Eu não vou entrar em detalhes aqui na fórmula para calcular esse
coeficiente, mas vamos imaginar que você é PM do Lava Carros, um app em
que as pessoas podem agendar lavagens de carros em suas próprias casas.
Você recebeu a missão de aumentar o número de carros lavados em 30%.
Vamos tomar como exemplo o \# de carros vendidos e o \# de carros
lavados entre janeiro e agosto de 2020

[![](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/16905ceb-9333-45e6-a659-a9e3005e7fe2_335x192.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F16905ceb-9333-45e6-a659-a9e3005e7fe2_335x192.png)

Para calcular o coeficiente de correlação entre essas duas variáveis,
podemos utilizar a função CORREL no Google Sheets ou Excel (o exemplo
completo está
[aqui](https://docs.google.com/spreadsheets/d/1X-Ccps1I7zl759pDqs1x50y4v2gyueKYjBEhmtmPtI0/edit?usp=sharing))

[![](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/97cf129c-435d-4d23-b144-28856863c258_336x233.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F97cf129c-435d-4d23-b144-28856863c258_336x233.png)

Para esse conjunto de dados, podemos ver que r = 0.94, o que significa
que há uma correlação positiva e quase perfeita, porque está muito
próximo de +1. É visível que conforme o \# de carros vendido cresceu o
\# de carros lavados também cresceu.

É claro que nesse exemplo, estamos com um conjunto de dados bem simples
e conseguimos ver visualmente, mas pense em um conjunto de dados
complexo dos seus usuários, com milhões de data points!

### Correlações estatísticas são pistas valiosas

Uma maneira relativamente comum de se trabalhar com gestão de produto é
definindo um *outcome*, métrica foco ou *output metric* (é tudo a mesma
coisa) que é um indicador de resultado que geralmente está ligado com
objetivos de produto de negócio. Uma *output* é sempre influenciada por
um conjunto de *input metrics* ou métricas proxy (também a mesma coisa),
que são métricas que vem de tarefas dos usuários dentro da nossa
plataforma de forma direta ou indireta.

Quem usa esses conceitos no dia a dia para gerir o produto sabe que o
objetivo é atingir algum acréscimo ou decréscimo em uma *output metric*,
porque se a sua estratégia de produto está bem definida, ela vai causar
o impacto que o negócio espera nos objetivos da empresa (assunto para
outra letter).

Para exemplificar, aqui nesse texto vou utilizar os termos *output* e
*input metrics* que retirei do livro do Eis ([Gestão moderna de serviços
digitais](https://amzn.to/34GEV6y))

[![](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/d1e6f815-be98-4503-9382-4e1e2d4fc651_800x611.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fd1e6f815-be98-4503-9382-4e1e2d4fc651_800x611.png)

###### Output e Input Metrics --- Gestão Moderna de Serviços Digitais --- Diego Eis

Trazendo para o nosso exemplo no Lava Carros, nossa *Output Metric* é \#
de carros lavados e uma *input metric* é o \# de novos carros
cadastrados. No modelo acima, ficaria assim inicialmente

[![](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/60502015-59c5-420f-aa92-f27b04b4f40a_1066x670.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F60502015-59c5-420f-aa92-f27b04b4f40a_1066x670.png)

Nesse caso, vimos que existe uma correlação positiva quase perfeita
entre o número de novos carros cadastrados e número de carros lavados.
Podemos então afirmar que quanto mais novos carros forem cadastrados,
mais irá aumentar o nosso número de carros lavados ou em outras
palavras, o aumento de carros cadastrados **causa** o aumento de carros
lavados?

### Correlações podem ser perigosas

Nosso cérebro é campeão em nos enganar com padrões que parecem
totalmente verdadeiros. Parece óbvio de que com mais carros cadastrados,
mais teremos um aumento de carros lavados e é aí que está o problema,
não costumamos validar o óbvio.

Você então, que é uma PM já vacinada contra esse tipo de padrão, resolve
ir além e faz uma análise mais profunda nos novos carros cadastrados e
descobre que 80% dos novos carros ainda não passaram por nenhuma
lavagem. Logo, isso diz que, apesar da alta correlação que existe entre
essas duas variáveis, o aumento de carros cadastrados não é causador
direto do aumento substancial da lavagem. Nesse caso, o índice de
causalidade é bem baixo, pois só 20% dos novos carros agendaram uma
lavagem.

Esse é um dos principais cuidados que temos que ter quando encontramos
altas correlações em nossas variáveis: **uma correlação, mesmo que
alta**, **não é indicativo direto de causalidade, ela é só uma pista.**

### Trabalhando com múltiplas variáveis

Visto que o óbvio nem sempre é o que vai nos trazer o resultado que
estamos buscando, o melhor que podemos fazer, é trabalhar com um
conjunto maior de *input metrics*, numa dimensão que nos permita ganhar
mais alcance de variáveis que podem ter um índice de causalidade maior
na nossa *output metric**.***

Evoluindo nosso modelo do Lava Carros**,** poderíamos ter mais variáveis

[![](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/f7ba4fd1-0bb1-4757-ad29-79cf0a5c42b0_800x641.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Ff7ba4fd1-0bb1-4757-ad29-79cf0a5c42b0_800x641.png)

Nesse caso, adicionamos o número de cupons de desconto distribuídos e o
tempo que um cliente espera para conseguir uma lavagem. Vamos supor que
as correlações de ambas variáveis sejam altas e positivas, que é o que
precisamos nesse caso, porque queremos aumentar o número de lavagem de
carros. Qual a possibilidade de ambas causarem um aumento no número de
carros lavados?

### A causalidade emerge da experimentação

Para descobrir se \# de cupons de desconto causa o aumento no \# de
carros lavados, o que precisamos fazer é um experimento. Podemos
escolher um grupo de clientes que nunca fizeram nenhuma lavagem e
mandamos um cupom de desconto para eles e observamos o resultado que
isso tem no agendamento de novas lavagens. 

Para tonar o índice de causalidade mais confiável, podemos inclusive
fazer mais de um experimento, dividindo os grupos que mandamos os cupons
por fatores demográficos por exemplo. Trabalhar com múltiplos
experimentos, irá nos ajudar a entender os fatores que de fato causam o
aumento da lavagem de carros.

No final, é o experimento que vai nos dizer se existe uma causalidade e
não a correlação. É claro que existem *input metrics* que são mais
fáceis de entender a causalidade do que outras, mas no geral, conseguir
trabalhar com múltiplos experimentos é o que vai nos trazer velocidade
para validar ou invalidar nossas hipóteses.

### Uma última pitada de causalidade

Um ponto muito importante é que uma *output metric* pode ter influência
externas também e no geral isso sempre é verdadeiro. É muito importante
que a gente também consiga enxergar essas variáveis, mesmo que a gente
não as consiga controlar.

No nosso exemplo, o número de dias que choveu forte pode ser uma
variável que tem um alto índice causador do aumento do número de
lavagens, uma vez que o carro ficou cheio de folhas e a água suja da
cidade ficou por todo o carro.

Não conseguimos controlar os dias que chovem forte, mas podemos usar
essa informação de causalidade externa para mandar cupons de desconto
para a base quando esses dias acontecerem, porque já sabemos que os
clientes tem mais tendência a agendar lavagens nessa situação.

Conseguir aplicar esses conceitos no dia a dia vai facilitar muito a
vida da PM na hora de tomar decisões e também de conseguir explicar as
decisões que foram tomadas. Afinal, contra correlações e causalidades,
não há argumentos!

### Referências

-   [Naked Statistics: Stripping the Dread from the Data - Charles
    Wheelan](https://amzn.to/3jh4IGJ)

-   [Como mentir com Estatística](https://amzn.to/34GOO4a)

-   [Gestão Moderna de Serviços Digitais - Diego
    Eis](https://amzn.to/2G0nBPR)

-   [Correlação de
    Pearson](https://www.statisticshowto.com/probability-and-statistics/correlation-coefficient-formula/)

-   [Guia Estatística Análise de
    Correlação](https://www.ecommercebrasil.com.br/artigos/guia-estatistica-analise-correlacao/)