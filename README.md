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

Aula 13 - Tabelas Responsivas

Envelopa a table inteira em uma DIV com id e em style adiciona            
        div#nomedoid {
                overflow-x: auto;
            }

Dessa forma a barra de rolagem vai ficar somente na tabela e não na página inteira.

Módulo 4 - Capitulo 22 - Aula 1 - Iframe:

Na aula 1 foi usado a tag iframe no meio de um parágrafo, onde foi possivel visualizar um site inteiro em uma pequena janela (bloco)

Aula 2 - Configurando iframes

Tamanho padrão do iframe é de 300x150.
Para alterar os tamanhos é só mudar em style o width e height (tamanho e largura)

É possível mudar fora do CSS logo na tag iframe, mas se houver alteração no CSS o que vai valer é o CSS.

Existe um parâmetro de rolagem, caso não tenha, você pode adicionar na tag iframe 'solling' com as opções AUTO(Se for necessário vai aparecer); Yes (independente se é necessario ou não); No (Não vai permitir rolagem, porem em alguns navegadores deixam.)

É possivel personalizar a borda também na CSS usando border: px solid black.

OBS: Nem todos os sites dão permissão para usa-los em iframe

Aula 3 - Conteúdo Local no iframe

Dentro da tag iframe é possivel adicionar páginas internas como foi colocado a tabela do módulo anterior.
Também é possível definir o local onde esse frame irá aparecer usando em CSS as tags 

         iframe {
            display: block;
            margin: auto;
        }

Aula 4 - Navegação no iframe

Caso o arquivo estiver em pasta diferente, basta localizar o caminho como descrito abaixo: 

        <iframe src="paginas-extras/pag001.html" frameborder="0" height="500" width="500">

Nessa situação o iframe funciona normalmente.

É possível adicionar em uma lista UL>LI
links para páginas, mas de uma forma que ela não saia dessa página e sim apareça a pagina externa em um iframe.
Para fazer isso, seu iframe precisa, OBRIGATÓRIAMENTE, ter um name (nome)
para que então você consiga dar um direcionamento do seu link para o iframe.

Vimos que ao envelopar um link podemos direciona-lo para uma página externa usando target:_blank, más é possível direciona-la para um iframe usando target:(nome dado ao iframe.)
Dessa forma o site externo aparecerá em seu iframe de forma simples.

Aula 5 - Conteúdo no iframe por código

Quando recarregamos a página, o iframe fica uma tela em branco. Podemos mudar isso indo no src do iframe para abrir a primeira página exemplo: 

        <iframe name="frame" src="paginas-extras/pag001.html" >

Porém temos um parâmetro novo que no lugar de src, criamos outro parametro que é o srcdoc, podendo adicionar textos ou imagens.
Textos:

         <iframe name="frame" srcdoc="<h1> Escolha uma das opções acima</h1>"

Imagens: 

         <iframe name="frame" srcdoc="<h1> Escolha uma das opções acima</h1> <img src='imagens/teste01.png'>" >

o código <img src='imagens/teste01.png'> PRECISA ESTAR ABERTO E FECHADO POR <> E POR '' (ASPAS SIMPLES)

Aula 6 - Incovenvenientes do iframe

As vezes o bot do google pode ter problemas para indexar o iframe, fazendo com que seu site não seja tão bem ranqueado.
Se o site não for responsívo, vai aparecer todo quebrado no iframe.
Cuidado com os sites que você coloca no iframe, você pode sofrer ataques de hackers.
Mas como me protejer disso?

Aula 7 - Tornando iframes mais seguros

Existem algumas regras que podemos utilizar para proteger nossos iframes.
Uma delas é a tag sandbox="sandbox" dentro do iframe como está abaixo:

    <iframe src="paginas-extras/pag004.html" sandbox="sandbox">  

OBS: Foi usado um formulário básico de exemplo.   

Dessa forma você vai estar bloqueando que o usuario envie dados pelo seu iframe.

Outra forma é configurar o parâmentro referrerpolicy (politica de referencia)
o valor padrão desse parametro é o 
"no-referrer-when-downgrade" OBS:Não precisa digitar isso.
Se você quiser tornar o que esta dentro do seu iframe um pouco mais limitado, basta colocar somente "no-referrer". Quando você faz isso, você esta dizendo que o que esta carregado no iframe não vai coletar nenhum tipo de informação do usuário.
Caso você queira deixar que o conteúdo do iframe, nesse caso o formulário, receba alguns dados você pode colocar o seguinte parametro:

    <iframe src="paginas-extras/pag004.html" sandbox="allow-same-origin">

