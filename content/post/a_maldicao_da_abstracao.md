+++
author = "Erick Pires"
comments = true
date = "2016-11-12T20:54:18-02:00"
draft = false
image = "images/a_maldicao_da_abstracao/cover.jpg"
menu = ""
share = true
slug = "a_maldicao_da_abstracao"
title = "A maldição da abstração"

+++

Obviamente eu escolhi o nome mais chamativo que consegui imaginar para esse post (ao melhor estilo Buzzfeed), mas um nome mais preciso seria "Produtividade vs Entendimento". Antes de falar sobre o motivo que me fez escrever esse texto, quero deixar claro essa relação entre abstração e produtividade, já que isso foi algo que eu levei um tempo para entender completamente.

Vou tomar como exemplo algo mais próximo de quem lida com computação, mas certamente o mesmo raciocínio se aplica a outras áreas. Quando alguém escreve um programa em assembly o programador tem um conhecimento enorme sobre o que o programa está fazendo, quais variáveis estão na memória e quais estão em registradores, quais registradores são usados para que, quais loops são desenrolados, quais funções sofrem inline, etc. Se o programador tivesse tempo infinito, ele poderia gerar o código de máquina mais otimizado possível para o seu programa (ok, alguém vai dizer que ele pode ficar preso em um mínimo local. Fine. Nesse caso ele chegaria muito próximo do código mais otimizado possível). É compreensível que alguns programadores não adotaram linguagens com um maior nível de abstração quando a transição para linguagens compiladas aconteceu, eles tinham muito mais controle sobre o programa em assembly. Mas nós não programamos em assembly hoje em dia. Nós criamos linguagens cada vez mais abstratas e o motivo disso, como sugerido antes, tem relação com a maior produtividade (ou seja, menor tempo para realizar um determinada tarefa) que essas linguagens proporcionam. Porém, nós abrimos mão de certa quantidade de controle para obter essa abstração, quanto menos o programador se preocupa sobre "detalhes" da implementação do programa, mais o compilador (ou interpretador, ou VM) tem que domar decisões por ele.

Bem, tudo que isso foi para dizer que embora abstração nos dê certa vantagem, abstração demais pode causar problemas. Como exemplo, vamos pensar na produção de um jogo. Muitas tarefas semelhantes (como atualizar o estado de todos os objetos, simular a "física" para todos os objetos, submeter dados para a GPU) precisam ser executadas durante um período de tempo razoavelmente curto (1/60 segundos) e em seguida o processo inteiro precisa ser refeito para preparar o próximo frame. Nesse cenário, é possível que um controle mais direto sobre, por exemplo, a alocação de memória seja necessário para garantir que os frames sejam gerados a tempo. Trabalhar com nível de abstração que não permita esse tipo de controle [insert Java hate comment here] provavelmente resultará em gambiarras pelo código e horas gastas tentando contornar essa limitação. Saber identificar o nível de abstração ideal para cada problema é uma habilidade que leva tempo para ser construída.

Agora vamos a algo que tem me incomodado faz um tempo. O aprendizado (e obviamente o ensino) de programação com pouca abstração tem deixado bastante a desejar. O problema mais imediatamente perceptível é que isso limita os tipos de problemas que alguém consegue resolver eficientemente. Eu não discordo da ideia de iniciar o aprendizado com certo nível de abstração, já que assim a taxa de crescimento da curva de aprendizagem se torna mais suave e é mais provável que quem está aprendendo continue motivado para aprender mais. Um ótimo exemplo disso é a plataforma do Arduino onde são abstraídas as etapas de acoplar ao microcontrolador um oscilador, um conversor serial-USB, entender uma IDE complicada, entender o que é ICSP, ligar um gravador e só então poder "ver" o código rodando. Além disso, as bibliotecas abstraem operações típicas de microcontroladores, como escrever em um registrador para ligar um Timer por exemplo. É interessante como o Arduino torna a programação de sistemas embutidos mais acessível para todo mundo. Mas eu vejo poucas tentativas de ensinar o lado mais low-level do funcionamento de um microcontrolador, e as que eu vejo tendem a criar uma dificuldade (ao meu ver) desnecessária. O mesmo pode ser dito sobre a forma que ponteiros são ensinados em um curso C, ou sobre um curso inteiro de programação em assembly.

Ok, talvez diminuir a abstração implique diretamente em uma maior dificuldade de aprender algo. Mas é possível que nós estejamos tentando ensinar de forma errada, e eu estou disposto a tentar responder essa questão. Mais precisamente, eu gostaria de ouvir as opiniões (e frustrações) de pessoas que notaram essa diferença brusca em dificuldade. Ideias sobre como deixar o aprendizado de conceitos low-level mais "suave" também são bem vindas. De qualquer forma, se você se interessar sobre o assunto por favor venha conversar comigo.

P.S.: Eu não deixei bem claro o motivo de uma curva de aprendizado "íngreme" me desagradar. Ao aprender algo com essa dificuldade é muito provável que quem está aprendendo deixe passar um conceito ou outro, simplesmente porque ele não consegue acompanhar a velocidade com que está sendo exposto a coisas novas. Com alguma probabilidade não nula esse conceito pode ser um "conceito chave" e nesse caso a pessoa termina com "buracos" no seu entendimento do assunto.

P.S.2: Eu não comentei sobre pessoas que só conseguem aprender em um estilo bottom-up, ou seja, de um estado de menor abstração em direção ao de maior abstração. O aprendizado para essas pessoas não precisa ser mais difícil do que o necessário.

P.S.3: Essa imagem
![ ](/images/a_maldicao_da_abstracao/say-low-level-one-more-goddamn-time.jpg)
