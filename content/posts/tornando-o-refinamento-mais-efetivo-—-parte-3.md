---
type: post
title: Tornando o refinamento mais efetivo — Parte 3
excerpt: O refinamento pode evitar lead times altos demais e trazer ciclos de
  aprendizado mais curtos
authors: Pablo Silva
date: 2020-05-15
publishDate: 2020-05-15
image: https://i.imgur.com/CVzesbq.png
categories:
  - Tático
tags:
  - ferramenta
  - agile
  - processo
---
No [segundo artigo](https://productoversee.com/tornando-o-refinamento-mais-efetivo-parte-2/) desta série sobre refinamento, falei sobre o conceito de novas capacidades e como ter esse tipo de visão ao escrever histórias, pode reduzir substancialmente a quantidade de esforço na hora de desenvolver e consequentemente, diminuir o risco de que o lead time aumente demais.

Nesse terceiro, e último artigo dessa série, vamos focar em entender como retirar incerteza das histórias, antes que os desenvolvedores comecem a de fato escrever código. Levar uma história com muita incerteza para frente, leva também um grande risco de que ela possa ficar travada em algum momento do fluxo de desenvolvimento. Já vi exemplos de uma histórias que ficaram travadas por meses, porque a incerteza não foi retirada no refinamento.

## A incerteza sempre está nos critérios de aceite

Como PM, uma de suas missões, é retirar o máximo de incerteza possível antes de que a história chegue no backlog de desenvolvimento. Nem sempre isso vai acontecer em sua totalidade e também não acho que seja possível retirar a incerteza 100%, por isso, utilizar técnicas para retirar incertezas no refinamento é algo fundamental.

No geral, a incerteza sempre vai estar nos casos de uso, ou seja, nos critérios de aceite. Então, vamos utilizar o exemplo do artigo anterior, onde imaginamos que vamos implementar uma página de login e colocamos os seguintes critérios de aceite:

* Está pronto quando só usuários previamente cadastrados conseguem ter sucesso ao realizar o login com usuário e senha
* Está pronto quando for possível fazer login via Facebook
* Está pronto quando for possível fazer login via Google
* Está pronto quando for possível fazer login via Twitter
* Está pronto quando for possível fazer login via Apple

Nesse caso, vamos usar o critério de aceite de fazer login via Facebook. Esse é um caso que o PM já poderia e deveria retirar bastante a incerteza desse critério, então considerando que ele não fez isso, podemos fazer as seguintes perguntas no refinamento:

* Temos acesso a API do Facebook?
* A API do Facebook tem requisitos mínimos para ser utilizada?
* Alguém do time já sabe como lidar com essa API?

Muitas vezes, a gente pode achar que fazer uma integração com a API do Facebook é algo simples, mas, se a gente não tiver controle das respostas dessas perguntas e a história entrar para desenvolvimento, várias coisas podem acontecer, como por exemplo:

* Achamos que tínhamos acesso a API mas não tínhamos e leva 30 dias para que o Facebook homologue um novo parceiro (é claro que aqui é extremo, mas quando falamos do sistema bancário, por exemplo, isso é bem comum). Logo, a história vai ficar travada esse tempo todo.
* Para ser homologado, precisamos mandar uma prova de performance da nossa infraestrutura. Fizemos o teste e nesse momento, para fazer esse teste de carga, vamos ter que subir mais máquinas na infraestrutura, o que demora 5 dias para conseguir autorização desse custo.
* Ninguém do time sabe lidar com a API do Facebook, então por si só, já tem uma incerteza técnica muito grande de como fazer. Isso certamente vai pesar no lead time e pode ser que a solução seja muito maior do que a gente pensou que fosse.

## Usando spikes para retirar incertezas

Uma das melhores técnicas para retirar incertezas das histórias é utilizar spikes. Spikes vieram dos Scrum/XP, onde é preciso estimar as histórias e quando as pessoas não tem conhecimento nenhum sobre o que precisa ser feito, fica muito difícil estimar. Por isso, criaram esse tipo de task que é basicamente uma atividade de pesquisa.

No geral a estrutura que eu uso para spikes é a seguinte:

> **Título:** Estudo para entender a API do Facebook
>
> **História associada:** Link para história que levou a esse spike.
>
> **Critério de aceite com incerteza**: Está pronto quando for possível fazer login via Facebook
>
> **Objetivo:** Precisamos entender como a API do Facebook funciona para que possamos ter certeza que não vamos ter um bloqueio na hora de desenvolver o critério de aceite especificado.
>
> **Definição de pronto:** Chamada de autenticação na API do Facebook
>
> **Timebox:** 2 dias

O spike pode responder também uma pergunta específica, por exemplo, se temos acesso a API do Facebook ou ser um estudo de como lidar com software que a gente não tem entendimento nenhum.

Fundamentalmente, um spike precisa ter um entregável que garanta que a incerteza foi retirada. Então, geralmente as entregas dele vão desde documentações autoexplicativas, até códigos que vão ser jogados fora, porque eram só para provar a capacidade de fazer algo.

Um último conceito muito importante sobre spikes é que eles tem timebox. É pra ser algo simples, não faz sentido um spike demorar tanto porque senão a incerteza é tão grande que isso indica que o PM precisa de fato voltar a definição de negócio da história, porque talvez falhou a pergunta sobre se era “factível” tecnicamente fazer essa nova funcionalidade ou incremento.

## Quando a incerteza de negócio é grande demais

Um outro tipo de incerteza que pode acontecer além da técnica é a de negócio. A gente tende a simplificar as coisas em software, mas não caia nesse conto. Muitas vezes requisitos de negócio que parecem ser simples, podem levar a ter que escrever um caminhão de código para ser resolvido.

Uma ótima prática para retirar esse tipo de incerteza é falar com especialistas sobre o negócio ou com pessoas que já passaram por problemas similares aos seus.

Um exemplo prático que passamos na Vindi foi quando fomos definir as regras de como vamos fazer antecipação de recebíveis para os nossos clientes. Olhando por cima parece algo simples: basicamente é pagar o cliente antes pelo dinheiro que ele receberia dali um mês. Simples não? Pois é, de maneira nenhuma. Tem tantas regras de negócio por trás que não necessariamente é simples de enxergar, como lidar com pagamentos em feriados, pagamentos aos finais de semana, risco de pagar e depois o cliente não receber (o tal do chargeback), risco de fraude, como lidar com o banco que vai realizar os pagamentos, é regulado pelo Banco Central?, precisamos usar canais específicos que são regulados pela Banco Central? e assim vai, poderia citar aqui muitas mais incertezas que existem quando você nunca passou por isso.

Nós retiramos todas essas incertezas falando com especialistas de antecipação do mercado e isso nos ajudou a criar histórias com muito mais detalhes e muito menos incertezas, tornando o nosso fluxo de desenvolvimento muito mais fluído. É claro que nosso cenário é muito crítico porque lidamos com dinheiro e risco muito alto, então fazer esse tipo de questionamentos se tornou algo normal pra gente, mas eu já vi exemplos em outras empresas que essas incertezas não foram retiradas e aí o lead time foi as alturas ou até mesmo meses de trabalho foram desperdiçados.

## O tempo para aprender está cada vez menor

Eu levo esse tema de retirar incerteza e complexidade das histórias muito a sério. A principal razão para eu fazer isso é que quanto maior o lead time mais tempo vamos demorar para aprender algo e vou te dizer, o mercado não espera.

Você como PM pode influenciar muito esse tempo se você “cuidar bem” das histórias que você escreve. Passar incerteza e esforço para desenvolvimento é algo muito mais comum do que a gente imagina, mas quanto mais metódico você for nos refinamentos, usando a matriz de complexidade e incerteza que mostrei no primeiro artigo e fazendo perguntas chaves que vão questionar muito a “saúde” dessa história, mais o time consegue manter o fluxo fluido e saudável. Isso com certeza, vai diminuir o tempo para que você aprenda se as suas decisões estão de fato gerando o resultado que você estava esperando ou se você precisa mudar a direção. Até que o usuário de fato use, tudo ainda é hipótese!

## Referências

[Better User Stories](https://www.betteruserstories.com/courses/better-user-stories/videos?video_id=1)

[Método SPIDR](http://s3.amazonaws.com/betteruserstories/videos/bonus_downloads/000/000/014/original/spidr-poster.pdf?1524602363)