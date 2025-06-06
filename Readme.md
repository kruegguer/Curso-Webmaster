                            Curso front end - Hora de Codar
            
            Html

=> Estrutura do Html

    1. DOCTYPE: esta tag declara a versão do html.

    2. html: esta tag envolve todo o código;
    3. head: nesta colocamos todas as configurações de um site, como a importação de CSS e o título da página (meta tags);
    4. body: é onde todos os elementos visíveis estão;


=> Titulos (h*)

    1. Os titulos são conhecidos como headings;
    2. Utilizamos principalmente para separar seções;
    3. O nome da tag é "h*", onde o "*" pode o ser um valor de 1 a 6;
    4. O maior titulo é o h1, e também é o mais importante, colocamos apenas um por página;
    5. A importância deve estar conectada com o próposito da nossa página, este assunto faz parte do html semântico, um tópico mais avançado. 

=> Paragrafos (p)

    1. Utilizamos os paragrafos para inserir textos maiores;
    2. Cada paragrafo começa uma nova linha, e este comportamento acontece com todas as tags de bloco;

=> Tags sem conteúdo

    1. Elas introduzem um conceito de self closing tags, onde a tag não possui uma outra tag de fechamento - ex: <br/>.

=> Comentários no Html

    1. Comentários são utilizados para descrever como algo funciona ou explicar para outros programadores o que fizemos.
    2. ex: <!--Comentário-->

=> Atributos

    1. Atributos podem ser utilizados para adicionar funcionalidades as tags;
    2. Ex: <a href="https://www.google.com" Google</a> - Tag de links;
    3. Ex2: abrir uma nova aba: _blank // <a href="https://www.google.com" target="_blank "Google</a>;

=> Imagens no Html

    1. Nós podemos inserir imagens no nosso site com a tag img;
    2. O caminho relativo até a imagem é inserido no atributo src;
    3. Normalmente colocamos uma imagem numa pasta chamada img ou assets;
    4. A tag img é uma self closing tag;
    5. Atributo Alt na tag img -> <img src="endereço da imagem" alt="Descrição da imagem"/>;
        5.1. Este recurso é importante para acessibilidade, fazendo com que nosso site seja melhor rankeado pelo Google também;

=> Listas não Ordenadas

    1. Listas são muito Importantes para o site;
    2. Podemos criar um menu a partir de uma lista;
    3. As não ordenadas são criadas pela tag ul;
    4. Cada item na lista é representado pela tag li;

=> Listas Ordenadas

    1. Listas ordenadas são interessantes para quando há um procedimento ou passos a serem seguidos;
    2. Ex: Receita de Bolo;
    3. Agora utilizamos a tag ol;
    4. Cada item na lista é representado pela tag li;

=> Tabelas
    1. Nós usamos tabelas para exibir dados que podem ser categorizados em colunas;
    2. Tabelas são estruturas complexas no HTML, e não utilizadas;
    3. Precisamos da tag table, isso cria a tabela;
    4. Cada linha é criada em uma tag tr, e os dados ficam td;
    5. No cabeçalho utilizamos a tag th;

=> Tag Div

    1. A tag div é utilizada para criar divisões/seções no nosso site;
    2. Podemos criar elementos menores também, como cards;
    3. O principal propósito é: encapsular elementos que estão conectados entre si; 


            CSS

=> Maneiras de Adicionar o CSS

    1. Temos algumas maneiras de adicionar CSS ao HTML;
    2. Inline: quando os estilos são adicionados por um atributo;
    3. Internal: quando o css é adicionado na tag head;
    4. External: quando o css é adicionado através de um arquivo externo, e depois importado ao HTML;
    5. Vamos sempre optar pelo external CSS;

=> A Anatomia do CSS

    1. Com CSS aplicamos CSS a um elemento;
    2. Primeiramente devemos selecionar o elemento, isso pode ser feito através da tag do elemento;
    3. Depois precisamos colocar as propriedades e os valores;
    4. Se quisermos mudar a cor de algo, utilizamos: color: red;

    -> external CSS
        1. Para adicionar CSS com esta tecnica precisamos criar arquivo .css;
        2. Geralmente ele ficam numa pasta chamada css;
        3. E nós o importamos através da tag link;
            ex: <link rel="stylesheet" href="caminho do arquivo css">
        4. As regras que estão no arquivos são aplicadas no html;

