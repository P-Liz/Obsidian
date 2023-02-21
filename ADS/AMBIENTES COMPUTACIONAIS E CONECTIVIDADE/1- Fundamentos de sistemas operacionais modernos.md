
[https://canaltech.com.br/software/qual-e-o-sistema-operacional-mais-usado-do-mundo-223507/](https://canaltech.com.br/software/qual-e-o-sistema-operacional-mais-usado-do-mundo-223507/)
#### Definição de sistema operacional

Travamentos, tela preta e shutdown são uma forma de o sistema operacional proteger a máquina de danos permanentes que possam ser causados por processos.

<mark style="background: #ABF7F7A6;">Definição: Programas implementados como software ou firmware, que tornam o hardware utilizável.</mark>

---

##### Firmware

Firmwares são programas armazenados de forma permanente no hardware que permitem o funcionamento e a realização de operações básicas em certos dispositivos da máquina. 

   Ex.: Circuitos integrados de memória, unidades de disco e processador.

Geralmente vem guardados em circuitos de memória não volátil (chips de memória ROM), contendo os programas em linguagem de máquina com o objetivo de executar operações especiais como a auto verificação do sistema, POST ou power on self teste e a carga do sistema operacional a partir de um dispositivo adequado, ou bootstrap.

<center>Hardware > Firmware > OS > Aplicativos</center>

---

- Arquiteturas internas diferentes utilizam diferentes processadores, e por sua vez, diferentes linguagens de máquina.

- Necessidade de camada intermediária entre o Hardware e Programas de aplicação, oferecendo ambiente de programação mais simples.

<center>Hardware  - Programas de abstração de linguagem de máquina - Aplicações</center>


- O comportamento do sistema operacional é como uma extensão do próprio _hardware_, ou como uma máquina virtual, que possui características diferentes da máquina física real.


---

Um sistema operacional deve atender a três princípios básicos:

1. Recursos do Sistema: Oferecer os recursos do sistema de forma simples e transparente para o usuário;
2. Gerenciamento dos recursos existentes: Gerenciar a utilização dos recursos existentes, buscando seu uso eficiente em termos de sistema;
3. Integridade e a segurança dos dados: Garantir a integridade e a segurança dos dados armazenados e processados no sistema, bem como de seus recursos físicos.

<center>Além de atender a estes princípios, um sistema operacional deve proporcionar uma interface para que ele possa ser utilizado por seus usuários.</center>

---

#### Arquitetura de um computador

A arquitetura de um computador é composta de três sistemas:

1. **Unidade de Processamento Central**

Unidade de Processamento Central (CPU) é a composição de registradores, Unidade de Controle (UC), Unidade Lógica Aritmética (ULA) e contador de programa.

-   **Registradores**: são memórias temporárias que existem dentro da CPU de altíssima velocidade;
-   **Unidade de Controle (UC)**: é responsável por buscar as instruções na memória principal e classificar o seu tipo;
-   **Unidade Lógica Aritmética (ULA)**: é responsável por fazer as operações booleanas e aritméticas;
-   **Contador de programa (PC)**: é responsável por avisar à UC qual será a próxima instrução a ser buscada e executada.

2. **Sistema de memória principal**

Sistema de memória principal é a unidade que armazena os dados e os códigos do programa.

4. **Sistema de entrada e saída**

Sistema de entrada e saída é a unidade responsável por pegar os dados de entradas e mostrar os resultados de saída do programa.  Ciclo dessa execução compreende:

1.  O contador de programa é utilizado pela UC para determinar qual e onde está a próxima instrução;
2.  A UC busca a instrução do programa na memória principal;
3.  A decodificação da instrução será feita para uma linguagem que a ULA possa interpretar;
4.  Os dados requeridos são transferidos da memória e alocados nos registradores da CPU;
5.  A ULA executa a instrução e coloca os resultados na memória ou nos próprios registradores.


#### Gargalo de Von Neumann

É o atrofiamento que está no canal de transmissão entre a CPU e a memória, pois essa não consegue trabalhar em frequências tão altas quanto a CPU, que fica ociosa por um certo tempo.

![[Pasted image 20230214213452.png]]

---

Leituras Complementares: 

- Página 13 do livro 'Sistemas operacionais' - Aborda a importância da computação paralela e distribuída, como forma de melhoria a recursos escassos de computação nos dispositivos móveis, bem como o papel que a ascensão dos middlewares desempenhou para possibilitar isso.

- Página 415 à 417 do livro 'Sistemas operacionais modernos' - Aborda a segurança dos OS's e   pequenas brechas de segurança além de ataques sofisticados. Divide os ataques em ativo e passivo. Demonstra as diferenças entre criptografia e endurecimento de segurança dos softwares. 
  Pontua que os OS's podem ser seguros, porém não são comercializáveis se assim o forem, pois devem ser mantidos simples e sem muitas funcionalidades. Complexidade é sinônimo de mais código com defeitos, erros e inseguro. Sistemas confiáveis possuem exigências de segurança declaradas e uma TBC (Trusted Computing Base) mínima, com apenas o hardware e software necessários para valer o sistema de segurança. Se a base de segurança estiver conforme, esta não pode ser comprometida, não importa o que mais esteja errado. 
  A TCB é composta de hardware e da maioria dos programas sudo, sendo o monitor de referência uma parte importante, pois centraliza todas as requests de segurança, o que não ocorre em OS's usuais. Metas de segurança atuais buscam reduzir os OS's a uma base computacional confiável, oferecendo maior segurança. Um modelo claro do que deve ser protegido e das permissões de uso é uma das formas para aumentar a segurança.
  
- Entrevista 'O egoísmo e o Linux', com Linus Torvalds - Sinceramente, tenho motivos bastante egoístas; isso vale para todo mundo e é o que explica o sucesso do Linux. As empresas que atuam no projeto também não são movidas por razões altruístas —elas querem obter algo com isso. O código-fonte aberto é uma ótima ocasião para reunir interesses diversos, aproveitando as motivações individuais de cada colaborador. O Linux nasceu de um conjunto de erros. “Eu via mais exemplos do que não fazer do que modelos a seguir”. A auto-organização tende a acontecer em vez de ser conduzida intencionalmente. Muitos objetivos individuais egoístas podem nem parecer tão egoístas assim vistos no conjunto; as pessoas e as comunidades agem de maneira altruísta, mesmo quando movidas por razões egoístas.

---

### Tipos de sistemas operacionais

Os sistemas operacionais podem ser classificados de acordo com diversos parâmetros e perspectivas, como, por exemplo, tamanho, velocidade, suporte a recursos específicos, acesso à rede etc. Muitos sistemas operacionais se encaixam bem em mais de uma das categorias de classificação.

<u>Batch</u>

Os sistemas operacionais Batch (de lote) mais antigos trabalhavam “por lote”, ou seja, todos os programas a serem executados eram colocados em uma fila, com seus dados e demais informações para a execução. O processador recebia os programas e os processava sem interagir com os usuários, o que permitia um alto grau de utilização do sistema.

![[Pasted image 20230217234016.png]]

<u>De rede</u>

Um sistema operacional de rede precisa ter suporte à operação dos dispositivos em rede, ou seja, a capacidade de oferecer às aplicações locais os recursos que estejam localizados em outros computadores pertencentes à rede, como arquivos e impressoras. Ele deve disponibilizar seus recursos locais aos demais computadores de forma controlada. A maioria dos sistemas operacionais atuais oferece essa funcionalidade.

<u>Distribuído</u>

Em um sistema operacional distribuído, os recursos de cada máquina estão disponíveis de forma transparente aos usuários. Ao lançar uma aplicação, o usuário interage com sua janela, mas não sabe onde ela está executando ou armazenando seus arquivos: é o sistema que decide, de modo transparente. Esses sistemas já existem há muito tempo, segundo Tanenbaum (1995) e Dasgupta _et al_. (1991), mas ainda não são uma realidade por completo no mercado.

**São alguns exemplos de **sistemas distribuídos**:**

-   A internet é o maior exemplo de **sistema** distribuído.
-   Qualquer aplicação intranet.
-   Qualquer aplicação mobile.
-   Aplicações e serviços baseados na Computação em Nuvem.

**<u>Multiusuário</u>

Um sistema operacional multiusuário deve suportar a identificação do “dono” de cada recurso dentro dele (arquivos, processos, áreas de memória, conexões de rede) e impor regras de controle de acesso para impedir o uso desses recursos por usuários não autorizados. Essa funcionalidade é fundamental para a segurança dos sistemas operacionais de rede e distribuídos. Grande parte dos sistemas atuais é multiusuário.

<u>Desktop</u>

Um sistema operacional _Desktop_ “de mesa” é voltado ao atendimento do usuário doméstico e corporativo, para a realização de atividades corriqueiras, como edição de textos e gráficos, navegação na internet e reprodução de mídias simples. Suas principais características são a interface gráfica, o suporte à interatividade e a operação em rede. Seus exemplos são os vários sistemas Windows (XP, Vista, 7, 8 e 10), o MacOS X e o Linux.

<u>Servidor</u>

Um sistema operacional servidor deve permitir o gerenciamento eficiente de grandes quantidades de recursos (disco, memória, processadores), impondo prioridades e limites ao uso dos recursos pelos usuários e seus aplicativos. Em geral, ele tem suporte à rede e multiusuários.

<u>Embarcado</u>

Um sistema operacional é embarcado (embutido ou _embedded_) quando for construído para operar sobre um _hardware_ com poucos recursos de processamento, armazenamento e energia. Aplicações típicas dele aparecem em telefones celulares, sistemas de automação industrial e controladores automotivos, equipamentos eletrônicos de uso doméstico (leitores de DVD, TVs, fornos micro-ondas, centrais de alarme etc.).

<u>Tempo real</u>

Um sistema operacional de tempo real não precisa ser necessariamente ultrarrápido. Sua característica essencial é ter um comportamento temporal previsível (ou seja, seu tempo de resposta deve ser conhecido no melhor e pior caso de operação). Sua estrutura interna deve ser construída de forma a minimizar esperas e latências imprevisíveis, como tempos de acesso ao disco e sincronizações excessivas. Existem duas classificações: _soft real time systems_, nos quais a perda de prazos implica a degradação do serviço prestado, um exemplo é o suporte à gravação de CDs ou reprodução de músicas. Caso o sistema se atrase, podem ocorrer a perda da mídia em gravação ou falhas na música que está sendo tocada.; e _hard real time systems_, em que a perda de prazos pelo sistema pode perturbar o objeto controlado, com graves consequências humanas, econômicas ou ambientais. Um exemplo é o controle de funcionamento de uma turbina de avião a jato ou de uma caldeira industrial. Exemplos de sistemas de tempo real incluem QNX, RT-Linux e VxWorks. Muitos sistemas embarcados têm características de tempo real, e vice-versa.

---

#### **Sincronização e comunicação de processos**

Em 1960 surgiu a programação concorrente, que tem como base a execução, de forma colaborativa, de múltiplos processos ou threads que trabalham na mesma tarefa.

Com **apenas um processador**, os processos se alternam no uso do processador e demais recursos, de acordo com os critérios de escalonamento de processos, que são estabelecidos pelo sistema operacional.

Com **múltiplos processadores**, o paralelismo amplia as vantagens que a programação concorrente proporciona, com várias tarefas sendo executadas em paralelo – cada tarefa em um processador diferente, normalmente.

É comum que os processos de uma aplicação concorrente compartilhem recursos. Entretanto, esse compartilhamento gera problemas que podem comprometer a execução da aplicação. Por isso, é necessário que os processos da aplicação concorrente sejam sincronizados pelo sistema operacional, com o objetivo de garantir o processamento correto dos programas. Se não tivermos um gerenciamento no uso concorrente dos recursos compartilhados, podem ocorrer inconsistências nos dados. Devendo ocorrer comunicação entre os processos, conforme abaixo.

##### **Comunicação por compartilhamento de memória**

*O compartilhamento de memória é um mecanismo de comunicação entre processos, que usa uma área da memória, um **buffer** compartilhado entre os vários processos de uma aplicação concorrente.*

Em **operações de escrita**, um processo só poderá gravar dados no _buffer_ caso esse não esteja cheio. Já em **operações de leitura**, um processo somente poderá ler dados do _buffer_ se existir algum dado para ser lido. Em ambos os casos, o processo fica em estado de espera até que o _buffer_ esteja pronto para a operação de escrita ou de leitura dos dados. O mecanismo que coloca os processos aguardando o recurso para prosseguir sua execução chama-se **sincronização**.

![[Pasted image 20230218004626.png]]

##### **Problemas de compartilhamento de recursos**

**Exclusão mútua**

É o mecanismo mais simples para evitar compartilhamentos problemáticos. A ideia é impedir que dois ou mais processos acessem o mesmo recurso de forma simultânea e quando um processo estiver usando um recurso, todos os demais devem ser colocados no estado de espera. A exclusão mútua afeta apenas os processos concorrentes quando eles acessam um recurso compartilhado. O trecho de código que acessa o recurso compartilhado é chamado de **região crítica**.

Em toda situação que houver **dois ou mais processos compartilhando o mesmo recurso**, seja um arquivo ou uma área de memória, deve existir um **mecanismo de controle para evitar esses conflitos de concorrência**.

Esse mecanismo de controle é conhecido como **condição de corrida**.

A exclusão mútua pode ser implementada por meio do _hardware._


##### **Soluções de _hardware_**

Neste caso, são apresentadas as soluções de desabilitação de interrupções e instruções _test-and-set._ Sabemos que os processos se comunicam, isto é, cooperam por meio do compartilhamento de posições de memória. Analogamente, _threads_ compartilham o mesmo espaço de endereçamento, ou seja, têm as mesmas variáveis globais.

Para colocar ordem nas interações entre os processos, é importante considerar que existem **operações atômicas**, as quais não podem ser interrompidas. Não é possível ver as “partes” de uma operação atômica, mas apenas seu efeito final, ou seja, não se consegue vê-la “em progresso”.

As operações do dia a dia são a base para as transações atômicas, que, por sua vez, formam a base para uma área chamada processamento de transações. Essa área trata de problemas de coordenação de acessos múltiplos e concorrentes a bancos de dados. Já os bancos eletrônicos são uma de suas aplicações importantes.

As operações atômicas devem ser muito confiáveis; e, em geral, o _hardware_ provê algumas delas.

**Transação Atômica**, é uma operação, ou conjunto de operações, em uma [base de dados](https://pt.wikipedia.org/wiki/Banco_de_dados "Banco de dados"), ou em qualquer outro [sistema computacional](https://pt.wikipedia.org/wiki/Sistema_computacional "Sistema computacional"), que deve ser executada completamente em caso de sucesso, ou ser abortada completamente em caso de erro. Um exemplo que ilustra este conceito é o da gravidez. Não se diz que uma mulher está "meio grávida"; ou ela está grávida ou não está.

O exemplo clássico para a necessidade de uma "transação atômica" é aquele da transferência entre duas contas bancárias. No momento de uma transferência de valores de uma conta "A" para uma conta "B", que envolve pelo menos uma operações de ajuste no saldo para cada conta, se o computador responsável pela operação é desligado por falta de energia, espera-se que o saldo de ambas as contas não tenha se alterado. Neste caso são utilizados sistemas que suportam transações atômicas.

##### **Mecanismo de sincronização**

A sincronização fundamenta-se na utilização de operações atômicas, para garantir o funcionamento correto de processos concorrentes.

##### **Gerência de memória**

Os computadores utilizam o conceito de hierarquia de memória em sua organização, combinando memórias voláteis e não voláteis, como memória _cache_, memória principal e memória secundária. O sistema operacional tem a função de coordenar e gerenciar a utilização dessas memórias, de forma eficiente. Esse serviço é implementado pelo sistema operacional por meio do **gerenciador de memória**. Entre as funções do gerenciador de memória destacam-se:
-   Controle das partes da memória estão sendo utilizadas e quais não estão;
-   É responsável por alocar espaços em memória para os processos que serão executados e liberar as posições de memória ocupadas quando os processos são finalizados;
-   Controle do _swapping_ de informação, constante na execução das aplicações.

##### **Unidade de Gerência de Memória**

A _Memory Management Unit_ (MMU) é um módulo de _hardware_ que faz o mapeamento entre os endereços lógicos (da memória virtual) e os endereços físicos da memória (RAM), ou seja, trata-se de um dispositivo que transforma endereços virtuais em físicos. Para isso, geralmente, a MMU traduz o número de páginas virtuais para o número de páginas físicas, utilizando um _cache_ chamado _Translation Lookaside Buffer_ (TLB). A figura a seguir ilustra o mecanismo de tradução de endereços.

![[Pasted image 20230218010456.png]]

O mecanismo de tradução do endereço virtual para o endereço físico é denominado de **mapeamento**.

##### Atenção!
<mark style="background: #D2B3FFA6;">Na maioria dos casos, os programas precisam ser compilados para que possam ser executados no sistema computacional. Várias atividades ocorrem entre o instante em que ele é compilado e o momento em que inicia sua execução: geração do código objeto, código executável, alocação em memória, nova entrada, inserção da referência do processo na fila etc.</mark>

O **mecanismo tradicional** de transformação de programas em processos está exposto na figura a seguir.

![[Pasted image 20230218020920.png]]
Na figura acima, podemos observar as fases que ocorrem desde o programa até a memória RAM, que são: a fase de compilação, envolvendo o compilador; a fase de ligação, que engloba o ligador, entre o objeto e o executável; e a fase de carga, na qual está o carregador, entre o executável e a memória RAM.

##### **Gerenciamento básico de memória**

Com relação aos gerenciadores de memória, existem dois tipos: os que permitem as trocas de processos entre a memória principal e o disco (troca de processos e paginação – mais complexos), e aqueles que não permitem (muito mais simplificados e limitados).

<mark style="background: #ABF7F7A6;">A necessidade da troca de processos e paginação acontece devido à quantidade insuficiente de memória principal para armazenar vários programas ao mesmo tempo.</mark>

##### **Monoprogramação sem troca de processos ou paginação**

Nesse caso, a memória é compartilhada entre o sistema operacional e o programa de usuário utilizado naquele momento, onde somente um programa de usuário é carregado na memória e executado por vez.

Pelo fato de permitir que apenas um único programa de usuário seja carregado em memória a cada instante, **a monoprogramação raramente é usada atualmente**, a não ser em sistemas embarcados simples.

##### **Multiprogramação com partições fixas**

Atualmente, os sistemas operacionais permitem que mais de um processo seja carregado em memória, de modo que, quando um fica bloqueado esperando por uma operação de E/S, outro, que esteja carregado em memória, possa usar a CPU. Dessa forma, a multiprogramação ajuda a melhorar a utilização da CPU, evitando desperdícios no ciclo de processamento.

Para que seja possível a multiprogramação, podemos dividir a memória em _n_ partições (muitas vezes, de tamanhos diferentes e ajustáveis). Os _jobs_ serão colocados em filas de entrada associadas a menor partição capaz de armazená-los. Pelo fato de usarmos partições de tamanho fixo, o restante do espaço de memória não utilizado pelo _job_ será perdido. Esse desperdício de memória é chamado de **fragmentação interna** (espaço de memória perdido dentro da área alocada ao processo).

a) partições fixas com filas de entrada separadas; 
b) partições fixas com uma única fila.

