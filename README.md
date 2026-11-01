# l4_paula_pastore_1g

1- O contêiner é como se fosse a caixa, e os itens os elementos. O flex, é inserido no elemento o pai, fazendo com que ele vire o contêiner, organizando os elementos dentro dele, os filhos diretos.

2- flex-direction: row, fazendo com que os elementos fiquem alinhados da esquerda para direita.

3- com o flex-grow: 0, que faz com que os itens não cresçam, quem distribui é o justify-content,podendo deixar o espaço no início, meio, ao redor ou entre os elementos dentro do espaço disponível.

4- o valor padrão de flex-grow é 0 , o que signica que o item não aumenta.

5- a faixa do pai, o contêiner é a mesa onde todos os itens vão ser organizados, os elementos filhos são os pratos individuais, a sobra é o espaço livre, e o flex grow determina quanto cada item(prato individual) vai ocupar desse espaço disponível.

6- o flex-grow: 1 deve ser colocado no elemento da marca, isso faz com que a marca ocupe todo o espaço que sobra na barra, enquanto os dois links permanecem apenas com o tamanho de textos.

7- soma = 2+3+1 = 6.
Valor individual = 600/6 = 100px
Item 1 = 2 * 100 = 200
Item 2 = 3 * 100 = 300
Item 3 = 1 * 100 = 100.
Cada item terá ao final, respectivamente, 200px, 300px e 100px.

8- 100 * 3 = 300, ainda faltam 300.
soma do flew grow = 0+1+2 = 3
300/3 = 100
Item 1 = 0(crescimento) * 100= 0 + 100 = 100.
Item 2 = 1(crescimento) * 100 = 100 + 100 = 200.
Item 3 = 2(crescimento) * 100 = 200 + 100 = 300.

9- Ele é ativado quando falta espaço, seu padrão é flew-shrink : 1

10- 400 * 2 = 800. Falta 200px
com o flex-shrink : 1, todos diminuem o mesmo tamanho.
600/2 = 300.
Cada item vai ter 300px.

11- Como flex-shrink : 0 faz com que os itens não encolham, ou seja, eles mantem 400px. O valor dos itens juntos é de 800px, enquanto a faixa tem apenas 600px. Então os itens vão transbordar pois falta 200px.

12- Um exemplo, seria um ícone, quando colocado com flex-shrink : 0, ele fica do mesmo tamanho independente da modificação ou a falta de espaço da página.

13- É o tamanho de um item antes ou depois dele crescer ou encolher. Quando o flex-basis tem um valor diferente de auto, o que prevalece e a base, o próprio flex em vez do width. Dito isso, nesse caso o 10rem vale como valor de partida

14- Isso acontece porque o flex-basis: 0 define o tamanho inicial dos elementos como zero, fazendo com que o navegador desconsidere o tamanho do conteúdo na distribuição do espaço. Assim, o flex-grow distribui todo o espaço disponível no container entre os elementos, de acordo com suas proporções, em vez de distribuir apenas o espaço que sobra após considerar seus tamanhos iniciais

15- flex: initial: equivale a flex-grow: 0, flex-shrink: 1 e flex-basis: auto.
    flex: 10: equivale a flex-grow: 1, flex-shrink: 1 e flex-basis: 0.
    flex: auto: equivale a flex-grow: 1, flex-shrink: 1 e flex-basis: auto.
    flex: none: equivale a flex-grow: 0, flex-shrink: 0 e flex-basis: auto.

16- Com flex: 1, os itens começam do zero; com flex: auto, eles começam com o tamanho do conteúdo devido ao flex basis.
usando flex: 1 - item 1 = 300px, item 2 = 300px
usando flex: auto - item 1 = 200px, item 2 = 400px

17- Falso. Apesar que os itens tenham o mesmo tamanho de conteúdo, flex: 1 e flex: auto não necessariamente apresentam o mesmo resultado em todas as situações. Isso acontece porque possuem valores diferentes para flex-basis:
    flex: 1: utiliza flex-basis: 0, desconsiderando o tamanho inicial do conteúdo.
    flex: auto: utiliza flex-basis: auto, considerando o tamanho inicial do conteúdo.

