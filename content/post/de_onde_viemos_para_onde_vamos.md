+++
author = "Erick Pires"
date = "2017-01-07T18:32:46-02:00"
menu = ""
slug = "de_onde_viemos_para_onde_vamos"
comments = true
image = ""
share = true
title = "De onde viemos? Para onde vamos?"
draft = true

+++

Ano passado eu estava fazendo a prova PosCOMP e uma das perguntas pedia a distinção entre [Máquinas de Moore e Máquinas de Mealy][1]. Eu lembrava de ter esse conhecimento em algum momento do passado (na verdade eu lembrava até da forma como o professor pronunciava Moore e Mealy), mas eu não lembrava o que a questão pedia. No momento eu resolvi seguir o fio de lembrança que apareceu na minha mente e ver onde ele me levava. Não quero enrolar demais falando sobre esse asunto, então vou pular alguns detalhes. Essas máquinas são na verdade implementações de Autômatos de Estado Finitos e deveriam ter sido ensinados na disciplina de Linguagens Formais (inclusive a questão era focada nesse aspecto das máquinas), mas como nem tudo é perfeito eu aprendi sobre elas na disciplina de Circuitos Lógicos (que está antes no currículo e por isso eu não sabia Linguagens Formais na época). Mas por qual motivo isso foi ensinado em Circuitos Lógicos? Bem, acontece que Moore e Mealy são exemplos clássicos de [Circuitos Lógicos Sequenciais][2] (e esse tipo de circuito é ensinado para apresentar as [Sandálias][3]. Piada sem graça, DONE).

Ok, mas por que estamos falando de flip-flops? Por dois motivos, o primeiro é que eu estou com vontade de escrever e por isso resolvi enrolar um pouco nesse texto. O segundo é porque há uma pequena relação entre Lógica Sequencial e o assunto sobre o qual eu quero falar. Uma das formas mais simples de explicar o que é Lógica Sequencial (e que na verdade não explica nem um pouco o que realmente está acontecendo) é como um circuito que "lembra" tudo o que aconteceu com ele no passado, ou de uma maneira mais formal é um circuito cujo estado atual depende dos estados anteriores. Algo que deve passar pela mente de todo estudante curioso (pelo menos passou pela minha) é que o estado inicial (o primeiro de todos) vai ter influência sobre todo o futuro do circuito.


[1]: https://www.tutorialspoint.com/automata_theory/moore_and_mealy_machines.htm
[2]: https://en.wikipedia.org/wiki/Sequential_logic
[3]: https://en.wikipedia.org/wiki/Flip-flop_(electronics)