A limitação dessa solução de particionamento fixo de memória é discriminar _jobs_ pequenos. Já a solução é ter, pelo menos, uma partição pequena.

##### **Multiprogramação com partições variáveis**

Nesse esquema de organização, a quantidade e o tamanho dos processos na memória podem variar dinamicamente com o passar do tempo; e o tamanho das partições é ajustado dinamicamente às necessidades exatas dos processos.

A figura a seguir ilustra o funcionamento desse algoritmo, considerando a ocorrência de _swapping_: trazer um processo do disco para a memória [_swap in_], executá-lo durante um intervalo de tempo e, depois, devolvê-lo ao disco [_swap out_].

![[Pasted image 20230218022012.png]]
Podemos observar que, inicialmente, só o processo A está alocado na memória e, com o passar do tempo, os processos B, C, D e E também são carregados nela. Diferentemente do esquema de partição fixa, na multiprogramação com partições variáveis, o tamanho e a localização dos processos variam à medida que eles deixam e voltam à memória (TANENBAUM, 1995).

- Uma das vantagens desse sistema é que a flexibilidade obtida melhora a utilização da memória, evitando desperdícios de espaço.
- Contudo, a gerência dos espaços vazios é mais complicada, bem como a alocação e liberação das partições.

Há algumas formas (algoritmos) de percorrer essa lista, a saber:

