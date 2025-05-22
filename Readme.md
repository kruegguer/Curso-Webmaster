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