=> Ordem do CSS

    1. O CSS é carregado a partir de uma ordem;
    2. Ordem: inline > internal = external > padrão do navegador;
    3. Esta regra funciona quando temos estilos em um mesmo elemento;
    4. Interno e externo tem a mesma propriedade, a ultima regra ganha "corrida";

=> Múltiplos arquivos de CSS

    1. É possível ter mais de uma folha de estilo no nosso projeto;
    2. Precimos apenas importar todas elas na tag head;
    3. Os arquivos importados por último tem mais prioridade;
    4. Esta é uma boa pratica, pois possibilita a divisão de CSS por páginas, por exemplo;

=> Comentário CSS

    1. A sintaxe é: /*comentário*/;

=> Classes e ID'S

    1. Classes e id's são atributos de tags do HTML, mas estão diretamente relacionados ao CSS;
    2. Podemos especificar elementos específico com eles;
    3. Id's são utilizados para elementos únicos - Os id's podem sobrescrever as classes. Eles possuem um valor semântico maior;
    4. Classes servem para um ou mais elementos, geralmente utilizadas em conjuntos de elementos;

    -> Classes

        1. As classes são inseridas através de um atributo de HTML;
        2. O valor do atributo é o nome da classe, e também uma escolha nossa;
        3. Por exemplo: temos um botão que aparece x vezes no nosso projeto, podemos colocar uma classe btn nele, ou seja, os padrões de estilo desses botôes podem ser transmitidos através desta classe para os demais;
        4. O seletor fica: .<nome_da_classe>;
    
    -> ID'S

        1. Os id's também são atributos do Html;
        2. Podemos escrever qualquer coisa como valor, será o nome do id;
        3. Id's são únicos, ou seja, não repetimos o mesmo nome na mesma página;
        4. O HTML não nos proíbe disso, mas é uma má prática e deve ser evitada;
        5. O seletor fica: #<nome_do_id>;

    -> Ordem dos Seletores

        1. Nós aprendemos sobre o seletor de id e classe;
        2. E se a tag estiver com id e uma classe, o que acontece?;
        3. Como nas maneiras de adicionar o css, temos também uma ordem;
        4. Ordem: Id > Classe > seletor de tag;
        5. Então o id vai vencer de todos os outros, utilize isso ao seu favor;
        6. Regras que não entram em conflito serão aplicadas normalmente;

=> As cores do CSS

    1. Em CSS as cores são divididas em grupos, temos:

        1.1. Nome de Cor: como red ou blue, não muito utilizados;
        1.2. RGB: configuramos as tonalidades de red, green, blue - vão 0 (TOM MAIS ESCURO) a 255 (TOM MAIS CLARO);
        1.3. Hexadecimal: uma união de letras e número que podem criar uma cor, a maneira mais utilizada;
        1.4. HSL: hue, saturation e lightness, mudando esses valores, temos uma cor - Muito utilizado no Photoshop;
    
        2. Hex 

            2.1. Hexadecimal ou HEX é a abordagem mais utilizada;
            2.2. Basicamente temos que inserir 6 digitos, precedidos de uma #.
            2.3. Os dois primeiros representam o tom de vermelho, depois o de verde e por fim o de azul;
            2.4. Os valores vão de 0 a 9 - A a F;
            2.5. 0 é o mais escuro e F é mais o claro;
            2.6. O valor #000 é a cor preta e #FFF é a cor branca; 
            2.7. Se o valor for repetido 6 vezes, podemos escrever a cor de forma mais simples;
                2.7.1. No caso de -#FFFFFF podemos escrever #FFF;
                2.7.2. A mesma coisa vale para -#112233, essa cor pode ser escrita como: -#123;
                2.7.3. esta é uma técnica muito utilizada;
        
        3. RGB

            3.1. RGB significa Red, Blue e Green;
            3.2. Nós precisamos inserir a intencidade de cada tom, como valores de 0 a 255;
            3.3. 0 é o mais escuro e 255 é o mais claro;
            3.4. Aplicamos RGB com a seguinte sintaxe: rgb(0-255, 0-255, 0-255);
            3.5. O primeiro valaor representa o tom de vermelho, depois o de verde e por fim o de azul;
            3.5. Ex: para criar a cor verde inserimos: rgb(0,255,0);
        
        4. RGBA

            4.1. Podemos criar cores também com o RGBA, "A" vem de alpha;
            4.2. A alteração dele muda a opacidade da cor;
            4.3. Os valores possíveis são de 0 a 1;
            4.4. Sendo 0 transparente e 1 totalmente visivel;
            4.5. A sintaxe é quase a mesma: rgba(0-255, 0-255, 0-255, 0-1);