**First-fit**

Inicia a procura a partir da primeira página de memória (parte baixa) e varre a memória até encontrar a primeira lacuna suficientemente grande para armazenar o processo.

**Best-fit**

Varre toda a memória e escolhe a página mais ajustada ao tamanho do processo necessário.

**Worst-fit**

Varre toda a memória e escolhe a página menos ajustada ao tamanho do processo.

**Next-fit**

Segue a mesma ideia do _first-fit,_ mas somente a primeira busca é iniciada na parte baixa da memória (primeira página), as outras se iniciam onde terminou a última. Usa-se uma lista circular para permitir que, eventualmente, toda a memória seja percorrida.

Existe a possibilidade de formar “buracos” por toda a memória ao longo da execução dos processos, o que não é viável. Assim, para eliminar esses buracos, podemos mover todos os processos para a parte mais baixa da memória – uma técnica conhecida como **compactação de memória**. No entanto, perde-se muito tempo de processamento para promover essa organização; logo, não é adequado realizar esta tarefa constantemente.

Algumas linguagens de programação permitem que a área de dados alocadas em um processo cresça ao longo de sua execução. Com isso, ocorrerão alguns problemas sempre que um processo necessitar crescer e sua partição não permitir nenhuma expansão. Se houver algum espaço nas proximidades do processo que puder ser alocado a ele, o crescimento será permitido sem que seja necessário movê-lo para outra partição maior, conforme ilustra a figura a seguir.

