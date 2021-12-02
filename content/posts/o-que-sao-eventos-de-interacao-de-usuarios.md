---
type: post
title: O que são eventos de interação de usuários?
excerpt: Como entender o que são eventos pode te ajudar a tomar melhores decisões no produto
authors: Arthur Martinho
date: 2021-11-24
image: https://i.imgur.com/cQ30Pqr.png
categories:
  - Indicadores e Dados
tags:
  - métricas
  - dados
---

Se você já trabalha com produto, provavelmente já esbarrou em alguma ferramenta de **análise de comportamento dos usuários**. Caso você ainda esteja na jornada de emplacar seu primeiro trabalho em produto, entender isso vai te ajudar nesse desafio.

E quando a gente fala de comportamento de usuário, muitas vezes a palavra **eventos** surge - e esse artigo é pra te explicar exatamente que diabos é isso.

Esse primeiro artigo vai fazer parte de uma série de outros 3:

* O que são eventos?📍**Você está aqui**
* Como podemos criar métricas de produto baseado em eventos?
* Quais são as ferramentas disponíveis para isso?

# O evento

Eu gosto da definição de eventos sendo **pequenos pedaços de informações gerados pela interação do usuário na plataforma**.

Para exemplificar melhor, vamos pra um produto bem conhecido - o Spotify.

Imagina que você quer mapear os possíveis comportamentos do usuário na tela de reprodução de músicas:

![](/images/posts/o-que-sao-eventos-de-interacao-de-usuarios-1.png)

Só nessa tela temos **diversas possíveis interações do usuário que geram esse pedaço de informação (eventos)**.

Alguns exemplos:

* Avançou a música
* Modo aleatório ativado
* Modo aleatório desativado (reparou que o mesmo botão tendo states diferentes representam ações diferentes?)
* Compartilhar a música
* Favoritar uma música 
* …

Beleza - agora que já entendemos o que é um evento, vamos aprofundar um pouco mais nos conceitos.

Sempre que você interage com o produto, dá pra tirar muito mais informações do que apenas qual evento você realizou.

Jura? Juro.

Sempre que você dá play ou pause, você tá fazendo isso em:

* Uma música
  * Que está dentro de um álbum (ou single, ou EP, etc)
    * Que pertence a um artista
      * Que pertence a um gênero musical

Nesse exemplo do print, se eu desse o play na música seria o seguinte

**Evento:** Play
**Música:** Sobre cafés e você
**Álbum:** Animalia
**Artista:** menores atos
**Gênero musical:** Rock

Esse tanto de informação que conseguimos tirar de uma única interação são chamados de **metadados** - ou seja - **dados de um dado**.

Normalmente você vai encontrar esses metadados sendo chamados de **propriedades de um evento**. 

# Mas e pra que servem os eventos?

Imagina que você precisa entender o comportamento dos usuários naquela tela de reprodução de músicas e vai analisar os eventos relacionados a isso.

Pra ficar mais visual eu montei uma planilha bem básica com alguns eventos hipotéticos registrados:

![](/images/posts/o-que-sao-eventos-de-interacao-de-usuarios-2.png)

A partir disso começam a surgir algumas análises como a distribuição de **gêneros mais tocados** entre 01/01/2021 e 06/01/2021 usando o evento **Play**.

![](/images/posts/o-que-sao-eventos-de-interacao-de-usuarios-3.png)

A partir de agora você já tem uma pista que os usuários têm ouvido mais Pop do que Rock na maioria dos dias - e que nos dias 03/01 e 05/01 você teve o pico de eventos na plataforma.

# E no que isso me ajuda?

Entender o comportamento do usuário dentro do seu produto é crucial para tomadas de decisões - priorizar o seu backlog, definir um roadmap e definição de OKRs são **decisões**.

E como saber que estamos tomando decisões que têm mais chances de darem certo? **Usando dados**. 

E é aí que os eventos entram - pra te auxiliar nessas análises e decisões de pra onde seu produto deve caminhar colocando o **usuário em foco**.

Saber que, nesse exemplo hipotético, os usuários da plataforma tendem a ouvir mais Pop do que Rock te ajuda a tomar alguma decisão no produto?

Sim - sem dúvidas.

Só tome cuidado. Não é pra você usar **apenas** a análise de eventos nas suas decisões, mas sim como um complemento. Existem diversos outros fatores que podem e devem interferir nas suas decisões, como o ROI de uma iniciativa, quanto de MRR está em jogo, custo de oportunidade, etc.

# Referências

* [What is Product Management Analytics](https://mixpanel.com/blog/what-is-product-management-analytics/)
* [Can We Make Better Decisions Using Product Instrumentation?](https://www.theproductfolks.com/blog/can-we-make-better-decisions-using-product-instrumentation)