=> Background color

    1. Quase todo elemento tem um background, e podemos mudar a cor dele;
    2. Todas as regras que vimos sobre cores podem ser aplicadas em cores de background;
    3. A regra é: background-color: "cor";
    4. As regras de cor de fundo e cor de fonte podem ser utilizadas juntas;

=> Background Opacity

    1. Podemos alterar a opacidade de uma cor de fundo com CSS;
    2. A regra é a opacity;
    3. Os valores vão de 0 a 1 - sendo o 1 totalmente visível e 0 remove a cor;
    4. Com esta regra mudamos também a opacidade dos elementos dentro do elemento que alterammos a opacidade, veremos uma solução depois;

=> Resolvendo o problema de opacidade

    1. Se você não quer aplicar a opacidade para os elementos filhos, precisa utilizar o RGBA em vez de opacity;
    2. Alterando o valor de alpha temos a opacidade colocada apenas na cor de fundo;
    3. Então preservamos o conteúdo e alteramos o background;

=> Background Images

    1. Podemos inserir imagens no background dos elementos;
    2. A regra é: background-color: url("pastaimage.jpg");
    3. Geralmente a imagem fica em outra pasta, então temos que voltar um diretório;
    4. Isso pode ser feito com o símbolo:..;

=> Centralizando a imagem de background

    1. As vezes a imagem é muito mais que o elemento que estamos inserindo, então precisamos melhorar a visualização, centralizando a imagem;
    2. Isso pode ser feito com duas regras: background-position com o valor de center e background-size com o valor de cover;

=> Box Model

    1. Box Model é uma entidade que é criada em todo elemento do HTML;
    2. Ela consiste em quatro partes: Altura e Largura, Padding, Border e Margin;
    3. Todas elas podem ser alteradas por CSS;
    4. Alguns elemento do HTML já vem com valor nestas regras;

    -> Height and Width

        1. A altura e a largura são o core do box model;
        2. Estas propriedades consistem no conteúdo do elemento;
        3. Podemos alterar as duas e mudar o tamanho do elemento na tela;
        4. Alguns elementos do HTML, os block elements, já vem com 100% de largura, preenchendo a tela toda na horizontal;
    
    -> Padding

        1. é o espaço entre o conteúdo e a borda do elemento, também conhecido como espaçamento interno;
        2. Este recurso é utilizado para criar uma distância entre o conteúdo (texto) e a extremidade do elemento;
    
    -> Padding Individual

        1. Podemos adicionar o padding aos lados individuais de um elemento;
        2. A regra é: padding - *;
        3. Onde * pode ser top, left, right ou bottom;
        4. Assim teremos valores customizados em cada um dos lados do elemento;
    
    -> Shorthand Properties

        1. As propriedades de shorthand nos permitem adicionar padding a todas as direções com uma regra;
        2. Apenas precisamos utilizar a regra padding, e configurar top, right, bottom e left nesta ordem;
        3. Exemplo: padding: 10px 5px 12px 30px;
        4. Esta regra de shorthand pode ser aplicada para outras propriedades, como a margin;
    
    -> Padding e Width

        1. A padding é adicionada a largura do elemento, e isso pode ser um problema;
        2. Por exemplo: se precisamos seguir um layout perfeitamente, um elemento com 200px de with e 25px de padding tem um tamanho total de 250px na horizontal;
        3. Podemos diminuir a largura do elemento, mas isso dificulta o calculo também;
        4. Isso pode ser resolvido com a regra box-sizing e o valor border-box, isso faz o elemento respeitar o tamanho que está em with;

    -> Border
        
        1. A borda é o elemento central, fica entre padding e margin;
        2. Padding é o espaçamento interno e margin o externo;
        3. Geralmente esta regra é utilizada com o propósito decorativo;
        4. A regra de border é definida em algumas partes: tamanho, aspecto e cor da borda;
    
    -> Border Individual
        
        1. Podemos adicionar borda aos lados especificos de um elemento também;
        2. Podemos utilizar border- *, onde * pode ser top, right, bottom e left;
        3. Isso é muito utilizado frequentemente, especialmente com a border-bottom e left;

    -> Border arredondada

        1. Com a propriedade border-radius podemos arredondar os cantos de um elemento;
        2. Podemos aplica-la assim: border-radius: 5px;
        3. Isso faz com que o canto seja arredondado em 5px;
        4. Importante: Podemos arredondar elementos que não tem a regra de border aplicada;

    -> Margin

        1. A propriedade de margin é responsável pelo espaçamento externo do elemento;
        2. Podemos aplicar o recurso como aplicamos o padding, ou seja: lados individuais e também o shorthand;

