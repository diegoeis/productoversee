---
title: "Comentário: Design System e o gap de comunicação entre Designers e Devs"
type: post
date: 2019-05-31
image: https://i.imgur.com/slk72ip.jpg
tags:
  - desenvolvimento web
  - carreira
  - design
---

Essa foi uma [série de tweets](https://twitter.com/diegoeis/status/1134339782149058560) que fiz outro dia. No final, tem o link da thread. Seguem as anotações:

----

Vocês já pararam para pensar que o design system é uma espécie de expressão de como havia (e ainda há) um buraco de comunicação e relacionamento entre devs e Designers?

Durante anos os devs implementam e criam, do início ao fim, design systems a partir dos layouts entregues pelos designers. Esses "design systems" entregues pelos Devs tem diversas profundidades: vão desde simples UI Kits, com elementos em HTML e CSS, passando por bibliotecas de componentes com comportamentos simples em JS até frameworks maiores.

Os devs faziam isso para faciltiar o seu próprio trabalho, e no processo até corrigiam problemas que aconteciam como a falta de padronização de cores (qual dev nunca reclamou de ter 5 padrões de cinzas? ou de margens diferentes em um mesmo elemento?). Frameworks e bibliotecas como Bootstrap e outros, surgem com essa necessidade de facilitar a padronização visual e técnica dos elementos da tela pra dar mais velocidade e consistência na construção de interfaces.

Estou dando o nome de design system, para aquela "organização" que designers fazem para alcançar a padronização, modularização e continuidade da interface.

O designer fazia o layout, o dev implementava esse layout e nesse processo de implementação, o dev modularizando tudo o que podia e isso é muito bom. Contudo, devs não levavam em consideração critérios de design, e muitas vezes se focando apenas nas necessidades técnicas afim de facilitar a manutenção e longevidade de código.

O problema da construção de interfaces sempre foi a componentização. A partir do momento que os devs perceberam isso, soluções como Web Components e ReactJS ajudaram muito nessa tarefa de montar uma interface usando módulos.

E nesse processo, o designer apenas se importava com o design da interface de forma “global”, digamos assim... os devs, por si só, quebravam a interface em pequenos pedaços de elementos funcionais, de fácil implementação e manutenção.

Não envolvendo os Designers, o resultando a médio e longo prazo era sempre a inconsistência de uso e principalmente do visual da interface durante todo o percurso do usuário no produto.

Todo mundo já viu essa briga velada acontecer. E ela acontece o tempo inteiro. Sites com vários estilo de botões, com medidas, distâncias e estruturas não padronizadas... uma interface inconsistente, não preparada para os cenários que o negócio pode ter e o usuário exigir.

Devo dizer que todo o conhecimento adquirido pelos devs sobre modularização de interfaces, está sendo conhecida pelos Designers apenas agora. O Design System, é um nome bonito para algo que os devs já fazem há anos. Alguns fazem muito melhor que Designers, inclusive.

Da mesma forma que alguns Designers já eram conscientes desse gap desde o início e era o que separava os bons Designers dos grandes Designers de interface para web.

Mas pra ter um design system decente, não se pensa apenas em componentes, que era o que a maioria dos devs (e não aqueles alguns citados acima) faziam. Se pensar apenas nos componentes por si só, o Design System vira uma simples biblioteca de elementos.

É no design system que os devs e Designers devem complementar suas especialidades: o designer entende como a interface pode variar e cria uma linguagem visual que se adequa a todos os cenários de comportamento. O dev, por sua vez, implementa isso de forma consistente e flexível.

<blockquote class="twitter-tweet"><p lang="pt" dir="ltr">Vocês já pararam para pensar que o design system é expressão de como havia (e ainda há) um buraco de comunicação entre devs e Designers?</p>&mdash; Diego Eis (@diegoeis) <a href="https://twitter.com/diegoeis/status/1134339782149058560?ref_src=twsrc%5Etfw">May 31, 2019</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>