---
type: post
title: O débito técnico de hoje é a urgência de amanhã
excerpt: Os débitos técnicos podem afetar profundamente o negócio
authors: Pablo Silva
date: 2020-10-29
tags: [Negócios]
categories: [Opinião, Tático]
image: https://images.unsplash.com/photo-1500099817043-86d46000d58f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2734&q=80
featured_post: true
---

É comum que tenhamos que fazer decisões difíceis de priorização na
construção de software. Não apenas priorizações de produto, mas também
priorizações técnicas, onde soluções perfeitas precisam esperar para dar
lugar para soluções incompletas, mas que resolvam o problema imediato.
Quando isso acontece, é muito comum que procrastinemos a continuação e a
evolução dessas soluções técnicas. E essa é uma das maneiras que os
débitos técnicos nascem.

Débitos técnicos são parecidos com cartão de crédito: se você não pagar
a fatura, os juros aumentam seu débito, até o ponto que não há como
pagar a fatura completa, forçando você a parcelar a dívida. Outro ponto
é que você poderá ficar com o nome sujo na praça, acarretando uma série
de problemas de curto, médio e longo prazo para o produto.

**Por que priorizar débitos técnicos é algo muito importante**
--------------------------------------------------------------

No cartão de crédito você até tem a opção de ficar inadimplente, agora,
no mundo de construção de software, ficar inadimplente pode significar
risco de continuidade do negócio.

Um exemplo prático: aqui na Vindi temos uma atenção redobrada com as
atualizações de segurança dos frameworks que usamos. Já deixamos o Rails
desatualizado durante muito tempo e uma versão mais atual corrigiu uma
falha de segurança muito crítica, que para o contexto do mercado
financeiro, é imprescindível que corrigíssemos. Como não tivemos a
rotina de atualizar o Rails assim que as novas versões eram publicadas,
tivemos que ficar quase um mês em um processo de atualização para
alcançar a versão mais atual, com o objetivo de evitar riscos de
funcionamento da plataforma.

Decidir não pagar esse débito de falha de segurança era assumir um risco
de dívida que não quisemos apostar, contudo, pagamos muito caro, tendo
que parar o time durante muito tempo, atrasando possíveis melhorias e
novidades que fariam o produto entregar mais valor.

Outra razão bastante importante para priorizar esses débitos é que em
algum momento você vai ouvir a seguinte frase: "Era pra essa alteração
ser muito simples, mas a arquitetura do nosso sistema é toda acoplada e
tem várias camadas, então quando mexemos numa camada, pode ter impacto
em todas as outras, ou uma simples alteração vai demorar dias ao invés
de horas pra ser feita.". Quando chegamos nesse nível já podemos saber
que o lead time das histórias poderia ser menor, mas não é pela
quantidade de débitos técnicos que foram deixados pra trás. O efeito
disso para o negócio é perder timing e competitividade, porque
alterações importantes e novas funcionalidades vão demorar um tempo
maior para irem pra produção. Aqui na Vindi também passamos por isso.

No final, o preço vai ficar muito caro e acabar prejudicando o negócio
em proporções que podem ser desastrosas.

**Duas técnicas para priorizar débitos técnicos sem custar tão caro**
---------------------------------------------------------------------

Na Vindi utilizamos duas técnicas para pagar débitos técnicos
continuamente e evitar que a conta fique muito cara.

A primeira forma que encontramos, é o que chamamos de **bloqueio
tecnológico**. Toda história de usuária antes de ser feita passa por uma
etapa de especificação. Nessa etapa, as engenheiras discutem sobre a
solução técnica daquela história e identificam se aquela parte do código
precisa ser melhorada, tanto em questão de qualidade do código, quanto
em qualidade e cobertura dos testes. Se a qualidade de um desses dois
quesitos for baixa, definimos que a história tem um bloqueio tecnológico
e a gente paga esse débito criando uma outra história técnica que será
feita antes da história de usuário. Dessa forma a gente sempre paga e
evita débitos técnicos.

A segunda tem relação com o nosso kanban. Como usamos esse método para
gerenciar nosso fluxo de trabalho e medimos todo o fluxo, nós sabemos
qual é a capacidade de WIP (work in progress) de cada equipe. Dessa
forma, para as equipes que identificamos que a conta está ficando alta
demais, decidimos ter um backlog técnico e um backlog de negócio, e
criamos uma raia no kanban onde só podem passar histórias técnicas com
uma capacidade de WIP que nos permita manter o equilíbrio entre técnico
e negócio, como na imagem a seguir

[![](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/912b8191-2548-475b-a8ac-3d80202b4d1e_900x578.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F912b8191-2548-475b-a8ac-3d80202b4d1e_900x578.png)

Nesse exemplo, a raia de itens técnicos tem um WIP (Work in Progress)
máximo de 1 e a capacidade do sistema todo é 3, deixando 2 para o
backlog de negócio. O backlog técnico é totalmente priorizado e
gerenciado pelas engenheiras, que decidem o que está mais crítico
naquele momento e atrapalhando o lead time das histórias.

Essas duas formas tem se mostrado bastante efetivas, pois acompanhamos
nosso lead time de perto e ele tem uma distribuição pouco dispersa e com
uma média móvel saudável.

**Tá, mas como convencer a liderança a pagar o preço?**
-------------------------------------------------------

A melhor maneira que encontrei para convencer a liderança de que
priorizar débitos técnicos é algo bastante importante foi mostrar o
histórico do lead time das equipes e como estávamos perdendo velocidade
no negócio. Tínhamos a dispersão controlada, mas num nível alto demais,
então muitas alterações que seriam bem simples do ponto de vista
técnico, demoravam muito e estava claro pra gente que era nossa
arquitetura.

Outro ponto que funcionou foi levantar e explicar os riscos de negócio
que tínhamos não priorizando as atualizações dos frameworks e outras
partes do código que nos colocavam em riscos como vazamento de dados por
exemplo. A partir desse dia, começamos a trabalhar junto com a equipe de
segurança para levantar as brechas de segurança continuamente e criamos
uma rotina de priorizações dos frameworks antes que essas brechas se
tornassem um problema grave.

**O débito técnico de hoje é a urgência de amanhã**
---------------------------------------------------

Algo que as empresas precisam entender é que débitos técnicos
naturalmente vão surgir no negócio. Tecnologias se atualizam com
frequência, novas formas e abordagens de escrever código surgem e a
maneira como o software foi desenvolvido nem sempre atenderá a
velocidade que o negócio precisa. É por isso que é muito importante que
débitos técnicos sejam considerados como demandas de investimento pelo
negócio e sejam priorizados.

A função da PM nesse caso é encontrar o equilíbrio máximo que ainda
permita que o negócio consiga de fato resolver os problemas dos clientes
e atinja os objetivos, mas que evite que os débitos técnicos se tornem
uma urgência e custam muito mais caros para ser pagos do que se
estivessem sendo priorizados ao longo do tempo.