=> Alinhamento de texto

    1. Nossos textos podem ser alinhados em várias direções;
    2. Por padrão ele é alinhado a esquerda;
    3. Porém com a regra text-align configutamos center (centro) ou right (direita), para alterar o valor default;
    4. Usamos muito o valor de center;

=> Decorando textos

    1. Com a tag text-decoration podemos adicionar efeitos ao texto;
    2. É possével colocar um undeline ou até mesmo uma linha que corta o texto;
    3. Esta regra é utilizada em casos específicos;
    4. A tag "a" tem um underline por padrão, podemos remover isso com a regra de text-decoration e o valor de none;

=> Espaçamento de letras

    1. Com a regra letter-spacing podemos alterar o espaçamento entre as letras de um texto;
    2. Isso é interessante em situações que o layout pede esta mudança;
    3. A regra é aplicada da seguinte maneira: letter-spacing: 5px;

=> Fontes

    1. Com CSS podemos alterar o tipo da fonte, com a regra font-family;
    2. As regras disponiveis são: Serif, Sans-serif, Monospace, Cursive e Fantasy;
    3. Todos os navegadores tem várias fontes que podemos utilizar, e ainda podemos adicionar fontes externas, por exemplo com o Google Fonts;

=> Estilo de fonte

    1. Nós podemos utilizar a propriedade font-style para mudar o aspecto das letras;
    2. Os valores são: normal, italic e oblique;
    3. Normal é valor default, e os outros as variantes;
    5. Oblique é como o tipo italico, com pequenas diferenças;

=> Font weight

    1. A propriedade font-weight pode deixar nossa fonte de texto mais fina ou mais grossa;
    2. Os valores vão de 100 a 900. sendo 100 o mais fino;
    3. Algumas palavreas também funcionam como valores, por exemplo: bold(600);
    4. Existem fontes que não tem todas as variações, devemos tomar cuidado com isso; 

=> Tamanho de fonte

    1. A regra de font-size é responsável por deixar a nossa fonte grande ou pequena;
    2. Quanto menor o valor, menor a fonte e vice-versa;
    3. Esta regra é configurada com unidades de medida, como o px;

=> Display

    1. Em HTML e CSS temos alguns elementos que são considerado de bloco e outros inline;
    2. A tag div é um exemplo de block e span um exemplo de inline;
    3. Com a regra display podemos mudar este comportamento, ou seja, deixar uma div como inline;
    4. block: Ocupa a linha toda e os elementos quebram linha quando adicionando novos elementos block;
    5. Inline: Os elemento ficam um do lado do outro;

=> Escondendo elementos

    1. Existem situações que precisamos ocultar elementos;
    2. Basta adicionar a regra display com o valor none, então o elemento não é mais exibido, porém ainda consta no HTML;

