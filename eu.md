A mandala e eu

Quando comecei a pintar as mandalas percebi que aquilo estava me fazendo muito bem.

Após algumas mandalas pintadas já estava feliz e orgulhoso da melhoria da qualidade de meu traço assim como com a melhor escolha das cores.

Percebi que além de escolher e intercalar as cores, e de pintar a mandala em si, também estava organizando o meu cérebro e pensando em várias e diversas coisas.

Consegui entender que a mandala era uma ferramenta que poderia me ajudar a organizar o meu pensamento.

Já rabiscava várias vezes fazendo desenhos ou mapas mentais sobre a minha vida, meus objetivos, meus problemas e metas para o futuro, porém nunca havia pensado que poderia fazer o mesmo sem falar nada e nem mesmo escrever uma palavra. Apenas pintando. Um processo hipnotizador.

Assim que me apossei da técnica, comecei a aproveitar aqueles momentos de alta concentração na pintura das mandalas e também comecei a explorar minha mente, organizar ideias e também pensar sobre minhas atitudes.

Esse encontro comigo mesmo ganhou frequência, cheguei a pintar 3 mandalas na sequência. Também observei que conforme os dias foram passando, tive mais vontade de pintar. Associei o próprio alívio imediato com a pintura das mandalas. Uma forma de fugir do mundo real para dentro mim mesmo.

Outro fato muito interessante foi a apreciacão das minhas mandalas e a conexão dos momentos específicos em que pintei com a mandala. Teve alguns casos que pintei enquanto sentia dores, e sei exatamente quais mandalas foram neses momentos. Existem mandalas que foram feitos em momentos de:

* raiva
* confusão mental
* tristeza


Consegui ter uma boa lembrança do momento mental conectado a mandala. Também acredito que o fato de ter percebido isso criou uma relevância bem maior nos meus sentidos neste aspecto.

Existiu algumas mandalas que eu realmente não gostei do que pintei. Porém em nenhum momento julguei elas ou mesmo decidi jogar fora. Comecei até mesmo a ve-las como uma espécie de "fotografia das emoções".

A mandala em sua composição de modelos geométricos me levou ao estudo da geometria sacra. Este me trouxe a compreensão de uma série de outros fatores universais que estão intrínsecos na vida e também são manifestados através das mandalas.

* The flower of life ( A flor da vida)
* Golden ratio (Razão áurea)
* Fibonacci
* Pi
* 4 elements
* 4 cycles between the elements

Também me levou a uma série de estudos sobre a matemática geométrica, poliedros perfeitos e também a profunda admiração por Pitágoras que a muito tempo atrás desenvolveu uma série de fórmulas legais e úteis na composição e decomposição das mandalas.

Outra feliz consequência foi o estudo das cores das mandalas associadas às notas musicais. Mais uma vez Pitágoras foi o primeiro homem a documentar e especificar isso na história. Porém depois dele mais outros 23 matemáticos que também criaram suas teorias. Acabei utilizando a teoria mais recente criada por Joshton (2003).

Além disso também desenvolvi alguns protótipos extraindo informações da mandala e apresentando em outros aspectos. Os mais interessantes foram:

## Leitura aspiral e transposição musical

Um dos primeiros desafios em extrair a música foi saber que não geraria harmonia inicialmente, mas sempre rola uma expectativa de que a mágica das cores iriam fazer o trabalho. Realmente aconteceu em apenas uma mandala, gerou um acorde harmônico contínuo e uniforme com as fórmulas básicas.

Isso foi realmente animador e então após umas boas horas escutando as primeiras composições aleatórias estava quase louco com aquele som sem sentido. Decidi que o caminho para poder tocar algo interessante era estudar sobre pelo menos um pouco de harmonia e tentar entender como poderia gerar harmonia e não apenas notas no ar.

A primeira transposição de cores foi apenas baseada em tons de grave para agudo conforme o brilho da cor (nota = r + g + b). O exemplo não foi muito bem sucedido em termos de sonoridade mas abriram a oportunidade para criação de rítmos a partir de médias de cores para médias de tons.

A leitura circular foi inspirada no toca-disco e também num outro projeto que vi que fazia uma leitura de uma fatia de madeira. Utilizei o tradicional "grand piano" MIDI para fazer os testes iniciais como neste projeto da madeira, mas optei pela leitura e interpretação digital e também fiz um algorítmo para pintar a mandala enquanto executava a leitura na mesma posição em que estava tocando naquele momento.

Fiquei feliz com a primeira versão porém decidi que iria me concentrar em aprender exatamente como construir harmonia então as cores apenas guiariam a harmonia ao invés de ditar as notas.



## Paleta de cores da mandala

O pensamento de programador sempre predominante e tentando criar regras, médias e fórmulas para as coisas, pensei em identificar as cores mais interessantes da mandala.

Quais as cores que mais foram pintadas e quais as cores ficam mais legais em conjunto. Dessa forma criei uma visualização de uma paleta com as 12 cores mais utilizadas em cada imagem.

Usei uma biblioteca chamada ColorThief para fazer o trabalho. Algo tão simples quanto:

    new ColorThief(mandala).getColorPallete(12);

Após fazer a paleta de cores aparecer no meu iPad, deixei a paleta na parte inferior da tela e pareceu muito com um piano. Então pensei "por que não?" e implementei o desafio. Da mesma forma que li as propriedades rgb de forma circular, agora apenas precisava conectar a cor da paleta de cores a nota.

Foi muito legal e fácil de implementar a conexão visual apenas tive um grante constrangimento com a incompatibilidade das bibliotecas multitouch e minhas tentativas de usar os eventos touch nativos do sistema operacional em modo multitouch. Não obtive muito sucesso na primeira versão e ficou meio estranho sem multitouch porém deu para testar o conceito com o próprio click no mouse.

Outro ponto que surgiu a partir daí foi a compatibilidade de bibliotecas de som com os dispositivos móveis. Estive alinhando alguns detalhes mas não obtive muito sucesso no uso dessas ferramentas para dispositivos no android e também no iOS. O som não ficou sintetizado com alta qualidade, não ficou tão bom quanto no computador. Esse é um tipo de frustração extremamente comum no ambiente de desenvolvimento de software: incompatibilidade entre dispositivos. Ou por falta de memória, ou por arquitetura de processamento ou falta de desempenho para execução em tempo hábil. Tudo coopera para não funcionar bem em todos os ambientes.

Como programador é um desafio deixar esses aspectos funcionais em todos tipos de computadores e telas e navegadores e versões específicas de cada um desses itens porém é frustrante não conseguir manter algo funcional para maioria deles.

Sempre opto por trabalhar em um modelo que não posso desanimar. Quando começo a trabalhar apenas em incompatibilidades o trabalho se torna desanimante e logo improdutivo. Estou tentando usar o máximo possível de padrões e bibliotecas que abstraiam estes tipos de inconveniências entre navegadores porém mesmo assim acabo passando horas e horas tentando compatibilizar e manter funcionando em várias plataformas. 

Por isso estou usando o Apache Cordova deste o início deste projeto. Para manter o aplicativo híbrido: instalado no celular rodando localmente ou rodando na web, ou rodando na web do próprio celular idênticamente ao instalado.


## Conversão das cores para as notas




# A experiência de ser pai


