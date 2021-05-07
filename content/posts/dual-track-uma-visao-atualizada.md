---
title: "Dual track: uma visão atualizada"
excerpt: Entendendo o contexto de ciclos de aprendizado e entrega em um processo de construção de produto
authors: Pablo Silva
date: 2021-05-19
publishDate: 2021-05-19
image: https://i.imgur.com/MFNuZEg.jpg
type: post
feature_post: true
sponsor: awari
categories:
  - Tático
  - Opinião
tags:
  - framework
  - times
  - discovery
---

A primeira vez que eu tive contato com o termo Dual Track foi num artigo da DZone que eu não consegui mais achar o link, isso no final de 2015. Eu era trainee da Locaweb e fui desenvolver um "projeto de agilidade" nas equipes de engenharia, o que me levou a pesquisar tudo o que eu conseguia sobre agilidade, fluxos de trabalho e interação dos times no dia a dia.

Por acaso, acabei encontrando um post no medium do Kevin Albrecht, onde ele detalhou o que ele chamou de [Dual Track Agile: Focusing on Customer Value](https://medium.com/kevin-on-code/dual-track-agile-focusing-on-customer-value-a2e39312585b) (Focando no valor para o cliente) e foi onde eu encontrei essa imagem que mostra o fluxo de trabalho como um todo

![](/images/posts/dual-track-uma-visao-atualizada-1.png "Dual Track Agile por Kevin Albrecht")

E deste então eu tenho usado essa imagem toda vez que eu falo sobre dual track no contexto de descoberta e entrega de produto. Essa imagem realmente me ajudou muito durante todos esses anos, mas como tudo na vida, as coisas evoluem e acabam mudando e por isso, eu resolvi criar uma nova imagem sobre a minha visão atualizada desse framework que é um dos mais utilizados no mercado de gestão de produto.

## O ano é 2021

Sem mais delongas, o desenho completo do dual track 2021, na minha visão, é o seguinte

![](/images/posts/dual-track-uma-visao-atualizada-2.jpg "Dual track 2021")

Você pode encontrar a imagem em alta definição [nesse miro](https://miro.com/app/board/o9J_lOOR3c0=/). Como vocês podem ver, existem algumas grandes mudanças no desenho e vou explicá-las a seguir.

## Foco na estratégia

A primeira grande mudança para o desenho anterior é sobre estratégia, o que para mim é o segundo (o primeiro é cultura, claro!) ponto mais importante em uma empresa e para qualquer área. Se não há uma estratégia bem definida, clara, transparente e alinhada o máximo possível com a empresa toda, o risco de cada uma das áreas estar indo para direções diferentes é muito grande.

Em condições ideais de estrutura organizacional, a estratégia do negócio se deriva da Missão e Visão. É basicamente a resposta para a pergunta: como vamos atingir a nossa visão e cumprir a nossa missão no tempo?

![](/images/posts/dual-track-uma-visao-atualizada-3.jpg)

Como geralmente os negócios se estruturam em anos fiscais, sempre temos ciclos anuais de planejamento estratégico. Não que a estratégia seja escrita em pedra para o ano todo, mas é importante pelo menos ter o ponto de partida claro.

A partir do momento que temos a estratégia de negócio bem definida, o próximo passo é a líder, junto com outras pessoas de produto, definirem a estratégia de produto e como ela se conecta com a estratégia de negócio. 

É fundamental que haja uma relação de causalidade direta entre a estratégia de produto e a de negócio, ou seja, se a estratégia de produto for atingida, a de negócio automaticamente será também. Aqui é importante falar que a estratégia de produto precisa estar bem estruturada e interligada com as áreas da empresa que impactam nos indicadores financeiros, como comercial, sucesso do cliente, marketing, atendimento e suporte. Sem essa relação bem estruturada, há um risco muito alto de o resultado da empresa não vir.

![](/images/posts/dual-track-uma-visao-atualizada-4.jpg)

E por último, ainda falando de estratégia de produto, o próximo passo é como quebrá-la pelos times que de fato desenvolvem o produto, geralmente formados por product manager, product designer e dev(a)s. 

![](/images/posts/dual-track-uma-visao-atualizada-5.jpg)

E aqui vai mais uma grande mudança do desenho anterior, não temos time de descoberta e time de entrega, nós temos time. Cada time tem uma parte específica da estratégia, onde todos do time são responsáveis por atingi-la. Sem silos, onde o(a) PM e o(a) PD trabalham juntos e depois entregam para o "time" de desenvolvimento o que precisa ser feito.

O time que vai decidir junto qual é a melhor maneira de se organizar em relação a descoberta e a entrega. Devs vão participar das entrevistas? O(A) PD vai ficar perto no desenvolvimento para realizar mudanças rápidas? O(A) PM que vai ficar responsável sempre por falar com as pessoas de negócio? Esse tipo de organização é de responsabilidade total do time, nessa visão de dual track.

## Descoberta como experimento

A principal mudança no ciclo de descoberta em relação ao desenho original é sobre o famigerado backlog. Ao invés de ter um backlog de ideias, temos agora um backlog de hipóteses. A ideia aqui é de fato tratar todas as demandas que não são de investimento (aquelas relacionadas a regulamentações e segurança por exemplo) como hipóteses.

![](/images/posts/dual-track-uma-visao-atualizada-6.jpg)

Essas hipóteses podem ser levantadas dentro da própria empresa, com o time de vendas, CS, atendimento e marketing, através das pesquisas e entrevistas que fazemos com os usuários e os dados que temos disponíveis e das reclamações e pedidos dos clientes. Que fique claro, toda informação pode ser importante, e as informações mais baratas de se conseguir estão dentro da empresa. As áreas que mais falam com os usuários sempre vão ter informações que podem (ou não) mostrar caminhos que o time não estava enxergando até então. Por isso, é muito importante estar perto dessas áreas e trabalhar junto mesmo. Dessa forma o custo do aprendizado diminui.

É normal ter um backlog de hipóteses muito grande, porém muitas dessas hipóteses podem ser facilmente invalidadas se o time manter o foco na estratégia que foi definida, ponto fundamental para atingir os resultados esperados. Acredite em mim, a maioria delas não vai fazer o time atingir o resultado que está buscando e só vai tirá-lo do foco. Por isso, repito aqui, o foco do time tem que ser a estratégia que foi definida e não entregar um monte de coisas.

Uma vez que que agora temos hipóteses, temos a segunda grande mudança no ciclo de descoberta, que são os experimentos. O que fazemos aqui é tentar entender se ao implementarmos algo, o resultado que estamos buscando virá. Por exemplo, se estamos buscando aumentar o número de transações aprovadas no cartão de crédito, implementar uma carteira digital onde se pode colocar múltiplos cartões pode fazer com que essas transações aumentem?

Temos duas maneiras gerais aqui de realizar um experimento desse tipo: envolvendo código ou não. Como escolhemos? Basicamente o que for mais barato.

Vamos supor que consigamos armazenar múltiplos cartões no banco de dados a mão. Podemos então pegar uma amostra de usuários que topariam testar essa hipótese com a gente e eles solicitarem os cartões para os clientes, nos mandarem. Armazenamos no banco e então roteamos as transações com falha para outros cartões. Isso vai te dar uma amostra já da performance de aprovação e com isso você conseguiria projetar.

Agora vamos supor que não conseguimos fazer o que falamos no exemplo anterior ou fazer dessa forma demoraria vários dias, por várias questões, como não conseguir encontrar usuários que topem, ou aprovação da área de segurança por exemplo. Diante desse cenário, a escolha então seria escrever um código de teste (um código meio lixo mesmo), que depois vai ser jogado fora ou melhorado, caso a performance de aprovação aumente.

Muitas vezes pode ser que testar com código seja mais barato e muitas vezes nem vai ser possível testar sem código. O importante é isolar o acesso ao código liberado para um grupo de controle, medir a performance do experimento e validá-lo ou não. Se não, simplesmente jogue o código fora e parta para a próxima hipótese, se sim, vá para o ciclo de entrega e melhore o que precisa ser melhorado na funcionalidade até que ela possa ser lançada para base toda.

## Nunca é tarde para mudar
Uma vez que um experimento é validado e temos uma projeção do resultado que vamos conseguir implementando e entregando a funcionalidade em produção, agora é a hora do ciclo de entrega.

![](/images/posts/dual-track-uma-visao-atualizada-7.jpg)

A principal mudança nesse ciclo é entender que mesmo após colocar em produção e mesmo com o risco de se estar errado diminuído com os experimentos, pode ser que o valor não seja de fato entregue. Muitas coisas podem acontecer, desde o contexto do usuário não ajudar até experimentos errados, com amostras estatísticas de baixa confiança. O importante aqui é entender que nunca é tarde para mudar, só pode ser que seja bem caro.

Se ficar realmente entendido que houve um erro, a melhor ação é de fato retirar a funcionalidade do ar. Mais funcionalidades, mais suporte, mais bug para tratar, mais débito técnico para pagar. Sem contar que pode tornar o produto mais complexo.

A segunda principal mudança que não existia na imagem do Kevin é que a entrega de valor era só para o usuário. Se você olhar para imagem, não há nada falando de valor entregue para o negócio. Como falei na parte da estratégia, se as entregas do time não levarem ao atingimento da estratégia de produto, as escolhas feitas foram erradas. É fundamental enxergar as métricas se movimentando com as entregas e se não, mudar o curso mais rapidamente possível.

## Fechando o ciclo

Se tudo o que falamos funcionar, vamos ter o resultado da imagem a seguir

![](/images/posts/dual-track-uma-visao-atualizada-8.jpg)

Quanto mais acertamos nos ciclos de descoberta e entrega, mais perto levamos a empresa a atingir sua estratégia e por consequência, se a estratégia for a correta (o que não depende dos times de produto), mais perto a empresa estará de sua visão e mais estará cumprindo a sua missão.

Como vimos, todo esse fluxo é composto de várias partes que são agregadas por várias áreas. Na teoria é lindo de se ver, mas na prática pode ser um pouco mais complicado do que se parece. 

No dia-a-dia é provável que você não tenha tudo o que precise para fazer experimentos. Vai faltar dados, apoio, vai ter pressão, insegurança de colocar código de baixa qualidade em produção, os usuários não aceitarão participar dos testes, demandas vindo da diretoria que precisam ser feitas e assim vai.

A proposta aqui não é ter um fluxo perfeito, mas sim um framework que te ajude, no contexto do time, com os recursos disponíveis, tomar a melhor decisão na busca de gerar valor para as pessoas e para a empresa.


## Referências:

https://medium.com/kevin-on-code/dual-track-agile-focusing-on-customer-value-a2e39312585b