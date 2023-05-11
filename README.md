# HTML-CSS
 Curso de html e css

Estou aprendendo a gerenciar meus repositórios!

A partir daqui, estará todas as minhas anotações de cada módulo começando pelo módulo 3.

Módulo 3

Aula 9 - 

Clonando Repositórios: Abre o repositório, vai em código e abrir com github desktop. Escolha a pasta que vai ser salvo e ele vai fazer a clonagem, após isso é só abrir com visual studio code. Da pra fazer por outro computador, desde que o mesmo tenha baixado git e github.

Aula 10 - Passo a Passo... Abre o Github DESKTOP -> File -> Acount -> Fazer Login com Github.com -> Feito isso, abra novamente File -> Git -> Save.
Já vai aparecer os documentos NO GITHUB DESKTOP, basta escolher uma e vai aparecer o botão para clonar.

Capitulo 19 - Aula 1

Baixando imagens de Fundo: Baixado e adicionado no github.

Aula 2 - Colocando imagem de fundo no site

Para colocar a imagem de fundo é fácil, se for em um lugar específico cria-se uma DIV, coloca a CLASS e o ID.

Em style, cria-se a DIV.(class)e o nome que você colocou na class. border-radius vai definir borda se será quadrada ou redonda. Width e height para definir tamanho, border apenas para adicionar uma borda, coloca-se border: px, solid e cor.
para deixar as divs uma ao lado da outra display:inline-block.
Para adicionar imagem é div#q3(div/class/nome do id) adiciona-se background image: URL e faz o caminho onde esta a imagem.
Pra colocar no site todo é a mesma coisa, basta apenas adicionar em Body

Aula 3- 
Para não repetir a imagem basta usar a tag background-repeat: no-repeat
e para mudar o tamanho da imagem
background-size: px px

Aula 4- 

Para posicionar primeiro coloca coluna e depois linha, exemplo: top/left; top/rigth; bottom/left; bottom/right; center/left; center/rigth; center/center. 
Para modificar o posicionamento aos poucos adiciona height:30vh; nesse caso é onde ela vai se posicionar na view port.

Aula 5 -

background-size:conver para imagem ficar 100% na tela
background-size: contain para a imagem ficar como filme na tv, aparece bordas pretas

Aula 6 - 

Pro background não quebrar quando o conteúdo for grande, basta cadicionar em body o background-attachment: fixed.
dessa forma o background fica fixo e não quebra independente do tamanho do conteudo.

shorthand - background
 color > image > position > repeat > [size] > attachment

o size infelizmente não funciona nessa shorthand, mas é só adicionar separado, exemplo:

 background: black url('imagens/wallpaper002.jpg') center center no-repeat  fixed;
 background-size: cover;

Aula 7 - Centralização vertical de caixas.

Sempre teremos containers e conteúdos,
conteúdo é o que fica dentro de um container. Para mexer no posicionamento do conteúdo, precisa adicionar tanto no conteiner quanto no conteúdo (em style) a POSITION. São positions diferentes de container para conteúdo, em container a position precisa ser relative e em conteúdo absolute. Ao adicionar a position, você consgue mexer no posicionamento adicionando left/top/right/bottom e seus respectivos valors, assim você consegue mudar o conteúdo de lugar de acordo com os valors que você adicionou (isso está descrito no fundo007.html)
Ao colocar, por exemplo, left 50% e top 50%, nota-se que o conteúdo ficou sim no meio do container, mas levando em consideração seu ponto de partida que é o ponto inicial (o canto superior esquerdo).
Para deixar o centro do conteúdo no centro do container adiciona-se transform. O transform pode ser mexido tando em px quanto em %, assim para ficar ambos centralizados, basta adicionar dessa forma:

left: 50%;
top: 50%;
transform: translate(-50%, -50%);

Assim ambos ficarão centralizados no meio da tela.
OBS: Os valores do transform translate precisa ser negativo!

CAPITULO 20 - Criando New Project
