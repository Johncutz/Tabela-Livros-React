Detalhes do Projeto - Tabela de Livros

Ideia do Projeto: 
    Fazer uma tabela de livros que contenha o ISBN(International Standard Book Number), ou seja o número de identificação internacional do livro, deve conter também o Título do livro e o nome do Autor.
    A criação deverá ser feita com React.js

Como foi feito:
    1º De início criei uma pasta chamada "components" e dentro dela criei três arquivos:
       TabelaHead, TabelaBody e TabelaFoot e inseri no arquivo App.js

    TabelaHead:
       Dentro do arquivo TabelaHead, como esperado, contêm o "thead" ou seja o elemento que contêm o cabeçalho de uma tabela.
       Dentro do "thead" foi criado uma linha que é considerado o título da aplicação, sendo chamado "Tabela de Livros", depois foi criado três colunas, sendo elas: ISBN, Título e Autor respectivamente.

    TabelaBody:
        Dentro do arquivo TabelaBody, como esperado, contêm o "tbody" ou seja o elemento que contêm o corpo de uma tabela.
        No corpo da "tbody", deverá conter o ISBN, Título e Autor de determinado livro, além de ter também um botão de remover.
        Para obter essas informações eu peguei um arquivo JSON com tais informações e inseri no projeto para ser minha API.
        Feito isto eu importei o Component do React e criei uma class App extends Component, na qual contem um objeto state deverá ter as informações dos livros.
        Também contem o método componentDidMount() ou seja o método normalmente usado para chamadas a APIs de dados. Dentro tem o método fetch() que faz a consulta ao endereço do arquivo JSON e retorna uma promise. Por fim criei dois .then() um recebe os dados da API e o outro defini os dados no objeto state.

    TabelaFoot:
        No corpo da TabelaFoot, deverá conter apenas um texto e informar a quantidade de livros que tem na tabela. 
        Para isso eu apenas criei um "this.state.livros.length" e coloquei dentro do footer.
    
