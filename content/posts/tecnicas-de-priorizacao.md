---
type: post
title: Técnicas de priorização
excerpt: Compartilhando algumas técnicas de fatiamento para auxiliar no seu dia a dia de escrita de histórias
authors: Éricka Padilha
date: 2021-08-25
image: https://i.imgur.com/87aP1bG.png
sponsor: awari
categories:
  - Tático
tags:
  - processo
  - metodologia
---

Uma das tarefas diárias de uma pessoa de produtos, em especial quem trabalha no papel de PO é realizar o fatiamento das histórias e épicos, desta forma, irei abordar alguns motivos de fatiar e algumas técnicas.

PO tem como missão maximizar o resultado do trabalho do time de desenvolvimento para entregar valor para o cliente e para empresa. E trazer clareza sobre os próximos itens do backlog, as metas e objetivos, ter tudo bem visível e transparente é essencial para o time entender o caminho que está seguindo e o quanto perto está de seu objetivo.

Mas não adianta nada estar tudo bem claro, mas cada próxima história ser do tamanho de um livro da J. K. Rowling, por isso é preciso aprender e exercitar continuadamente essas técnicas (e algumas outras), afinal, quando algo simples chega até nossas mãos é mais fácil pensamos que será fácil de resolver e atender o objetivo.

## E por que gastar tempo fatiando??

O primeiro ponto de todo é: se é SIMPLES consideramos FÁCIL de fazer, e mais do que isto, o tempo para seguirmos um ciclo básico de PDCA (Plan, Do, Check e Action) é menor, facilitando que a validação sobre o valor que desejamos entregar e corrigindo a rota caso necessário.

Com o fatiamento conseguimos:

* **Validar mais rápido** pedaços de uma **feature maior**, não precisando esperar o conjunto completo para verificar a utilidade de algumas coisas;
* **Reduzir os riscos** do negócio/produto com as validações que ocorrem durante a construção (podendo inclusive incluir o cliente durante as etapas);
* Mais rápido poderá **validar hipóteses** de negócio (ciclo construir-medir-aprender);
* Mais rápido será a construção do produto, principalmente em MVP que é importante lançar logo para ter o timing de mercado;
* **Menos incertezas** no desenvolvimento (aprendizado);
* Deixa **mais simples e objetivo**, o que reduz a **complexidade**;
* Reduz o custo de desenvolvimento (menor complexidade, menor risco, pacotes menores de entrega e validação);
* Facilita a entrega e sua validação;
* **Facilidade na comunicação**, quando conseguimos reduzir as incertezas e complexidade é mais fácil passar o recado e clarificar qual é o objetivo;
* **Redução de desperdício** e custos (com retrabalhos ou trabalho que não gera valor ao negócio).

Beleza, entendemos os motivos, vamos olhar algumas técnicas

# COMECE PELO PROBLEMA

Parece óbvio né? Então, qual é a grande dor que seu produto está enfrentando? Comece sua fatia por este problema, aqui segue um exemplo:

* Grandes quantidades de chamados juntos a central de atendimento ao cliente;
* Maioria das ligações devido a uma mensagem confusa e baixo tempo de duração em tela que ocorriam na inicialização do app.
  * 2.043 chamados / mês
  * R$ 5,52 custo por chamado
  * R$ 11.277,36 / mês
* Objetivo: reduzir o número de chamados e consequentemente o valor gasto na central;
* Solução: Mensagem mais amigável e com maior tempo de duração.

![](/images/posts/tecnicas-de-priorizacao-1.png)

# DADOS DE ENTRADA E SAÍDA

Por vezes é uma tentação trazer em uma única história a solução completa, o entendimento muitas vezes é que não custa nada adicionar só mais um campo, ou no meu exemplo, só mais um filtro.

Quando iniciamos com pontos menores podemos lançar com mais rapidez ao mercado e validar o uso da funcionalidade, receber feedback dos clientes se há necessidade de evolução. E sim, conheço histórias da inclusão de todos os filtros que nunca foram se quer usados pelos usuários.

![](/images/posts/tecnicas-de-priorizacao-2.png)

# SOLUÇÃO MAIS SIMPLES

Evitar trazer grande complexidade e pensar em todos os cenários de problemas possíveis, o importante é trazer soluções que atendam o momento atual e lembrar que a evolução irá existir.

Um exemplo disso é uma aplicação onde o cliente atual atendido possui um conhecimento mais técnico, e a opção de retorno de resposta para este cliente é a utilização do padrão HTTP, onde para clientes desse nível receber uma mensagem 200 (sucesso) ou 404 (not found) não é estranho.

![](/images/posts/tecnicas-de-priorizacao-3.png)

# POR CANAL DE INTEGRAÇÃO

Quando temos histórias que envolvem a integração com outros canais é importante entender seu cliente para identificar por qual deve se iniciar, e cada fatia deverá corresponder há um canal diferente. No exemplo temos como necessidade a opção de compartilhar a informação de comprovante, para que isto seja feito temos que integrar com plataformas externas que nos auxiliem no envio do comprovante.

Sendo assim podemos iniciar pelo que possui mais aderência ao cliente, e que já possibilite o envio do produto para produção.

![](/images/posts/tecnicas-de-priorizacao-4.png)

# POR CONTEÚDO

Este é mais um caso onde entender as necessidades do cliente é importante, além de identificarmos o que é mais simples para entregar valor e iniciar o processo de validação de um produto. No exemplo, trago um app de pagamento onde inicialmente só era possível realizar transações escolhendo o meio de pagamento desejado, mas numa segunda fatia há outra opção extra: escolher iniciar o fluxo pelo valor.

![](/images/posts/tecnicas-de-priorizacao-5.png)

# USUÁRIO

Em alguns produtos temos mais de um usuário, sendo assim podemos fatiar de acordo com cada um deles. Entregando valores conforme as necessidades de cada usuário. Um exemplo disso é uma plataforma para consulta de produtos da empresa, e o primeiro usuário é o interno, sendo este utiliza de forma constante o computador, sendo assim a primeira fatia pode estar associada a realizar consultas via web em um site, e podemos no futuro transformá-lo em um app para atender os clientes externos.

# PLATAFORMA

É preciso identificar qual é a plataforma mais relevante para o produto, ou seja, aquela que seu usuário mais utiliza ou que terá maior retorno. Assim é possível fatiar de acordo com a plataforma que esteja mais aderente ao objetivo e traga maior retorno.

Um ponto importante é olhar não apenas para plataforma, mas como para versão de Browser, tamanho de tela, versão do Sistema Operacional entre outros dados para que as fatias estejam realmente trazendo maior valor conforme as características de seu usuário e produto. 

# Referência:

Estas técnicas foram algumas que aprendi no Treinamento para Product Owners da K21. 