18- A propriedade min-width impede que o item, a palavra ou imagem diminua de tamanho, pois determina um tamanho mínimo. Para resolver, basta ajustar a propriedade para min-width: 0. Desse jeito o item poderá encolher além do tamanho mínimo do conteúdo, evitando que a palavra longa estoure a faixa.

19- Esse problema poderia aparecer na montagem de um menu lateral, quando contém um texto, palavra ou link muito longo numa área sem espaço.

20- a) A ordem será C, A, B, pois o elemento C possui order: -1, fazendo com que ele apareça antes dos demais elementos, que possuem order: 0 por padrão.
    b) A ordem de foco será A, B, C, pois a propriedade order altera apenas a ordem visual dos elementos, não a ordem de navegação pelo teclado.
    c) Porque leitores de tela geralmente seguem a ordem do HTML, e não a ordem visual definida pelo CSS. Isso pode causar confusão para pessoas com deficiência visual, pois o conteúdo pode ser apresentado em uma sequência diferente daquela que aparece na tela.

21- O valor padrão de order é 0. Entre order: -1 e order: 2, o elemento com order: -1 aparece primeiro, pois os itens são organizados em ordem crescente do valor de order. Ou seja, quanto menor o valor de order, mais a esquerda (ou acima, dependendo da direção do flex) o elemento aparece.

22- Quando o elemento pai possui align-items: stretch, todos os filhos são esticados para ocupar o espaço disponível no eixo transversal, desde que suas dimensões permitam.
    align-self: flex-end: passa por cima do alinhamento definido pelo pai e posiciona o filho no final do eixo transversal.
    align-self: auto: utiliza o valor de align-items definido no pai. Nesse caso, o filho mantém o comportamento stretch, ocupando o espaço disponível.

23- Align-items é utilizado no elemento pai para definir o alinhamento de todos os seus filhos no eixo transversal, enquanto align-self é utilizado individualmente em um filho para alterar seu alinhamento, independentemente do que foi definido pelo pai.

24- Itens de .pagina: <header>, <div class="miolo"> e <footer>, pois são filhos diretos de .pagina.
    Itens de .miolo: <aside> e <main>, que são filhos diretos de .miolo.

25- Porque .miolo possui duas funções: é um item flex dentro de .pagina e também precisa funcionar como um container flex para organizar seus próprios filhos. Ao utilizar display: flex em .miolo, os elementos <aside> (menu) e <main> (texto) são organizados lado a lado, permitindo criar um menu lateral e uma área de conteúdo principal.

26- .pagina - organiza o topo, o miolo e o rodapé na vertical.
    .miolo - organiza o menu e o conteúdo lado a lado, e ocupa o espaço restante da página.
     aside - define uma largura fixa para o menu lateral.
     main - ocupa o espaço restante e permite que o conteúdo se ajuste sem estourar o layout.

27- O erro é utilizar flex-grow: 1 diretamente no contêiner, pois essa propriedade controla o crescimento de um item flex, e não do próprio container. A correção é aplicar display: flex no elemento pai e flex-grow: 1 no elemento filho que deve ocupar o espaço disponível

28- min-width: 0 - Permite que o item encolha abaixo do tamanho mínimo do seu conteúdo, evitando que ele ultrapasse os limites do container, é indicado quando o problema acontece porque o valor padrão min-width: auto impede o item flex de encolher
    overflow-wrap: break-word - Permite que as palavras muito grandes sejam quebradas em mais de uma linha, fazendo com que não transborde, é indicado quando o problema é causado por palavras extensas, links ou sequências de caracteres sem espaços.

29- flex-basis: define o tamanho inicial de um item antes da distribuição do espaço disponível.
    flex-grow: determina quanto um item pode crescer para ocupar o espaço que sobra no contêiner.
    flex-shrink: determina quanto um item pode encolher quando não há espaço suficiente.
    order: define a ordem visual em que os itens aparecem dentro do contêiner flex.
    align-self: permite definir individualmente o alinhamento de um item, independentemente do alinhamento definido pelo pai.