allow-same-origin ( Permitir conteúdo de mesma origem.)

Ao apertar ctrl + espaço vai aparecer outros parametros. como allow-forms; allow-scripts etc etc.
Adicionando mais esses dois parametros você esta dizendo que para esse iframe você permite coisa da mesma origem, uso de formulários e scripts. Todo o resto continua ligado na segurança.

Aula 8 - Dicas para iframes melhores

Com iframes pode incorporar:
Videos, mapas e documentos do google docs (creio que de outros lugares também).

Capitulo 23 - Aula 1 - Criando um Projeto do Zero

Feito

Capitulo 24 - Aula 1 - Formulário

Para iniciar um formulario, ele precisa estar entre as tags 
<form></form>. Feito isso, cada parágrafo que criar dentro dele será um conteúdo do Formulário, como nome, sobrenome etc.
Para fazer esses campos virarem de fato um formulário precisa adicionar logo após o conteúdo do parágrafo a tag input:text (para texto) e input:submit (para botão).
É importante saber que não existe até o momento uma ligação entre o seu texto e sua caixa, precisa antes de algumas informações para que fique de forma util.
Caso aquela barra que aparece os nomes para completar automaticamente esteja atrapalhando, é só adicionar dentro da tag form o parametro autocomplete:off

Aula 2 - Label

Para enviar o formulário para algum lugar ele precisa de um diretório.
Foi usado de exemplo o php.
Dentro da tag form, adiciona-se o parametro action="cadastro.php"

Para fazer a ligação da caixa do nome e do sobrenome, precisa adicionar as label (etiqueta). É necessário todo texto ter um nome e um id que já aparecem quando adiciona input.
Para adicionar label, envelopa o texto do paragrafo com a tag label e adiciona o nome que está no ID.
Ao enviar esses dados, ele fica na barra de URL do navegador indicando, nesse caso, qual o nome e o sobrenome. Mas como fazer para sumir com isso no caso de senhas?

Aula 3 - Métodos Get e Post

Get já é um método padrão, é esse método que faz com que apareça os dados após o envio do formulário na URL.
O método Post some com esses dados, para usa-lo, na tag form, adiciona-se o parametro method=post, dessa forma os dados não ficam na URL.
Não significa que os dados estão protegidos, somente não estão aparecendo visualmente na URL.
Existe uma maneira de ver esses dados. 
Inspecionando o formulário na aba Network aparecerá o arquivo pra onde está indo esses dados e consequentemente os dados enviados. 
Para proteger 100% os dados é preciso usar HTTPS.
Usa-se o método post quando os dados não forem sensíveis, como nome, peso, idade, etc.
Quando se envia dados por get só pode ser enviado 3000 bits ou 3000 letras.
No caso de dados sensiveis, imagens e outros o método a ser usado é o post, que inclusive não tem o limite de 3000bits.

Aula 4 - Criando caixa de texto e senha

No formulário já criado, existe um problema. Quando você aperta no botão de enviar, mesmo sem nenhum dado ele envia mesmo assim. Isso é pq esta faltando alguns atributos.

Dentro da tag imput, para fazer com que o campo seja obrigatório, adiciona-se required como parametro.
Pode definir também o tamanho do conteúdo que será digitado.
Em input também logo após required, adiciona-se minlength="5" (minimo) e maslength="15" (máximo)

Outro parametro, ainda em input é o SIZE, que delimita quantas letras vai caber no quadro, caso exceda esse valor, criará uma rolagem lateral.

Da também pra colocar um texto indicativo no balão, ainda em input, adiciona-se placeholder e o que quer que esteja escrito.

O autocomplete pode ser usado não só na tag form, como também em input.
Quando em form o autocomplete estiver ligado, adiciona ele em input em cada caixa indicando o que é.
Por exemplo na caixa de usuario coloca-se autocomplete="username".
Na caixa de senha tem 2 tipos diferentes, tem o autocomplete="current-password" e o 
autocomplete="new-password".
O currente-password é usado para login e o New password é usado para cadastro.