=> Positions

    1. A regra position e seus valores são responsáveis por posionar o elemento na tela;
    2. Temos algumas possibilidades: relative, fixed, absolute, sticky e mais;
    3. O valor padrão é static, todo elemento começa com esta posição;
    4. Esta regra é essencial quando precisamos mudar onde o elemento deve dicar no projeto;

    -> Position Static

        1. O valor de static na position não faz nada com o elemento, porque este é o valor padrão, ou seja, todo elemento já tem este tipo de positin;
        2. Outros valores são afetados pelas regras: top, right, bottom e left, porém static não;
        3. Static apenas segue o fluxo do HMTL;
    
    -> Position Relative

        1. Com a position configurada como relative temos mais possibilidades que static;
        2. Agora as regras top, right, bottom e left, movem o elemento pela tela;
        3. O elemento ainda segue o fluxo do HTML;
        4. Atenção: normalmente não utilizamos estas regras de posição com relative;
    
    -> Position Absolute

        1. Com o valor de absolute em position, o elemento pode ser movido pela tela toda, ou seja, quebramos o fluxo do HTML;  
        2. Esta regra também é afetada por top, right, bottom e left;
        3. Posicionar com absolute pode ser uma solução ou um problema, dependendo do ponto de vista;
    
    -> Position Relativo com Absolute

        1. Podemos resolver o problema de absolute com relative;
        2. Um elemento com position absolute é ligado ao elemento mais próximo com posição relativa, se não ele é ligado ao body;
        3. Então com um container com posição relative, podemos controlar melhor a área de ação dos elementos com absolute;
    
    -> Position Fixed

        1. Com o fixed o elemento pode ser fixado na tela, mesmo após o scroll na página, o elemento permanece na mesma posição;
        2. O recurso é frequentemente utilizado para criar barra de navegação fixa;
    
    -> Position Sticky

        1. Sticky também faz o elemento fixar na tela, mas tem um outro comportamento também, quando o elemento volta para a sua posição original ele comporta como relative;
        2. A posição do elemento é onde ele foi inserido no HTML;
    
    -> Position z-index

        1. Se temos dois elementos com as mesmas posições ou se eles colidem na página, podemos escolher qual será exibido;
        2. Utilizamos o z-index para isso, o elemento com maior valor prevalece;

