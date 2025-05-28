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

    1. Box Model é uma entidade que é criada em todo elemento fo HTML;
    2. Ela consiste ela consiste em quatro partes: Altura e Largura, Padding, Border e Margin;
    3. Todas elas podem ser alteradas por CSS;
    4. Alguns elemento do HTML já vem com valor nestas regras;

    -> Height and Width

        1. A altura e a largura são o core do box model;
        2. Estas propriedades consistem no conteúdo do elemento;
        3. Podemos alterar as duas e mudae o tamanho do elemento na tela;
        4. Alguns elementos do HTML, os block elements, já vem com 100% de largura, preenchendo a tela toda na horizontal;
    
    -> Padding

        1. é o espaço entre o conteúdo e a borda do elemento, també conhecido como espaçamento interno;
        2. Este recurso é utilizado para criar uma distância entre o conteúdo (texto) e a extremidade do elemento;