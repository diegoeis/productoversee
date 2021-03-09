---
type: post
title: Conhecendo o débito técnico no desenvolvimento de produtos
excerpt: " O resultado de correções rápidas e momentâneas, sem considerar o
  longo prazo, impactam diretamente o custo e risco do negócio"
authors: Newton Calegari
date: 2021-03-24
publishDate: 2021-03-24
image: https://i.imgur.com/hBISm0d.jpg
categories:
  - Tático
tags:
  - desenvolvimento
  - tecnologia
  - fluxo
---
O débito técnico no desenvolvimento de produtos acontece quando tomamos decisões priorizando a velocidade da implementação em detrimento de escolhas arquiteturais que resolvam o problema por completo. Geralmente é resultado da implementação de correções rápidas e momentâneas, sem considerar uma solução mais adequada para o longo prazo.

O débito técnico possui dois fatores que impactam diretamente o negócio: custo e risco.

* Em termos de custo, qual é o custo para a organização ao manter o débito técnico?
* Quanto ao risco, quais são as chances de que esse débito técnico atual se transforme em um problema maior no futuro, exigindo maior atenção e esforço para resolvê-lo?

Um componente de um produto que possui débito técnico pode trazer complexidade extra, dificultando, assim, sua manutenção ou melhoria.

O conceito de débito técnico apareceu pela primeira vez em um [artigo publicado em 1992](https://productoversee.createsend1.com/t/t-l-myhhllt-l-j/) por Ward Cunningham na conferência OOPSLA'92 sobre engenharia de software.

Neste paper Cunningham escreveu a respeito de um sistema chamado WyCash, utilizado para gerenciamento de portfólios de investimento. O que talvez tenha facilitado a construção da metáfora com o débito financeiro.

Assim como em um empréstimo nós precisamos pagar juros sobre o principal, quando optamos por uma solução rápida ou temporária a nível de software, nós também pagamos juros sobre essa decisão.

Em 2003, pouco mais de uma década após o paper de Cunningham, Martin Fowler, referência na área de engenharia de software, [descreveu débito](https://productoversee.createsend1.com/t/t-l-myhhllt-l-t/) da seguinte maneira:

Doing things the quick and dirty way sets us up with a technical debt, which is similar to a financial debt. Like a financial debt, the technical debt incurs interest payments, which come in the form of the extra effort that we have to do in future development because of the quick and dirty design choice

Em uma adaptação livre para português, seria algo como:

Fazer coisas de maneira "rápida e suja" vai gerar débito técnico, que é similar ao débito financeiro. Do mesmo modo que um débito financeiro, o débito técnico está sujeito ao pagamento de juros, que vem na forma de esforço extra que nós temos que fazer no futuro por causa de uma decisão arquitetural "rápida e suja".

Fowler ainda provoca dizendo que podemos escolher entre continuar pagando esses juros ou pagar todo o valor por meio da [refatoração](https://productoversee.createsend1.com/t/t-l-myhhllt-l-i/) do componente que causou débito técnico.

## O impacto do débito técnico

Nosso papel como gerentes de produtos é identificar maneiras de adicionar ou ampliar o valor dos nossos produtos.

A sugestão de refatoração, apesar de contribuir para pagar o débito técnico, pode não se encaixar no nosso fluxo de desenvolvimento de produtos pois as atividades de revisão e reescrita de código dificilmente propõem novo valor imediato para os usuários. Essas atividades são encaradas como pagamentos de juros de uma dívida iniciada a partir de uma escolha arquitetural que se mostrou inadequada.

É neste momento que começa a surgir um conflito no processo de gerenciamento de produtos: se por um lado contrair dívidas técnicas trará melhorias rápidas e valor imediato para os usuários; por outro lado, esse débito pode crescer e dificultar a implementação de melhorias no futuro.

Nós, como gerentes de produtos, devemos avaliar o [trade-off](https://productoversee.createsend1.com/t/t-l-myhhllt-l-d/) entre o valor presente e o futuro.

Introduzir muito débito técnico, com o objetivo de priorizar funcionalidades que tragam valor imediato, traz um risco que pode vir a comprometer a viabilidade do produto a longo prazo, tornando-o um artefato cada vez mais complexo e exigindo esforços ainda maiores para refatoração.

Em contrapartida, focar em manter a qualidade do software impecável pode postergar a entrega de valor de um produto e comprometer sua sobrevivência no mercado em que está inserido.

Não são decisões simples, tampouco fáceis de serem tomadas.

É comum empresas contraírem dívidas financeiras para viabilizar a execução de projetos buscando um retorno ([ROI](https://productoversee.createsend1.com/t/t-l-myhhllt-l-h/)) positivo no futuro. Da mesma forma, é normal aceitarmos débito técnico, desde que mantido sob controle.

É um risco que faz parte do jogo.

## A visibilidade do débito técnico

Por ser naturalmente um assunto mais próximo dos times de engenharia, o conhecimento e controle sobre débito técnico acontece localmente, a nível de time.

O que facilita sua percepção em ambientes mais próximos da execução e mais distantes do nível estratégico, tornando-o invisível para organização e acarretando em dificuldades para conquistar buy-in de stakeholders importantes para o pagamento dessa dívida.

Sabendo que o débito técnico pode impactar negativamente o negócio no longo prazo, cabe à pessoa no papel de gerente de produtos traduzir de maneira acessível este assunto para as pessoas que estão no nível de negócio.

## Lidando com débito técnico no dia a dia

Saber o que impactará a curto, médio e a longo prazo faz diferença na priorização e gerenciamento da evolução do produto.

Não podemos nos isentar da responsabilidade pelo surgimento de débito técnico nos nossos produtos. Geralmente surge como resultado da priorização de uma solução imediata, em alguns casos paliativa, em detrimento de uma solução que melhor atende aos [requisitos não funcionais](https://productoversee.createsend1.com/t/t-l-myhhllt-l-k/) ou arquiteturais do software.

O aparecimento de débito técnico é inevitável justamente por resultar do trade-off entre o curto e o longo prazo. Contudo, quanto maior o nível de incerteza em relação a uma funcionalidade, maiores podem ser os juros sobre a dívida técnica a serem pagos no futuro.

O primeiro passo é saber da possível existência de débito técnico, isso permitirá que o time tenha consciência de que algumas implementações poderão contribuir para essa dívida.

Para ter dimensão do débito técnico podemos adotar uma estratégia simples: a identificação de itens do backlog que podem gerar débito técnico. Por meio da utilização de uma tag ou alguma outra marcação podemos identificar aquele item como resultado ou causa de débito técnico.

Esta marcação explícita nos permite buscar facilmente itens que podem ser otimizados e melhorados a fim de pagar, aos poucos, parcelas da dívida técnica.

Sabemos que o débito aparecerá até mesmo nos melhores times, então para trazer entender o que possivelmente originou esse débito, nós podemos utilizar a [matriz](https://productoversee.createsend1.com/t/t-l-myhhllt-l-u/) de [débitos técnicos](https://productoversee.createsend1.com/t/t-l-myhhllt-l-o/), dividida em 4 quadrantes que podem dar pistas sobre a origem do débito técnico: imprudente ou prudente, e deliberado ou inadvertido. ​

![Matriz do Débito técnico formato pelos quadrantes de imprudente, prudente, deliberado e inadvertido.](https://i2.createsend1.com/ei/t/89/836/A75/121706/csfinal/ScreenShot2021-02-22at22.03.291-9900000000079e3c.png)

Além destas abordagens, existem outras que podem se adequar mais à cultura do time. Neste artigo sobre [débito técnico e urgências futuras](https://productoversee.createsend1.com/t/t-l-myhhllt-l-b/) Pablo Silva apresenta outras estratégias de "pagamento" para evitar que a dívida fique muito cara.

Não somente o entendimento do estado atual do nível de débito técnico é importante, mas também saber o que fará com que essa dívida cresça. Por isso, em equipes com níveis diversos, pessoas mais experientes devem ajudar o restante do time a avaliar o impacto de determinada solução e se tal solução adotada implicará no crescimento da dívida.

Novamente, nós como gerentes de produtos, devemos considerar o débito técnico como um dos fatores que influenciam na decisão de priorizar uma nova implementação ou release. Do ponto de vista estratégico, é importante que não priorizemos uma funcionalidade a todo custo, ou seja, decidir sem avaliar minimamente o impacto e os "juros" consequentes dessa decisão.

É normal que uma escolha por uma solução rápida seja a única a possível para o momento, já que uma opção mais completa poderia comprometer o tempo para entrega de valor do produto. Por isso é fundamental que saibamos balancear o montante de débito técnico e não somente evitá-lo a todo custo.

## Referências:

* [https://speakerdeck.com/labcodes/debito-tecnico-porque-isso-vai-estragar-teu-software?slide=25](https://productoversee.createsend1.com/t/t-l-myhhllt-l-p/)
* [Débito técnico em uma startup: quando, como e por que?](https://productoversee.createsend1.com/t/t-l-myhhllt-l-x/)