---
type: post
title: Quando a média não é um bom indicador de produto
excerpt: Enxergar o comportamento dos usuários pode não ser tão simples assim
authors: Arthur Martinho
date: 2021-10-25
image: https://i.imgur.com/9uDD9in.png
categories:
  - Indicadores e Dados
tags:
  - estatística
  - análise
  - dados
---
Imagina só comigo👇

Você é um PM em um app de streaming de música e chega de um stakeholder ou daquele HiPPO (Highest Paid Person’s Opinion) a ideia:

> Vamos usar a média de músicas ouvidas como indicador de performance do nosso produto.

Sempre que ouço alguma coisa assim eu já fico preocupado. Média costuma ser algo bem ilusório. 

# Agora contextualizando um pouco mais

Vamos continuar na ideia de que você é PM nesse contexto e essa aqui é sua base de usuários **ativos** e quantas músicas cada um ouviu nos **últimos 30 dias**

![](/images/posts/quando-a-media-nao-e-um-bom-indicador-de-produto-1.png "(Quem pegou a referência, pegou hehe)")

São 13 usuários, com um total de 4963 músicas ouvidas - seu indicador de performance, nesse cenário, será uma média de \~381 músicas por usuário.
Agora que você já tem a média, você deve analisar se a média é uma boa representação do comportamento dos usuários. Como primeiro passo pra isso, eu gosto de calcular o **Desvio Padrão**. 

# Desvio Padrão e Coeficiente de Variação

Beleza… Mas o que é Desvio Padrão? Nada mais é do que um valor que **indica a dispersão dos dados dentro da base analisada em relação à média**. 

Calcular a dispersão dos dados em uma base pequena costuma ser mais fácil, então pra facilitar vamos pra um cenário hipotético com apenas 3 usuários dessa nossa base:

![](/images/posts/quando-a-media-nao-e-um-bom-indicador-de-produto-2.png)

Repare que tem uma disparidade muito grande entre a quantidade de músicas ouvidas pra cada um desses usuários. A média nesse caso seria de **\~499**. Faz algum sentido olhar pra média nesse caso? 2 usuários estão **extremamente distantes** desse valor, o que já é 66% da base analisada.

Se a gente quiser entender, numericamente, qual é essa dispersão, a gente usa o desvio padrão (no google sheets é =stdev()) - que nesse nosso cenário reduzido é de **\~561**

Então beleza, juntado os dados nesse cenário reduzido temos:
* Média =~ 499
* Desvio Padrão =~ 561

Um jeito de interpretar esses dados é usando o **coeficiente de variação** - basicamente dividir o desvio padrão pela média. Na maioria das vezes, quanto menor o coeficiente, melhor - porque significa que a dispersão dos dados em relação à média é baixa.

Nesse nosso caso, o CV seria de (561/499) = 1,12.  E como analisar isso?

Normalmente eu trabalho com 3 cenários para análise desse coeficiente:
* CV ≤ 0,3 - cenário bom (baixa dispersão de dados)
* 0,3 < CV < 0,5 - cenário razoável (dispersão média de dados)
* CV ≥ 0,5 - cenário incerto (alta dispersão de dados) 

(Algumas outras referências consideram que somente a partir de 1,0 que o CV começa a ficar incerto demais, mas vamos nos ater à tabela anterior.)

Nosso CV de 1,12 fica no pior do cenários - ou seja - dados dispersos e bem distantes da média. 

Para esse cenário reduzido, faz sentido a gente olhar pra média? **Não**. Mas dessa vez não é só um “feeling” de que média não vai ser um bom indicador, mas sim descobrindo isso através de algumas ferramentas simples de estatística. 

# Voltando para o nosso cenário inicial

Beleza, agora expandindo pros nossos 13 usuários e com a média de \~381 músicas por usuário. 

Aplicando os conceitos ali de cima, temos a seguinte relação:

![](/images/posts/quando-a-media-nao-e-um-bom-indicador-de-produto-3.png)

Mais uma vez nosso CV dando acima 0,5 - mostrando um alto grau de dispersão entre os dados. 

Agora é a hora que você conversa com o seu stakeholder, mostra esses dados e explica que média não vai ser um bom indicador para seu produto. E aí podem vir duas perguntas que eu vou dividir em dois tópicos separados cada uma.

# Por que trabalhar em cima da média nesse cenário não ajuda muita coisa?

Acho que mais do que entender o que vale usar ao invés da média é entender **o que você quer medir**.

