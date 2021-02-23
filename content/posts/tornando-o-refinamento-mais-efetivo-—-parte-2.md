---
type: post
title: Tornando o refinamento mais efetivo — Parte 2
excerpt: O refinamento pode evitar lead times altos demais e trazer ciclos de
  aprendizado mais curtos
authors: Pablo Silva
date: 2020-05-14
publishDate: 2020-05-14
image: https://i.imgur.com/OhIHY7t.png
categories:
  - Tático
tags:
  - ferramenta
  - agile
  - processo
---
No [primeiro artigo](https://medium.com/@oseupablo/tornando-o-refinamento-mais-efetivo-parte-1-b75e8a17553d) desta série sobre refinamento, falei sobre como retirar complexidade e incerteza das histórias é algo bastante crítico pois pode influenciar diretamente no lead time das entregas do time e consequentemente no tempo que é levado para entregar valor.

Nesse segundo artigo, vamos focar em entender como “quebrar” histórias, e assim reduzir o esforço e o risco, utilizando uma técnica que chamei de novas capacidades (valor) para os usuários.

# Toda nova capacidade pode virar uma história

A maneira como eu sempre vejo histórias de usuário é de uma ótica de novas capacidades que eu pretendo entregar para os usuários ao entregar uma história em produção. Aliás, se você escreve uma história que não vai permitir que o usuário tenha acesso a nenhuma nova capacidade, então é melhor não fazê-la. É claro que histórias técnicas geralmente não entregam valor visível para o usuário, sendo a única exceção cabível que enxergo para furar a afirmação que acabei de fazer.

Para exemplificar o que eu acabei de falar, imaginemos que vamos implementar uma página de login e colocamos os seguintes critérios de aceite:

* Está pronto quando só usuários previamente cadastrados conseguem ter sucesso ao realizar o login com usuário e senha
* Está pronto quando for possível fazer login via Facebook
* Está pronto quando for possível fazer login via Google
* Está pronto quando for possível fazer login via Twitter
* Está pronto quando for possível fazer login via Apple

Nesse exemplo, eu vejo várias novas capacidades que os usuários vão ter acesso depois que a gente colocar essa história no ar: poder fazer login com usuário e senha, poder fazer login com a conta do Facebook, poder fazer login com a conta do Google, poder fazer login com a conta do Twiter e poder fazer login com a conta da Apple.

É claro que é um cenário hipotético, vamos assumir que validamos e os nossos usuários realmente tem a necessidade de poder fazer login por tantos meios. Aliás, aproveitando o gancho, a primeira regra que uso no dia a dia é: “Se tem muitos critérios de aceite, desconfie, essa história pode estar gigante.” De fato, quando olhamos para a complexidade de implementar integração com tudo isso, depois usar todas essas integrações e garantir que temos todas as credenciais, o esforço realmente parece muito grande e é preciso quebrar para diminuir o risco.

Cada tipo de login pode e deve virar uma história separada e cada um deles pode virar mais duas histórias, uma para fazer a integração e a outra pra usar a integração. A lógica é, sempre que o usuário for ter acesso a uma nova capacidade, ela pode ser entregue de forma separada, gerando valor mais rapidamente.

# Um exemplo prático ao lidar com interfaces

Para exemplificar a técnica de capacidades que citei acima, vamos utilizar a seguinte interface

![Image for post](https://miro.medium.com/max/60/0*vjALP8HutTlhJj6z.png?q=20)

![Image for post](https://miro.medium.com/max/1456/0*vjALP8HutTlhJj6z.png)

que é um relatório de recebíveis de vendas por boleto.

Quando falamos de interfaces, um padrão que eu tenho visto é a história de usuário ser criada com o seguinte critério de aceite:

* Está pronto quando o layout anexo for implementado

E em alguns casos, alguns outros critérios relacionados com validações de dados por exemplo. O ponto aqui é, implementar uma tela pode ser algo muito, muito grande do ponto de vista de esforço. Cada elemento dessa tela, na pior das hipóteses, pode ter que ser gerada dinamicamente no backend e todo esse backend pode não existir ainda, o que seria um esforço gigantesco para colocar em uma história só.

Uma técnica que tenho visto ser aplicada em situações como essa é dividir a criação da tela em frontend e backend. Eu não sou adepto dessa técnica porque ela gera uma dependência desnecessária, pois o front terá que esperar o back e isso faz com que a entrega de valor demore mais para acontecer.

Dito isso, considerando então a técnica de entregar novas capacidades para os usuários, vamos analisar o layout dos recebíveis das vendas de boleto que mostrei acima, quantas novas capacidades você consegue enxergar nessa tela? Eu enxergo no mínimo 15:

* Ver o histórico de todos os repasses já feitos por data e valor líquido
* Ver o histórico dos repasses dentro de um espaço de tempo por data e valor líquido
* Ver o valor da taxa de repasse
* Entender o valor da taxa de repasse
* Ver o valor líquido do repasse
* Ver qual o status de um repasse
* Ver o total recebido de todos os boletos
* Ver a quantidade de boletos que foram pagos em todo o tempo
* Ver o total recebido dentro de um espaço de tempo
* Ver a quantidade de boletos que foram pagos dentro de um espaço de tempo
* Ver os detalhes de um determinado repasse
* Ver o quão longe está de acontecer o próximo repasse
* Ver qual é o valor do repasse mínimo
* Entender o que é o valor de repasse mínimo
* Solicitar um repasse antes de atingir o valor mínimo

A maior parte dessas novas capacidades tem um esforço mínimo para ser implementada, o que ajuda a diminuir muito o lead time. Vamos supor que já seja possível entregar o relatório só com a primeira capacidade e que faça sentido para o usuário (podemos estar em fase de testes ainda por exemplo) e o tempo para fazê-la seja de 3 dias, ao invés de esperar 1 mês para entregar tudo de uma vez, ótimo não? Já vamos aprender algo muito mais rápido.

# Quanto mais você se aprofunda, mais esforço consegue quebrar

Existe uma capacidade que pretendemos entregar para o usuário, que mesmo depois de quebrarmos a tela em 15 pedaços, ainda vai demandar um esforço muito grande:

* Ver qual o status de um repasse

Quando olhamos, parece uma simples chamada no banco de dados buscando pelo status do repasse. Acontece que quando você entende a estrutura que tem por trás, vai ver que não é tão simples assim. Para que esse status seja atualizado no banco de dados, vai ser preciso receber do banco (a instituição financeira) um arquivo de texto (sim acreditem, ainda é assim), interpretar esse arquivo que vem com todos os repasses de todos os clientes que tiverem mudança no status do repasse e aí alterar esse status no banco para que o relatório leia a informação no banco de dados.

Se, toda essa estrutura não estiver pronta, antes de dar essa nova capacidade para o usuário, vamos ter que construí-la para podermos usá-la, o que eu chamo de bloqueio tecnológico. Por vezes já vi começar a fazer uma história e ela ficar travada por conta de algum bloqueio tecnológico que não foi previsto e pior, ao encontrar um bloqueio, ele ser desenvolvido junto com a história. Resultado: lead time nas alturas!

Por isso, *quanto mais você se aprofundar e quanto mais cedo envolver os desenvolvedores na ideação da solução, mais cedo podemos entender os bloqueios tecnológicos e também ter noção do esforço que uma nova capacidade que queremos entregar irá ter. Fazendo isso metodicamente, conseguimos reduzir o lead time e o risco de desperdício e garantimos que vamos aprender e gerar valor mais rápido.*

Volto numa próxima oportunidade para falar de maneira prática, como reduzir incerteza das histórias. Até lá, compartilha com a gente outras técnicas para quebrar histórias que vem dando certo para vocês!

# Referências:

* [Better User Stories](https://www.betteruserstories.com/courses/better-user-stories/videos?video_id=1)
* [Método SPIDR](http://s3.amazonaws.com/betteruserstories/videos/bonus_downloads/000/000/014/original/spidr-poster.pdf?1524602363)