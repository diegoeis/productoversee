---
title: Duas métricas ágeis super importantes para PMs
excerpt: Um PM que entende bem o fluxo de desenvolvimento consegue se planejar melhor
authors: Pablo Silva
date: 2020-10-29
tags: [Agilidade]
categories: [Indicadores e Dados]
image: https://images.unsplash.com/photo-1536407078615-9fd99f2915c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80
featured_post: false
---

Duas métricas que os desenvolvedores mais usam para controlar o fluxo de
desenvolvimento, principalmente quando eles usam kanban, são Throughput
e Lead Time.

Throughput basicamente mede a quantidade de entregas num determinado
espaço de tempo. Geralmente se usa quantidade de itens entregues por
semana. A seguir exemplifico com um gráfico de throughput de um período
do ano passado de uma das equipes de desenvolvimento de produto da
Vindi.

Já o lead time é o tempo desde que se começou a despender esforço com um
item até o momento que ele foi considerado pronto. Digo o momento em que
se começou a gastar esforço, porque para algumas equipes esse momento
pode ser no refinamento e em outras pode ser no momento em que de fato
se começou a escrever código. Depende muito do que a equipe considera a
coluna de input. A seguir também exemplifico com um gráfico de lead time
de uma das equipes de desenvolvimento da Vindi no mesmo período do
gráfico de throughput.

Agora vocês devem estar se perguntando \"Mas Pablo, o que eu PM, tenho a
ver com esses gráficos? Eles não são sobre o fluxo de desenvolvimento?
Eu agora lá escrevo código para influenciar nessas métricas?\". Pois
bem, você como PM tem uma grande influência no fluxo de desenvolvimento
e consequentemente na saúde dessas e outras métricas.

Quando decidimos por implementar alguma hipótese que validamos, no geral
o que acontece é que escrevemos histórias de usuário e toda história
carrega um grau de incerteza e complexidade. Incerteza porque pode ser
algo totalmente novo ou o time ainda nunca mexeu nessa parte do sistema
por exemplo. Complexidade porque toda história tem um esforço para ser
desenvolvida, que pode ser desde muito grande até bem pequeno.

É exatamente por que as histórias sempre tem complexidade e incerteza
que fazemos refinamento com os desenvolvedores. Cada um dos requisitos
de negócio, vulgo critérios de aceite, que colocamos na história pode
torná-la mais complexa e mais incerta e com isso aumentamos o risco de
aumentar o lead time e diminuir o Throughput ou seja, a vazão do time.
Mas qual o problema disso? Quando o nosso Lead Time é muito alto ou o
nosso Throughput é baixo, é sinal de que estamos demorando muito para
colocar algo em produção e consequentemente estamos demorando muito para
aprender e gerar valor.

Se você analisar o gráfico de Lead Time acima, tivemos histórias ainda
abertas com um tempo de esforço já próximo de 50 dias. Imagina 50 dias
para aprender se o que você vai colocar em produção realmente vai
validar suas hipóteses. O mesmo comportamento pode ser encontrado no
gráfico de Throughput onde temos semanas sem entregas e consequentemente
semanas sem aprendizado. Esse tipo de comportamento é muito prejudicial
para o negócio, porque o mercado é muito acelerado e quanto mais
demoramos para impactar o usuário, menos chance temos de impactar o
negócio.

Toda vez que você identificar hiatos alguns gaps em um gráfico de
Throughput ou Lead Time, procure entender se não foi por que a história
ficou travada por alguma incerteza que passou despercebida ou se ela não
foi devidamente quebrada e a complexidade estava muito alta. Procure
garantir que nas próximas vezes o refinamento será mais efetivo. O
refinamento é um dos momentos mais críticos de um fluxo de
desenvolvimento de produto porque é nesse momento a maior chance de
garantir que o risco está baixo e que a história passará pelo fluxo de
desenvolvimento o mais \"suave\" possível. É responsabilidade do PM
garantir um refinamento quase perfeito.

E você, como estão seus refinamentos? Volto numa próxima letter (já eu
aqui conquistando o meu espaço nessa letter marota :D) para trazer dicas
básicas e avançadas para você arrebentar nessa cerimônia tão importante.


Referências:
-----------

-   [Requisitos em equipes ágeis: Falando sobre complexidade e
    incerteza](http://blog.plataformatec.com.br/2017/01/requisitos-em-equipes-ageis-falando-sobre-complexidade-e-incerteza/)

-   [Métricas Ágeis: Obtenha melhores resultados em sua
    equipe](https://www.casadocodigo.com.br/products/livro-metricas-ageis)

-   [Métricas Ágeis: Throughput e gráfico de
    Burnup](http://blog.plataformatec.com.br/2017/08/metricas-ageis-throughput-e-graficos-burnup/)