É moleza olhar pra um contexto e proferir: **vamos medir a média de uso da feature XPTO e usar isso como indicador de produto \o/**. 

No mundo ideal em que existe todo um playbook da estratégia, visão de produto bem definida, OKRs redondos, todos no time alinhados e KPIs rodando lisos, esse tipo de coisa não acontece, mas no mundo real é bem comum ver algumas disfunções nessas horas.

A pergunta **“o que queremos alcançar medindo o indicador XPTO?”**, pela minha experiência, é onde as respostas mais se enrolam - seja por não saber a resposta, seja pela resposta não condizer com a pergunta. 

Eu costumo dizer que antes de você chegar num indicador, tem bastante trabalho e um monte de pergunta que você precisa responder - no final, a parte mais fácil vai ser definir como medir. 

Vamos pegar esse exemplo da média. Imagina que o objetivo “subconsciente” desse indicador é auxiliar indicadores de **retenção ou engajamento**  dos usuários.  Será que não existem outros caminhos pra isso?

Aqui as coisas vão sempre variar de contexto pra contexto e seu trabalho vai ser sempre entender o que faz mais sentido - vamos supor que nesse contexto hipotético do app de música, seja possível ouvir músicas através de playlists ou álbuns. Alguns indicadores possíveis relacionadas ao engajamento são:
* % de usuários ativos que ouviram pelo menos uma música em uma playlist nos últimos 30d 
* % de usuários ativos que ouviram pelo menos uma música em um álbum nos últimos 30d

Agora que já temos alguns outros indicadores de engajamento nas features do app, como vamos trabalhar em cima deles? 

Vamos supor que você leu o artigo [Why Fixing Week One Retention Will Save Your Mobile App](https://apptimize.com/blog/2016/08/week-one-retention/) e que quer testar algumas hipóteses ou rodar experimentos em cima da sua jornada de primeira semana de uso para ver como isso impacta nas suas métricas de engajamento.

Daí começam a surgir análises. Depois de algumas conversas com o time de dados (ou você abriu o Mixpanel/Amplitude), você descobre que adicionar duas músicas em uma playlist na primeira semana pós signup retém 3x mais do que quem está fora desse recorte.

Surge, então, outro indicador:
* % de novos usuários que adicionaram pelo menos 2 músicas em uma playlist dentro da primeira semana nos últimos 30d

Reparou como a gente foi afunilando nossas possibilidades? Saímos de **média de músicas ouvidas nos últimos 30d > % de usuários ativos engajados nos últimos 30d  > % de novos usuários que adicionaram pelo menos 2 músicas em uma playlist dentro da primeira semana nos últimos 30d**.

O que você acha que vai ser mais acionável? Quais desses indicadores você vai conseguir ver o impacto do seu trabalho?

# Por último, quer dizer que a média não é um bom indicador? 

Claro que não.

Nesse caso em específico a gente trabalhava com uma base de **perfis de usuários muito diferentes** - em cenários maiores e mais complexos, podem haver partes do produto que usar a média faz todo sentido, enquanto outros não.

Imagina o cenário - você analisou a quantidade de bugs que chegam no suporte todo mês e chegou nessa planilha:

![](/images/posts/quando-a-media-nao-e-um-bom-indicador-de-produto-4.png)

E aí você resolveu fazer as contas e chegou nisso aqui:

![](/images/posts/quando-a-media-nao-e-um-bom-indicador-de-produto-5.png)

Claramente há um padrão na quantidade de bugs chegando por mês e a média representou isso muito bem com um coeficiente de variação bem baixo.

Talvez nesse cenário faça sentido ser um indicador de saúde do contexto.

Ainda há vários tipos de análises que podem ser feitas, como distribuição da severidade dos bugs por mês e outros fatores, é claro, mas de maneira genérica parece fazer sentido usar média de bugs por mês nesse cenário. 

Normalmente usamos a média para entender como o conjunto de dados analisado se comporta de maneira mais genérica. Usar **apenas** a média pode gerar um risco na análise devido a baixa robustez do indicador, principalmente por ser sensível a outliers.

# Gostou desse tipo de conteúdo?

Muito se fala sobre ser data driven e mais um monte de coisa, mas eu tenho a sensação de que o mercado ainda vem amadurecendo quanto a isso e nem sempre o cenário que encontramos nas empresas o é que vemos nas postagens do LinkedIn.

A ideia é trazer cada cada vez mais conteúdos sobre Product Analytics na prática e como aplicar no nosso dia a dia de produto. Você também é um entusiata dos dados? Me adiciona no Linkedin e vamos tomar um café virtual!

# Referências
* [Correlação estatística e causalidade em métricas de produto](https://productoversee.com/correlacao-estatistica-e-causalidade-em-metricas-de-produto/)