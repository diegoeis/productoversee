---
title: Tornando o refinamento mais efetivo — Parte 1
excerpt: O refinamento pode evitar lead times altos demais e trazer ciclos de aprendizado mais curtos
authors: Pablo Silva
date: 2020-05-13
publishDate: 2020-05-13
image: https://i.imgur.com/CVzesbq.png
type: post
featured_post: true
sponsor: awari
categories:
  - Tático
tags:
  - ferramenta
  - agile
  - processo
---
O refinamento é uma das cerimônias mais importantes num fluxo de desenvolvimento de produto. É nessa cerimônia que temos a chance de diminuir incertezas e complexidades nas histórias que decidimos priorizar para desenvolvimento.

É muito importante que se diminua complexidade, pois todo item com esforço muito grande que entra no fluxo de desenvolvimento, tem um alto risco de aumentar muito o Lead Time (já falei sobre a importância de um PM entender o Lead Time [nesse texto](https://medium.com/@phsil/duas-m%C3%A9tricas-%C3%A1geis-super-importantes-para-pms-a060aaa1732f)) porque nunca é só desenvolver, esse código terá que ser revisado, testado e depois colocado em produção. Quanto maior a unidade de esforço, maior o risco também de subir bugs porque a solução vai se tornando mais complexa, é um efeito natural e que vai acontecer em algum momento.

É muito importante que se diminua a incerteza no máximo possível, porque quando se tem incerteza sobre os critérios de aceite, há uma grande chance do item travar no meio do desenvolvimento quando essas indefinições se concretizam. Item travado no fluxo, lead time aumenta e consequemente se demora mais pra entregar valor ou validar experimentos.

## A matriz de complexidade e incerteza

Uma vez a galera da antiga Plataformatec que estava prestando uma consultoria de agilidade para a Vindi, mostrou essa matriz:

[![](https://cdn.substack.com/image/fetch/w_1456,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F69b9253e-89e3-42c6-a001-4c694ab65524_700x393.png)](https://cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F69b9253e-89e3-42c6-a001-4c694ab65524_700x393.png)

E, utilizando ela em todos os seus refinamentos, vai te ajudar muito e os desenvolvedores, metodicamente, a entender se uma história tem complexidade e esforço aceitáveis para entrar no fluxo de desenvolvimento.

Como vocês podem ver, se o item de trabalho não estiver nos quadrantes 1, 2, 3 ou 4 é um indicador que se precisa remover complexidade ou incerteza e nos piores, casos os dois. É um ótima ferramenta que recomendo se utilizar em todos os refinamentos, sem exceção. Tornar o refinamento metódico é algo que ajuda muito a fazer com que ele seja mais efetivo e então, conseguirmos diminuir o lead time.

## Como identificar incerteza

Algumas perguntas vão te ajudar a identificar incertezas no refinamento:

* Está clara a regra de negócio dessa história? Todos os critérios de aceite estão claros?
* Existe algum impedimento externo?
* Se vamos utilizar um serviço externo, os desenvolvedores já tem domínio de como utilizar o serviço?
* Os desenvolvedores já tem conhecimento dessa parte do código que terá que ser alterada? (Para casos de legados complexos)
* Se vamos utilizar uma API externa, ela está funcionando tanto no ambiente de testes quanto em produção? Temos todos os acessos para autenticação?
* Existem restrições de segurança que precisam ser atendidas?
* Todos os usuários podem ter acesso a essa funcionalidade?
* Existem validações específicas que precisam ser implementadas?
* Sabemos os possíveis erros que podem acontecer com a interação do usuário e como tratá-los?
* Temos todos os layouts, protótipos e guia de front end que vão ser necessários para desenvolver as telas?

É claro que tem muito mais. Uma técnica que eu uso é toda vez que surge uma pergunta nova, coloco na lista de perguntas que sempre vou fazer para identificar incertezas no refinamento. Atualmente, várias delas tenho feito antes mesmo de abrir um refinamento, pois eu mesmo posso resolver.

## Como identificar esforço

Geralmente, a percepção de esforço vem dos desenvolvedores. Algumas vezes eles abrem o código ali mesmo na hora para terem uma percepção melhor sobre o que precisa ser feito, principalmente quando eles nunca mexeram nessa parte do código.

No geral, uma quantidade muito grande de critérios de aceite, é indicador que a história terá um esforço grande para ser feita. Isso é sinal de que você poderia quebrar a história, talvez deixando as validações ou algum estilo mais elaborado para uma próxima história.

A melhor maneira de você conseguir entender se uma história está com esforço muito grande é identificar quantos comportamentos você está querendo alterar em uma história só. Por exemplo, se você, numa história quer criar um novo relatório e nessa história coloca como critérios de aceite que sejam listadas todos os registros, seja possível filtrar, tenha um cabeçalho de consolidação dos dados, tenha um gráfico de barras e possíveis ações para cada registro listado, certamente essa história está "grande" demais. Tudo isso que eu falei podem ir em histórias separadas.

Um dos principais pontos é você sempre pensar em comportamentos que você quer dar para o usuário que antes ele não tinha. Na próxima Letter sobre refinamentos, vou dar um exemplo prático sobre esse tema. Até lá!

### Referências:

* [Requisitos em equipes ágeis: Falando sobre complexidade e incerteza](http://blog.plataformatec.com.br/2017/01/requisitos-em-equipes-ageis-falando-sobre-complexidade-e-incerteza/)
* [Fifty Quick Ideas To Improve Your User Stories](https://www.amazon.com.br/Fifty-Quick-Improve-Stories-English-ebook/dp/B00OGT2U7M/ref=sr_1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=Quick+ideas+to+improve+your+users+stories&qid=1589245196&sr=8-1)