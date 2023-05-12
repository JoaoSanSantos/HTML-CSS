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

CAPITULO 20 - Criando New Project Cordel Moderno.

Descrevendo processo HTML: Foram separados no body 3 tags.

1° Header, para fazer o cabeçalho. Dentro do header tivemos um H1 para determinar o título e um parágrafo para créditos ao autor da poesia.

2° Sections, para dividir o conteúdo. Dentro de cada section tivemos paragrafos para o conteúdo escrito.
Os paragrafos foram determinados Class para cade um deles, alguns com Class Normal e outros com Class Imagem. As Class imagem ganharam ID para separa-los para aplicar css separadamente.

3° Footer, para definir o Rodapé. Dentro do rodapé foi adicionado apenas um parágrafo para determinar os créditos ao criador do site.

Descrevendo processo CSS: 

Definiu-se primeiro o header, a section e o footer, cada um com suas configurações de backgrounds e cores de letras. Além disso foi definido padding, text aling e text heigh (espaçamento em 'EM').

Após essas configurações definiu-se como seria o site inteiro usando a tag * adicionando margin 0 e pading 0.

Adicionou-se as fontes com a tag @import url

adicionou-se :root para adicionar as fontes de maneira mais rápida, adicionando no root 3 fontes diferentes.

Foi definido que o HTML e o BODY teriam: min-height: 100vh;
        background-color
        font-family

Após isso abriu-se outras tags separadas para o Header que foi o Header>h1 e header>p para atribuir as diferentes caracteristicas de cada um deles.

para os links usando a tag 'a' definiu-se o texto, o estilo da fonte e a cor.

Abrindo a tag a:hover definiu-se o efeito que teria ao passar o mouse por cima de cada link, dessa forma definiu-se underline.

a Section foi separada em 5 partes:

1° Section.Normal para definir suas atribuições como background e cor de fonte.

2° Section.Imagem para definir suas atribuições como background e cor de fonte.

3° Section.Image > p para definir suas atribuições como background e cor de fonte.

4° Section#img1 para definir a imagem de fundo 

5° Section#img2 também para definir uma imagem de fundo direfente da sessão anterior.

Capitulo 21 - Tabelas

Aula 01 - Introdução

Aula 02 - Criando Tabela

Tag Table.

hierarquia de tabela simples

Table > Table Row(tr) > Table Header > Table Data (TD)

Na primeira aula foi usado somente table > tr > td, dessa forma abaixo

 <table>
        <tr>
            <td>A1</td>
            <td>B1</td>
            <td>C1</td>
        </tr>
        <tr>
            <td>A2</td>
            <td>B2</td>
            <td>C2</td>
        </tr>
        <tr> 
            <td>A3</td>
            <td>B3</td>
            <td>C3</td>
        </tr>
        <tr>
            <td>A4</td>
            <td>B4</td>
            <td>C4</td>
        </tr>
    </table>

Aula 2 - Alinhando o conteúdo em Tabelas

O alinhamento, pode ser horizontal e vertical. Para horizontal pode usar text-align e para vertical usa-se vertical-align

Se for numero, cria-se uma class para cada td que for numero e faz o alinhamento como descrito acima.

Aula 3 - Tags semanticas para tabelas