=> Formulários

    1. Forms tem o papel de receber dados do usuário e enviar para o servidor, onde podemos validar dados;
    2. As tags mais utilizadas são: form, label, input;
    3. A tag form cria o formulário e o delimita;
    4. Label descreve os inputs;
    5. O imput é a tag que inserimos os dados, temos vários tipos: number, email, text e etc;
    
    -> Criando um formulário

        1. Para criar um formulário vamos precisar da tag form, que encapsula todos os elementos do formulário;
        2. Dentro dela temos labels e inputs, mas podemos ter outras tags como divs;
        3.A tag de input tem um atributo chamado type, que é onde definimos o propósito do input;
        4. Um input do tipo text, receber dados de texto;

    -> Atributos da tag form

        1. A tag form tem dois atributos geralmente, que são: action e method;
        2. Action: arquivo/pagina que os dados serão enviados;
        3. methood: GET (receber dados) ou POST (enviar dados);
    
    -> Atributo Name

        1. Utilizamos o atributo name para configurar os nossos inputs;
        2. o valor é ligado ao próposito do input, a sua categoria;
        3 Ex: Um input que recebe a idade de um usuário, pode ter um name com o valor de age/idade;
        4. Este atributo é utilizado para pegar o valor quando form é enviado para o servidor;
    
    -> Atributo Label

        1. A tag label tem um atributo, e nós o utlizamos para linkar com um input, o nome do atributo é for;
        2. O valor deve ser o mesmo que o atributo name do atributo que corresponde aquela label;
        3. Utilizamos o for por própositos semânticos e isso ajuda o nosso site ser melhor rankeado no GOOGLE;
    
    -> Enviando dados de formulário

        1. Podemos enviar os dados do form para o servidor através de um botão de submit;
        2. O botão também é um input, porém mudamos o type para submit;
        3. Quando o usário clicar no botão o processamento do form acontece, os dados serão enviados ao servidor através de uma requisição HTTP;
        4. Aqui é onde precisamos de uma integração com o back-end, para aproveitar os dados do formulário;
    
    -> Elemento Select

        1. A tag select tem as opções representadas por tagas de option;
        2. Select também tem um atributo name;
        3. O value estará em cada uma das options, e é isso que receberemos no lado do servidor;
        4. Então temos duas tags para criar um elemento de seleção: select e option;

        -> Atributo selected

            1. Podemos iniciar o nosso input de select com uma opção selecionada;
            2. Para isso esta option precisa ter o atributo selected;
            3. Abordagem interessante para quando temos uma opção muito provável;

        -> Múltiplas seleções

            1. Podemos criar um select que nos permite mais de uma option selecionada;
            2. Interessante quando queremos aceitar um ou mais dados;
            3. Por exemplo: opicionais de um carro / recheio de um lanche;
            4. Precisamos apenas inserir o atributo multiple na tag select;
    
    -> Elemento de Textarea

        1. A taga é semelhante ao input text;
        2. Podemos utilizar para textos maiores, por exemplo: A bio do instagram;
        3. Isso nos permite uma área maior para digitar e verificar o texto que digitamos;
    
    -> Fieldset e Legend

        1. Fieldset é uma tag para agrupar inputs e legend é como uma label, que descreve os inputs agrupados;
        2. Utilizamos esta tag para conectar dois ou mais inputs que tenham o mesmo sentido;
        3. Por exemplo: nome e sobrenome;
    
    -> Datalist

        1. Datalist é como um select, porém com um autocomplete;
        2. Podemos pesquisar por possíveis valores para preencher o input ou selecionar alguma opção por meio de uma lista;
        3. As opções são linkadas por um atributo chamado list;
    
    -> Input para Senha

        1. Se nós estamos esperando uma senha do usuário, podemos utilizar a tag input, porém no atributo type colocaremos "password" e então o texto passa a ser exibido com *, para mascarar os dígitos;
    
    -> Reiniciando o form

        1. Podemos reiniciar todos os campos do form;
        2. Isso é feito através de um input do tipo reset;
        3. Ele é botão, que ao ser clicado limpa o form;
    
    -> Input Radio

        1. Este input é utilizado para selecionar apenas uma opção de várias possibilidades, por exemplo: O modelo do carro que estamos comprando;
        2. Não podemos escoher dois, então há uma necessidade da decisão entre uma das opções;
    
    -> Input Checkbox

        1. O checkbox é similar ao radio;
        2. Temos que selecionar uma ou mais opções, e também cancelar a seleção de uma opção, por exemplo: os opcionais de um carro;
    
    -> Input de Data

        1. O Input do tipo date é utilizado para selecionar uma data;
        2. Temos um calendário que nos auxilia para datas passadas ou futuras;
        3. Podemos também preencher o valor digitando;
    
    -> Input para Arquivos

        1. O input de arquivos pode ser criado com o type igual a file;
        2. Assim podemos enviar um arquivo ao servidor, por exemplo: imagens ou pdfs;
    
    -> Input para Números

        1. Configurando o type para number temos um input que só aceita dígitos;
        2. Este input possui setas, que nos permite alterar o número através de cliques;
    
    -> Input para e-mails

        1. O input de e-mail é similar ao de texto, porém quando enviamos o formulário temos uma validação que checa se o texto tem o padrão de um e-mail, verificando o @, por exemplo;
    
    -> Atributo Value

        1. Com o value podemos definir um valor ao input alvo, como se o usuário já tivesse preenchido algo;
        2. É muito utilizado quando temos um valor padrão;
    
    -> Atributo Disable

        1. O atributo disabled é utilizado para bloquear um input, então não podemos digitar neste input;
        2. Útil quando não queremos que o usuário preencha um determinado input;

    -> Atributo Placeholder

        1. Com o atributo placeholder podemos adicionar dicas para os usuário do sistemas, ela será exibida no próprio input;
        2. Ao começarmos a preencher com algum valor, a dica some e o nosso valor que fica sendo exibido;

    -> Atributo Required

        1. O atributo required força o preenchimento de algum campo, se tentarmos enviar o form sem um valor no campo com required, receberemos uma alerta da página;
        2. Isto é um tipo de validação;