Aula - 5 Number, month, date e time

Criando o input:number abre uma caixa só para numeros. 
Se o conteúdo a ser digitado nessa caixa forem numeros inteiros, basta definir só o maxlength e o minlangth(0).
Se precisar de numero quebrados, adiciona-se o parametro step e colocar por exemplo 0.5 ou 0.1;

Criando input:month, você da a opção de selecionar mês e ano. Adicionando a tag value, você pode definir uma data base atual que aparecerá automaticamente como descrito abaixo:
value="2023-05"

O input:date é a mesma coisa do month, o que muda é que será adicionado o dia do ano.

E o input:time mostra as horas.

Aula 6 - Compatibilidade com navegadores

Todo navegador é diferente um do outro. O safari do desktop é o pior deles.

Aula 7 - Formulário com Telefone e email

telefone e o email não tem tanta diferença dos outros acima.
input:tel para telefone e input:email para email.
Porém, para telefone tem um parâmetro chamado pattern que é usado para conter uma expressão regular.
Toda expressão regular começa com ^ e termina com $.
Exemplo abaixo:

pattern="^[0-9]{4}-[0-9]{4}$"

Isso significa que vai ler digitos de 0 a 9 e os primeiros digitos serão 4 - os segundos digitos depois da barra também serão lidos de 0 a 9 e serão também 4 digitos.
A expressão acima é para numeros simples, para celular muda para:

pattern="^[0-9]{4,5}-[0-9]{4}$"

ou pode ser escrito dessa outra forma

pattern="^\d{4,5}-\d{4}$"

Para colocar ddd

pattern="^\(\d{2}\)\d{4,5}-\d{4}$"

Outra coisa que pode ser feito é agrupar tudo isso (nome, email, telefone) em uma tag chamada fieldset, feito o agrupamento, entre a tag fieldset e o primeiro paragrafo adiciona outra tag chamada legend. O fieldset vai fazer uma borda agrupando o formulario e a tag legend vai dar um titulo pra isso, que pode ser por exemplo 'dados pessoais'.

Aula 8 - Checkbox e Radio Button

A checkbox como o nome já diz é uma caixa para confirmar opções.
No caso abaixo foi usado esportes:

     <fieldset>

        <legend>Esportes favoritos</legend>

        <input type="checkbox" name="esbas" id="iesbas"> <label for="iesbas">Basquete</label> <br>

        <input type="checkbox" name="esfut" id="iesfut"> <label for="iesfut">Futebol</label><br>

        <input type="checkbox" name="esvo" id="iesvo"> <label for="iesvo">Vôlei</label> <br>

    </fieldset>

Dentro de fieldset foi adicionado legend para dar legenda ao fieldset e o input:checkbox. Fora da tag foi dado o nome dessa caixinha e esse nome foi envelopado em label, para que a caixinha fosse selecionada ao clicar em cima do nome.

O input:radio serve para selecionar sexo.
Exemplo de html abaixo:

     <fieldset>

        <legend>Sexo</legend>

        <input type="radio" name="sexo" id="isxmas"> <label for="isxmas">Masculino</label>

        <input type="radio" name="sexo" id="isxfem"> <label for="isxfem">Feminino</label>

    </fieldset>

Dentro de um novo fieldset, foi adicionado novamente a tag legend e o input:radio.
É sempre 1 input para uma caixa diferente, nesse cado do input radio, é necessário que o NAME seja o mesmo, no caso acima esta 'sexo'. Caso o name seja diferente, ao selecionar um sexo, você não consegue tirar essa seleção ao selecionar o outro, nesse caso os dois ficarão marcados, por isso o name deve ser igual, para poder alternar de um para o outro.
Caso queira que um dos dois já esteja selecionado quando o usuario acessar o formulário, basta adicionar o parametro, dentro do input, checked. Dessa forma ele já aparecerá selecionado.
É necessário dentro de cada input:radio adicionar o padrão Value definindo um nome como M para masculino e F para feminino, se não ao enviar aparecerá como ON.É necessário dentro de cada input:radio adicionar o padrão Value definindo um nome como M para masculino e F para feminino, se não ao enviar aparecerá como ON.

Aula 9 - Elementos Color ,  range e file

Color é para que apareça uma paleta de cor na página.

     <p>
            <label for="icor">Cor</label>
            <input type="color" name="cor" id="icor">
        </p>

