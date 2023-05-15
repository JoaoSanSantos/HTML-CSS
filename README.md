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

Aula 2 - Alinhando o conteúdo em Tabelas pequenas

O alinhamento, pode ser horizontal e vertical. Para horizontal pode usar text-align e para vertical usa-se vertical-align

Se for numero, cria-se uma class para cada td que for numero e faz o alinhamento como descrito acima.

Aula 3 - Criando Tabelas Grandes

Anatomia de tabelas grandes:
        Table
                Thead
                        TR, TD, TH
                Tbody
                        TD, TD, TH
                Tfoot
                        TR, TD, TH


Mesmo que fique bagunçado e tfoot fique logo após thead, a semantica não deixará ele aparecer no meio da tabela, já vai organizar ele no rodapé.

A base de dados ficou assim:

 <table>
        <thead>
            <tr>
                <th>Estado</th>
                <th>População</th>
            </tr>
        </thead>

        <tbody>
            <tr>
                <td>São Paulo</td>
                <td class="num">45.919.049</td>
            </tr>
            <tr>
                <td>Minas Gerais</td>
                <td class="num">21.168.791</td>
            </tr>
            <tr>
                <td>Rio de Janeiro</td>
                <td class="num"> 17.264.943</td>
            </tr>
            <tr>
                <td>Bahia</td>
                <td class="num">14 659 023</td>
            </tr>
            <tr>
                <td>Paraná</td>
                <td class="num">11 835 379</td>
            </tr>
            <tr>
                <td>Rio Grande do Sul</td>
                <td class="num">11 088 065</td>
            </tr>
            <tr>
                <td>Pernambuco</td>
                <td class="num">9 051 113</td>
            </tr>
            <tr>
                <td>Ceará</td>
                <td class="num">8 936 431</td>
            </tr>
            <tr>
                <td>Pará</td>
                <td class="num">8 442 962</td>
            </tr>
            <tr>
                <td>Santa Catarina</td>
                <td class="num">7 762 154</td>
            </tr>
            <tr>
                <td>Goiás</td>
                <td class="num">6 950 976</td>
            </tr>
            <tr>
                <td>Maranhão</td>
                <td class="num">6 800 605</td>
            </tr>
            <tr>
                <td>Espírito Santo</td>
                <td class="num">4 108 508</td>
            </tr>
            <tr>
                <td>Paraíba</td>
                <td class="num">4 030 961</td>
            </tr>
            <tr>
                <td>Amazonas</td>
                <td class="num">3 952 262</td>
            </tr>
            <tr>
                <td>Mato Grosso</td>
                <td class="num">3 035 122</td>
            </tr>
        </tbody>

        <tfoot>
            <tr>
                <th>Total de Habitantes</th>
                <td class="num"><strong>210 147 125</strong></td>
            </tr>
        </tfoot>

Aula 4 - Caption e Escopo de títulos em tabelas

Caption = Legenda

caption vem antes de thead

OBS: Th significa título e TD significa dado.

Todo th tem scope='col' ou scope='row'

Scope col é para titulos onde os dados estão em coluna logo abaixo, no caso do Thead. Já o Scope row é para titulos onde os dados estão em linha ao lado,no caso do tfoot.
Caso queira diminuir a largura da tabela somente em um lado, exemplo na população, basta após o scope de 'th população' adicionar Style="width: px"

Aula 5 - Efeito Zebrado na tabela

Geralmente quando tem uma tabela com muitos dados, fica difícil acompanhar com os olhos os dados corretamente. Então para não ter essa dificuldade adiciona-se o efeito zebrado.

Em style adiciona-se

tbody > tr:nth-child(2n) {
            background-color: lightgray;
        }

O '2n' significa o numero de linhas, ou seja, ficou zebrado uma linha sim e uma linha não. Podemos tambem adicionar impar ou par usando odd ou even. 

Caso o fundo não seja braco, é interessante especificar a formula acima 2 vezes, uma cor especifica para colunas odd(impar: 1, 3, 5, 7) e even(par: 2, 4, 6, 8). Se o fundo for branco é só fazer uma tbody e fica tudo certo.

Aula 6 - Cabeçalho fixo

Para fazer um cabeçalho fixo na tabela pra que ela role pra baixo somente na tabela, é simples.
Basta em Style, adicionar:

         thead > tr > th {
            position: sticky;
            top: -1px;
            background-color: gray ;
        }

Dessa forma, seu cabeçalho ficará fixo durante a rolagem da tabela. Se tive texto abaixo da tabela, o cabeçalho irá sumir junto com a rolagem.

Aula 7 - Mesclagem de Células

Rowspan e colspan, são usados para fazer uma célula ocupar duas ou mais linhas ou duas ou mais colunas.

Basta, adicionar essa tag dentro do td que deseja ocupar mais linhas ou colunas dessa forma:

     <tr>
            <td>A</td>
            <td colspan="2">B</td>
            
        </tr>
        <tr>
            <td rowspan="3">A</td>
            <td>B</td>
            <td>C</td>
        </tr>
        <tr>
            
            <td>B</td>
            <td>C</td>
        </tr>
        <tr>
            
            <td>B</td>
            <td>C</td>
        </tr>

Aula 8 - Desafio 13

Concluido 

Aula 9 - Exemplo de Tabela Completa

exercidio feito

Aula 10 - Escopos de Grupo

Como escrito a algumas aulas atrás existem escopos diferentes para linhas e colunas, mas também existe grupos de linhas e grupos de colunas.
Rowgroup é para th que tem mais de uma linha representado.
Colgroup é para th que tem mais de uma coluna representado.

Relembrando: th/col é para coluna, th/row é para linhas. th/colgroup é para grupos de colunas e th/rowgroup para grupos de linhas

Aula 11 - Exercício

Feito

Aula 12 - Agrupando Colunas com Colgroup

Temos um pequeno problema. Quando a tabela é muito grande ex 500 linhas, como mudar o estilo de apenas uma coluna, sem precisar alterar um por um colocando class?

Dentro de table, é possivel criar uma nova tag que é a colgroup. Dentro dela você vai criar outra tag chamada col. 
O numero de 'col' vai ser de acordo com o número de colunas que tiver a sua tabela.

Feito isso, basta dar uma class para cada um, ir em style e digitar 'col.nomedaclass, ex: 

        col.cnome{
            background-color: greenyellow;
        }

Feito isso, sua coluna inteira terá um estilo, sem precisar adicionar um por um.
Caso queira pegar também um unico estilo para duas ou mais colunas, basta definir na tag 'col' SPAN="2", por exemplo, dessa forma pegará 2 colunas ou o numero de colunas que você adicionar. 