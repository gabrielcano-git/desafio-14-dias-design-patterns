# Dia 1

Durante o dia 1, tinha 3 principais grandes objetivos, que consolidei nesse arquivo.

## 🎯 Objetivos:

- Saber "O que são Design Patterns?";
- Entender os "Tipos de padrões";
- Conhecer o "Gang of Four (GoF)", e entender sua relevância.

## 📖 Recursos:
- Livro: [Design Patterns: Elements of Reusable Object-Oriented Software (GoF)](https://a.co/d/ebQH90v).
- Artigo: [Refactoring Guru - Introdução](https://refactoring.guru/pt-br/design-patterns/what-is-pattern).
- Vídeo: [O que são Design Patterns?](https://www.youtube.com/watch?v=J-lHpiu-Twk)

## Aprendizado

Na minha cabeça, os padrões de projeto tinham uma conexão muito grande com os livros do *Uncle Bob*, que, pela forma como são escritos, me causam um pouco de gastura.

Os padrões de projeto são como um cinto de utilidades do Batman para que você possa resolver os problemas. Nos seus livros, o *Tio Bob* trata tudo de uma forma muito preto no branco, e isso, durante minha trajetória na programação, me gerou muitos problemas.

Era muito comum que os desenvolvedores quisessem sempre fazer as melhores classes, as classes mais abstratas possíveis, fazer coisas extremamente desacopladas, quando tínhamos *recursos limitados* de *tempo* e *dinheiro*. Isso fazia com que todos os projetos e manutenções gerassem *prejuízos*.

Elevar a complexidade de um projeto com a implementação de padrões *não traz mais qualidade para o código*, mas sim, apenas mais complexidade.

Dito isso, sabendo que borracharia do Sr. Abel não vai virar, em 1 ano, um super e-commerce, neste exato momento, eu trabalho em uma das maiores empresas de tecnologia brasileiras.

Como os problemas se tornam cada vez mais complexos e de tamanho gigantesco, o código legado fica legado ainda mais rápido, caso não sejam utilizados padrões para a escrita do código.

Dito isso, dentro do meu *PDI*, meu gestor pediu para que eu mergulhasse de cabeça nesse assunto.

Então, respondendo as perguntas do meu primeiro dia de estudos.

### O que são Design Patters?

É um conjunto de formas de escrita de código orientado a objetos, para facilitar a manutenção e o crescimento do código, baseado em algumas situações corriqueiras de representação do nosso universo em um código, com problemas já conhecidos de arquitetura e desafios comuns a diferentes tipos de cenários.

Dominando esses padrões, é bem provável que você consiga resolver qualquer problema de programação de forma elegante, rápida e sustentável.

## Tipos de padrões

Já conhecia os tipos de padrões: *Criacionais*, *Estruturais* e *Comportamentais*. No artigo de [introdução aos Design Patterns do Refactor Guru](https://refactoring.guru/pt-br/design-patterns/what-is-pattern) (_site que eu já conhecia e de vez em quando dava um pulinho lá_), ele explica bem por que esses padrões existem, quem os criou e cita um exemplo bem legal, que foi onde me encontrei durante muito tempo.

"É provável que você passe a vida inteira sem saber o que são padrões de projeto, porém, você já deve estar utilizando alguns deles no seu dia a dia". Como disse o [Jovem Tranquilão](https://www.youtube.com/@JovemTranquil%C3%A3o) em um dos seus vídeos, quando você estuda padrões de projeto, você simplesmente dá um nome para algo que você já pratica há muito tempo e isso facilita a sua comunicação com outras pessoas durante o desenvolvimento.

Como parte de consolidação dos meus estudos, irei explicar como já utilizo, alguns padrões.

### Criacional: Builder

Como trabalhei muito tempo com *WordPress*, uma bala de prata para quem trabalha no dia a dia da ferramenta é o *ACF (Advanced CUstom Fields)*. Apenas utilizar esse cara na versão do painel, é bom, porém não te traz capacidade de controlar os campo corretamente, nem de versionalos com facilidade.

Para isso, foi criada uma biblioteca chamada *ACF Builder*, que ela literalmente transformou o código PHP do *ACF* em uma *classe builder*, onde você vai construindo os campos e depois renderiza tudo de uma vez.

### Estrutural: Proxy

Esses padrões, acredito que tenham sido os que menos utilizei concientemente, porém, como se tratam de estruturas, em algum momento você com toda certeza já utilizou esses padrões.

Um que é relativamente simples, é o padrão de *Proxy*, pois em diversos momentos, quando você recebe uma requisição, você faz várias mágicas, de forma invisível para o usuário, para executar algo, nem que seja um _redirect_.

Então, esse padrão na teoria, nunca deixa a requisição chegar diretamente no destinho final, como uma requisição, que acessar uma classe, que tem acesso direto ao banco. Não, você não faz isso, você normalmente coloca uma camada entre o banco de dados e o que você está retornando, seja um *repository*, um *model*, nos conceitos de alguns frameworks, ou qualquer outra coisa. Isso, é um *Proxy*.

Um exemplo simples, utilizando o próprio *WordPress*, é a função `WP_Query`, que faz um proxy entre sua consulta e o banco de dados.

## Link para download do livro

Download do livro no repositório [ICMC-USP](https://github.com/ropalma/ICMC-USP/blob/master/Book%20-%20Padr%C3%B5es%20de%20Projeto%20-%20Soluc%C3%B5es%20Reutiliz%C3%A1veis%20de%20Software%20Orientado%20a%20Objetos.pdf).