Range irá colocar uma barra que pode ser mudada de nível, começando do zero até o 100, que pode ser alterada de 0 para 10 ou qualquer outro numero

    <p>
            <label for="inivel">Nivel de Satisfação</label>
            <input type="range" name="nivel" id="inivel" min="0" max="10" value="0">
        </p>

File é para enviar documentos, imagens e arquivos. Lembrando sempre que o form tem que estar em Post para que não dê nenhum problema.

     <p>
            <label for="ifoto">Foto</label>
            <input type="file" name="foto" id="ifoto">
        </p>

Aula 10 - Select, datalist e textarea

Select serve para criar uma lista de escolha, no exemplo abaixo usamos Estados. Nesse formato só é possível escolher aquilo que foi delimitado pelo programador.

    <p>
            <label for="iest">Estado</label>

            <select name="estado" id="iest">

                <optgroup label="Região Sudeste">
                    
                    <option value="" selected>---Escolha---</option>

                    <option value="SP">São Paulo</option>

                    <option value="PR">Paraná</option>

                    <option value="RJ">Rio de Janeiro</option>

                </optgroup>

                <optgroup label="Região XYZ">

                    <option value="AM">Amapá</option>

                    <option value="MT">Mato Grosso</option>

                </optgroup>
            </select>

Cada option será uma opção de escolha na lista, optgroup faz um agrupamento dessas opções em um grupo especifico.

Datalist é igual ao select, porém além de mostrar as opções da lista, também é um quadro digitável, caso a opção que você procrua não esteja na lista.

    <label for="iprof">Profissão</label>

            <input type="text" name="prof" id="iprof" list="lstprof">

            <datalist id="lstprof">

                <option>Administrador</option>

                <option>Contabilista</option>

                <option>Desenvolvedor</option>

                <option>Professor</option>

            </datalist>
        </p>

Textarea é uma area onde o usuario pode escrever um texto de qualquer tamanho, além de poder aumentar e diminuir o tamanho do bloco.

      <p>
            <label for="imsg">Mensagem</label>
            <textarea name="msg" id="imsg" cols="30" rows="10"></textarea>
        </p>

Aula 11 - Elemento Output 

Output pode servir para somar dois numeros de campos diferentes, usando javascript.

     <p>
            <label for="in1">Numero 1:</label>
            <input type="number" name="n1" id="in1" min="0" max="50" required oninput="isoma.innerHTML = Number(in1.value) + Number(in2.value)">
        </p>
        <p>
            <label for="in2">Numero 2:</label>
            <input type="number" name="n2" id="in2" min="0" max="50" required oninput="isoma.innerHTML = Number(in1.value) + Number(in2.value)">
        </p>
    <p>
            <label for="isoma">Soma:</label>
            <output name="soma" id="isoma">0</output>
        </p>

O output também pode dar valor a barra do range, html fica dessa forma:

    <p>
            <label for="inum">Número:</label>
            <input type="range" name="num" id="inum" min="0" max="10" value="0" oninput="ival.innerHTML = Number(inum.value)">
            <output id="ival">0</output>
        </p>

Capitulo 25 - Aula 1 -  O que são Media Queries?

Media query é necessário quando a exibição é feita para tamanhos diferentes de mídias, como celula, table, diferentes tamanhos de munitores etc.
Media Query serve para apresentar um mesmo conteúdo ou site de diversos tamanhos diferentes.Media Query serve para apresentar um mesmo conteúdo ou site de diversos tamanhos diferentes.

Aula 2 - Criando site com versão para impressora

    <header>
        <h1>Noticias</h1>
        <menu>
            <ul>
                <li>Esportes</li>
                <li>Política</li>
                <li>Tecnologia</li>
            </ul>
        </menu>
    </header>
    <main>
        <article>
            <h2>Midia Quiries</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis, quis dolor. Nostrum alias voluptatibus error voluptas quae, vel fugiat tenetur cupiditate ipsum odio, veniam consequatur perferendis aperiam saepe. Sunt, voluptates?</p>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos, impedit adipisci, dolore expedita excepturi illum, praesentium est provident suscipit ea explicabo nisi. Autem rerum sapiente nobis dolores itaque, esse deleniti?
            </p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci veritatis possimus dolore id illum cum sint quos amet est libero reiciendis, praesentium, rem tempora aut velit fuga earum? Consectetur, iste.</p>
        </article>
    </main>