![[Pasted image 20230218022648.png]]
Essa figura mostra a alocação de espaço com possibilidade de expansão. Caso não haja espaço para aumentar o tamanho da partição ou não tenha uma partição grande o suficiente para realocar o processo, então, um ou mais processos deverão ser removidos para o disco (_swapping_). Se não for possível realizar o _swapping_ (área de _swapping_ cheia), o processo que deseja “crescer” deverá esperar ou ser eliminado.

**Gerência de memória com mapeamento de _bits_**

Quando se trata de gerenciar o uso das memórias, existem dois modos: com mapa de _bits_ ou uma lista encadeada indicando os espaços ocupados e os disponíveis (lista ligada).

No primeiro modo (mapa de _bits_), a cada unidade de alocação da memória, é atribuído um _bit_ para dizer se a posição está livre ou ocupada. Assim, o conjunto de todos os _bits_ é representado em uma tabela, chamada mapa de _bits_, que mapeia todas as posições de memória dizendo o estado de cada uma. O tamanho da unidade de alocação é muito importante, assim, quanto menor as unidades forem, maior será o mapa de _bits_. Como o mapa de _bits_ também é armazenado em memória, seu tamanho ocupará espaço útil e, consequentemente, uma parte da memória será desperdiçada para esse armazenamento.

<mark style="background: #ABF7F7A6;">Em virtude do processo de percorrer o mapa de _bits_ ser lento, este método quase não é usado.</mark>

![[Pasted image 20230218022934.png]]
Conforme podemos perceber nessa figura, o segmento representado por (a) possui cinco segmentos alocados a processos e três livres; o segmento (b) traz o mapa de _bits_; e o segmento (c) traz a lista ligada.

##### **Gerência de memória com lista ligada**

Os espaços livres e ocupados são feitos por meio de uma lista ligada, em que P indica uma região ocupada por um processo e H um espaço livre de memória, conforme segue na **figura** **anterior,** representação dos espaços de memória com mapa de _bits_ e lista ligada.