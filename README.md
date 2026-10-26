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