CSS:Impressora - 

    @charset "UTF-8";

/*Estilo para Impressora*/

* {
    margin: 10px;
    padding: 10px;
    font-family: 'Courier New', Courier, monospace;
    font-size: 1em;
    line-height: 1.5em;
}

menu {
    display: none;
}

article {
    width: 100%;
}

article::after {
    content: 'Esse artigo foi impresso através do site www.cursoemvideo.com';
}

CSS:Tela - 

    @charset "UTF-8";

/*Estilo para telas*/

* {
    margin: 0px;
    padding: 0px;
    font-family: sans-serif;
    font-size: 1em;
}

header {
    background-color: rgb(158, 158, 158);
}

header >h1 {
    text-align: center;
}

menu ul {
    list-style-type: none;
    background-color: grey;

}

menu li {
    background-color: rgb(75, 75, 75);
    color: white;
    display: inline-block;
    padding: 10px;
}
article {
    width: 600px;
    display: block;
    margin: auto;
}}

Isso nada mais são do que MEDIA TYPES.

Temos dois tipos de media acima o media screnn e o media print.

Isso é definido abaixo do title, adicionando dois links pra css separados.
Um com parametro media screen e o outro com media print (tela/impressora)

Aula 3 - Multiplas Media Features com CSS

Media Query = Media type + Media Features

Existem dois tipos de orientações do dispositivo, são elas portrait (em pé)
e landscape (deitado).

Quando se coloca media types, dentro dela pode ser criado também as medias features, dessa forma abaixo:

    <link rel="stylesheet" href="estilos/style.css" media="all">

    <link rel="stylesheet" href="estilos/retrato.css" media="screen and (orientation: portrait)">

    <link rel="stylesheet" href="estilos/paisagem.css" media="screen and (orientation: landscape)">

As medias features precisam estar entre parenteses.
O media all, significa que é para todas as midias, já os dois medias screens são específicos para telas, um será em retrato (portrait) e o outro em paisagem (landscape).
Cada feature vai dar uma orientação para mobile quando ele estiver em pé ou deitado deixando de certa forma o site responsivo.

Aula 4 - Reunindo tudo em um unico CSS

Quando o projeto é pequeno, não é necessário 3 páginas de css, pois é possível agrupar tudo isso em um unico CSS.

Abaixo de title abre um style e coloca suas declarações lá, da seguinte forma:

     <style>

        /*Declarações gerais*/

                    * {
                margin: 0px;
                padding: 0px;
                font-family: Arial, Helvetica, sans-serif;
            }

            html, body {
                width: 100vw;
                height: 100vh;
                background-color: #233eff;
                background-size: contain;
                background-repeat: no-repeat;
            }

            h1 {
                color: white;
                text-shadow: 3px 3px 0px #233eff;
                padding: 10px;
            }
        /*Declarações Portrait*/

            @media screen and (orientation: portrait) {
                body {
    background-image: url(../imagens/cev-portrait.jpg);
    background-position: center bottom;
}
            }

        /*Declarações Landscape*/

            @media screen and (orientation: landscape) {
                body {
    background-image: url(../imagens/cev-landscape.jpg);
    background-position: left bottom;
}
            }

    </style>

Sempre tem que ter o @media screen e a orientação em parantese.
Ou se preferir, pode criar uma pasta de css e incluir essas declarações dentro dela, porém não pode esquecer que a declaração de media all precisa ter a tag dela também.
É só adicionar antes das declarações de media all o
@media all {e as declarações aqui dentro}. Não é necessário fazer isso, mas é pra ficar organizado.

Aula 6 - Mobile First

Abordagem criada em 2009 por Luke Robusk que trabalhava no yahoo e hj ta no google.Abordagem criada em 2009 por Luke Robusk que trabalhava no yahoo e hj ta no google.

Aula 7 -Criado html e css mobile first

Aula 8 - Device Breackpoints

Nada mais é que o tamanho de telas como (celular, tv, monitor etc.).

O HTML Ficou assim:

    <!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Media Query</title>
    <link rel="stylesheet" href="estilos/style.css" media="all">
    <link rel="stylesheet" href="estilos/media-query.css">
</head>
<body>
    <main>
        <h1>Testando Media Queries</h1>
        <img id="phone" src="imagens/icon-phone.png" alt="Acessando via Smartphone">
        <img id="tablet" src="imagens/icon-tablet.png" alt="Acessando via Tablet">
        <img id="print" src="imagens/icon-print.png" alt="Versão para Impressão">
        <img id="pc" src="imagens/icon-pc.png" alt="Versão Desktop">
        <img id="tv" src="imagens/icon-tv.png" alt="Versão para Tv">
    </main>

</body>
</html>

Percebe-se que foram criados duas pastas para CSS. 
1° Mobile First:

    @charset "UTF-8";

/*Versão Mobile First*/

* {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1.3em;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

html {
    height: 100vh;
}

body {
    background: black url(../imagens/back-phone.jpg) no-repeat;
    background-size: cover;
    background-position: center center;
}

main {
    background-color: rgba(255, 255, 255, 0.842);
    width: 90vw;
    margin: auto;
    margin-top: 20px;
    border-radius: 10px;
    padding: 10px;
}

h1 {
    text-align: center;
    color: white;
    font-size: 1em;
    text-shadow: 2px 2px 2px rgba(0, 0, 0, 0.493);
}

img {
    display: block;
    margin: auto;
}

img#phone { display: block;}
img#tablet {display: none;}
img#print {display: none;}
img#pc {display: none;}
img#tv {display: none;}

2° Para outros tamanhos de tela:

    @charset "UTF-8";

/*Todas as demais midias*/

/*Typical Device Breackpoints
-----------------------------
Celular: 320px - 480px
Tablet: 481px - 768px
Desktop: 1025px - 1200px
Tv: 1201px acima*/

@media print {

    * {
        font-family: 'Courier New', Courier, monospace; 
    }

    body {
        background-image: url(../imagens/back-print.jpg);/*desnecessário*/
        
        
    }

    main {
        width: 90vw;
        border: 2px solid black;
    }

    main::after {
        content: 'Essa impressão foi feita por João Carlos';
        text-decoration: underline;
        font-size: 0.7em;
        text-align: center;
    }

    main h1 {
        text-shadow: none;
        color: black;
    }

    img#phone { display: none;}
    img#tablet {display: none;}
    img#print {display: block;}
    img#pc {display: none;}
    img#tv {display: none;}
}

   

@media screen and (min-width: 768px) and (max-width: 992px) {
    body {
        background-image: url(../imagens/back-tablet.jpg);
    }

    img#phone { display: none;}
    img#tablet {display: block;}
    img#print {display: none;}
    img#pc {display: none;}
    img#tv {display: none;}
}

@media screen and (min-width: 992px) and (max-width: 1200px) {
    body {
        background-image: url(../imagens/back-pc.jpg);
    }

    img#phone { display: none;}
    img#tablet {display: none;}
    img#print {display: none;}
    img#pc {display: block;}
    img#tv {display: none;}
}

@media screen and (min-width: 1201px) {
    body {
        background-image: url(../imagens/back-tv.jpg);
    }

    img#phone { display: none;}
    img#tablet {display: none;}
    img#print {display: none;}
    img#pc {display: none;}
    img#tv {display: block;}
}

Aula 9 e 10 - site com menu responsivo

html

    <!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Media Query</title>
    <link rel="stylesheet" href="estilos/style.css">
</head>
<body>
    <header>
        <h1>Meu Site</h1>
        <menu>
            <ul>
                <li><a href="#">opção 1</a></li>
                <li><a href="#">opção 2</a></li>
                <li><a href="#">opção 3</a></li>
                <li><a href="#">opção 4</a></li>
                <li><a href="#">opção 5</a></li>
            </ul>
        </menu>
    </header>
    <main>
        <article>
            <h2>Testando Media Queries</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, asperiores porro praesentium esse assumenda architecto aliquid cum voluptates minima perferendis deserunt aut doloribus sequi ipsa, consectetur, error temporibus magnam alias?</p>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cupiditate magnam velit commodi incidunt voluptate id assumenda quaerat rerum doloribus totam laborum optio, ipsam quas aspernatur ratione. Quis animi nam iusto.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate, natus. Obcaecati molestias recusandae, unde autem nesciunt reprehenderit aperiam provident iusto animi. In soluta illum, modi possimus aliquid iure? Amet, recusandae!</p>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ducimus magni velit excepturi corporis, fugit commodi. Aspernatur optio nostrum iure cum deleniti, accusantium aut consequatur quam aliquid culpa, eum esse tempora.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum neque possimus delectus sapiente molestias ipsam repellat at totam doloribus ad alias sit, rerum repudiandae, laudantium eveniet. Cupiditate, ducimus ab. Vitae.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat corrupti et molestiae quos adipisci repellat beatae odio suscipit, reprehenderit dicta minima quas dolores, placeat dolorem, nostrum velit! Distinctio, magnam laboriosam?</p>
        </article>
    </main>
</body>
</html>

CSS 

    @charset "UTF-8";

* {
    font-family: Arial, Helvetica, sans-serif;
    margin: 0px;
    padding: 0px;
}

body {
    background-color: lightgray;
}

header {
    background-color: grey;
}

header > h1 {
    padding: 10px;
    text-align: center;
}

menu {
    display: block;
}

menu > ul {
    list-style-type: none;
}

menu > ul > li > a {
    display: block;
    padding: 10px;
    text-decoration: none;
    text-align: center;
    background-color: rgb(87, 87, 87);
    color: white;
    border-top: 2px solid grey;
}

menu > ul > li > a:hover {
    background-color: grey;
}

main {
    width: 90vw;
    background-color: white;
    margin: auto;
    margin-top: 10px;
    padding: 10px;
    border-radius: 10px;
}

article > h2 {
    padding-bottom: 20px;
    text-align: center;

}

article > p {
    text-align: justify;
    margin-bottom: 20px;
    text-indent: 20px;
}

Aula 11 - Criando menu Hambúrguer

Para Criar o Menu hamburguer é simples, da pra ussar o código do google icon: https://m3.material.io/resources/icons.

A partir daí, você vai escolher o estilo do icone. ctrl+f abre uma barra de navegação, pesquise por navigation e achará o icone menu.
Para usa-lo você vai entrar em: https://developers.google.com/fonts/docs/material_icons?hl=pt-br.
E procurar por fonte do icone na web.
Um pouco mais abaixo estará o código do google web fonts.

<link href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet">

Copia o link e cole abaixo do title.

No html abaixo do h1 e acima do menu adiciona-se a tag i com a class material-icon e se quiser pode dar um id também. Dessa forma é só escolher o icone através do nome, no exemplo abaixo o nome esta menu.
<i id="burguer" class="material-icons">menu</i>

Em CSS 

i#burguer {
    background-color: rgb(48, 48, 48);
    color: white;
    display: block;
    text-align: center;
    padding: 10px;
    cursor: pointer;
}

i#burguer:hover {
    background-color: white;
    color: black;}

Agora vem os próximos passos:
Passo 1: Desligar o display do menu (none)
Passo 2: Dar um id para o menu, em html.
Passo 3: Adicionar Javascript como o exemplo abaixo

OBS: O ID dado ao menu foi 'itens'

    <script> 
        function clickMenu() {
            if (itens.style.display == 'block'){
                itens.style.display = 'none'
            }
            else {
                itens.style.display = 'block'
            }
        }
    </script>

OBS 2: Esse script é logo abaixo da tag Main e acima da tag Body
OBS 3: Não vai ser em todos os navegadores que esse icone vai aparecer. No meu celular, por exemplo, apareceu a palavra cardápio.

Aula 12 - Media queries para outros dispositivos

Para tirar o hamburguinho em telas maiores:
Cria uma aba nova para CSS e adiciona

    @media screen and (min-width: 768px) {
    i#burguer{
        display: none;
    }

    menu { 
        display: block;
    }

    menu > ul > li {
        display: inline-block;
    }
}

Nota-se que terá um erro. Se você abrir o menu hamburguer, fechar e tentar aumentar a tela, todo o menu vai sumir. 
Para corrigir isso terá que fazer outro javascript.
Dentro da tag body da html, adiciona-se o seguinte parametro:
<body onresize="mudouTamanho()">
Em seguida dentro da tag script que já havia criado para o código anterior, adiciona-se:

     function mudouTamanho() {
            if (window.innerWidth >= 768) {
                itens.style.display = 'block'
            }
            else {
                itens.style.display = 'none'
            }
        }

