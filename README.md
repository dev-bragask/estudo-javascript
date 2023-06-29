# Estudo-JavaScript
Estudo básico sobre JavaScript. Contem os seguintes tópicos: armazenamento de dados, variáveis, operadores, condições, repetições, array, funções e DOM .

## O que é JavaScript?
JavaScript é uma linguagem de programação utilizada para criar interatividade em páginas da web. Ela permite que os desenvolvedores criem aplicativos e sites mais dinâmicos, com recursos como animações, validação de formulários, efeitos visuais, jogos e muito mais.

Originalmente criada em 1995 pela Netscape, hoje em dia, o JavaScript é amplamente utilizado em todo o mundo em desenvolvimento web, e é suportado por todos os principais navegadores, incluindo o Google Chrome, Firefox, Safari e Internet Explorer. Ele é uma linguagem de programação orientada a objetos, com recursos como variáveis, funções, loops e condicionais, e também tem suporte para manipulação de eventos, AJAX e APIs. Com o JavaScript, é possível criar aplicações tanto do lado do cliente quanto do lado do servidor, utilizando plataformas como Node.js.


## **Armazenamento Dados**
Em JavaScript, `"number"` e `"string"` são tipos de dados fundamentais que são usados para armazenar diferentes tipos de informações.

Um `"number"` (número) é usado para armazenar valores numéricos, como inteiros e números de ponto flutuante. Esses valores podem ser usados em operações matemáticas, como adição, subtração, multiplicação e divisão. Por exemplo: 

    let x = 10

Uma `"string"` (cadeia de caracteres) é usada para armazenar texto, como nomes, frases ou parágrafos. As strings são delimitadas por aspas simples ('') ou aspas duplas (""). Por exemplo: 

    let nome = "Nícolas"

- **Number()** = É uma função que converte um valor em um número. 

    `Number.parseFloat()` = É um método que é usado para converter uma string em um número de ponto flutuante (Quebrado). Atravez desse método o javascript vai receber valores de número quebrado.
    
    `Number.parseInt()` =  É um método que é usado para converter uma string em um número inteiro. Atravez desse método o javascript vai receber valores de número inteiro.
    
    `.toFixed()` = É um método que é usado para formatar um número como uma string com um número específico de casas decimais.  <br/>
    
    `.replace()` = É um método que é usado para substituir uma parte de uma string por outra. Ele retorna uma nova string que é criada substituindo a parte da string original que corresponde a um padrão especificado por outra string ou valor.
    
- **String() =** É uma função que converte um valor em uma String.

    `.toSting()` = É um método que converte um valor em uma String, só que no final do código.
    
    `.length()` = Retorna o número de caracteres na string (tamanho da string).
    
    `.toUpperCase()` = É um método que retorna uma nova string com todos os caracteres em maiúsculo.
    
    `.toLowerCase()` =  É um método que retorna uma nova string com todos os caracteres em minúsculo.
    
    `.toLocaleString()` =  É um método que retorna uma string com o valor numérico formatado de acordo com a localidade do usuário. 
    
    Por exemplo: 
    
        .toLocaleString('pt-BR' ,{style: 'currency' , currency: 'BRL'})
    
## **Variável**

Variáveis em JavaScript são usadas para armazenar dados e informações em um programa. Uma variável é um nome simbólico que faz referência a um valor armazenado na memória do computador.

Em JavaScript, as variáveis podem ser declaradas usando as palavras-chave var, let ou const. A diferença entre essas palavras-chave é a forma como as variáveis são declaradas e como elas podem ser usadas posteriormente.

É importante lembrar que as variáveis declaradas com const não podem ter seu valor atualizado posteriormente. Já as variáveis declaradas com let e var podem ser atualizadas posteriormente, mas com algumas diferenças importantes no escopo. Variáveis declaradas com let têm escopo de bloco, enquanto as variáveis declaradas com var têm escopo de função ou global.

- **Template strings**

Ao contrário das strings tradicionais em JavaScript, que são definidas com aspas simples ou duplas, as template strings são definidas com backticks (``). Isso permite a inclusão de variáveis e expressões dentro da string usando a sintaxe ${ } dentro das backticks.


## **Operadores**

- Aritméticos <br/>
    5 + 2 = 7 (soma) <br/> 
    5 - 2 = 3 (subtração) <br/>
    5 * 2 = 10 (multiplicação) <br/>
    5 / 2 = 2.5 (divisão) <br/>
    5 % 2 = 1 (divisão inteira/resto da divisão) <br/>
    5 ** 2 = 25 (potencia) <br/>
    
- Relacionas <br/>
    |  > maior <br/>
    |  < menor <br/>
    |  >= maior e igual <br/>
    |  <= menor e igual <br/>
    |  == comparação <br/>
    |  != diferente <br/>
    
- Lógicos <br/>
    | ! negação <br/>
    | - && conjunção ex:
    
        const a = 3;
        const b = -2;
    
        console.log(a > 0 && b < 0);
    
    Os dois valores tem que ser verdadeiros para aparecer true.
    
    | - || disjunção ex:
    
        const a = 3;
        const b = -2;
    
        console.log(a > 0 || b > 0);
    
    Apenas um dos valores precisa ser verdadeiro.
    
- Auto atribuições  <br/>
    | n = 3 <br/>
    | n += 5 (8)
    
- Incremento  <br/>
    | x ++ (x+=)
    
    O operador de incremento é representado pelo símbolo ++ e é usado para adicionar 1 ao valor de uma variável. Existem duas formas de usar o operador de incremento: o operador pode ser colocado antes da variável ou depois da variável.
    
- Identidade <br/>
    | 5 == 5 true <br/>
    | 5 == ‘5’ true <br/>
    | 5 === ‘5’ false  
    | 5 === 5 true <br/>
    | 0 mesmo acontece com o !== 
    
- Ternário <br/>
    | Media >= 7 ? “aprovado” : “reprovado” <br/>

    O operador ternário é uma forma compacta de escrever uma estrutura condicional simples em uma única linha. Ele é representado pelo símbolo ? e : e possui a seguinte sintaxe:` <br/>
    condição ? valor se verdadeiro : valor se falso
    
## **Condições**
As condições são usadas para executar diferentes ações com base em diferentes condições. Existem duas maneiras de criar uma condição em JavaScript: usando a instrução if e a instrução switch.
    
    Condição simples = If(condição){ } 
    Condição complexa = if(condição){ }else{ } 
    Condição aninhadas = uma condição dentro da outra. (Else if)  
    Condição múltiplas = valor fixo (switch(expressão){valor_break})
    
    exemplo :
    let idade = 18;

    if (idade >= 18) {
      console.log("Você é maior de idade.");
    } else {
      console.log("Você é menor de idade.");
    }
    
Neste exemplo, estamos verificando se a variável idade é maior ou igual a `18`. Se for verdadeira, o código dentro do bloco if será executado, caso contrário, o código dentro do bloco else será executado. No caso, como a variável idade é igual a `18`, o código dentro do bloco if será executado e a mensagem "Você é maior de idade." será impressa no console.


## **Repetições**

As repetições em JavaScript são usadas para executar um bloco de código várias vezes. Existem duas maneiras principais de criar uma repetição em JavaScript: usando a instrução `for` e a instrução `while`.

A instrução `for` é usada para executar um bloco de código um número específico de vezes. A instrução `while` é usada para executar um bloco de código enquanto uma condição específica for verdadeira.

    while(condição){ }
    do{ }while(condição)
    for(incio;testeLogico;incremento;){ }
    for(variável in Array){ }
    
    exemplos: 
    
    for (let i = 1; i <= 5; i++) {
      console.log(i);
    }
    
    let j = 0;
    while (j <= 10) {
      console.log(j);
      j += 2;
    }
    
    
No primeiro exemplo, estamos usando a instrução for para imprimir os números de `1` a `5`. A variável i é inicializada como `1`, e o bloco de código dentro do for é executado enquanto i for menor ou igual a `5`. A cada iteração, a variável i é incrementada em `1`, e o número correspondente é impresso no console.

No segundo exemplo, estamos usando a instrução while para imprimir os números pares de `0` a `10`. A variável `j` é inicializada como `0`, e o bloco de código dentro do while é executado enquanto `j` for menor ou igual a `10`. A cada iteração, a variável `j` é incrementada em `2` (para imprimir apenas números pares), e o número correspondente é impresso no console.

## **Array**

Um array é uma estrutura de dados que armazena múltiplos valores em uma única variável. Ele é uma forma de agrupar dados relacionados. Veja como trabalhar com arrays em JavaScript:

    const array = []; // Array vazio
    const numeros = [1, 2, 3, 4, 5]; // Array com valores
    const frutas = ['maçã', 'banana', 'laranja']; // Array de strings

    let num = [0,1]
    num[2]=6
    A saída será: [0, 1, 6]
    Agora o array num possui três elementos, sendo 0 no índice 0, 1 no índice 1 e 6 no índice 2.

    num.push(7) = adiciona um novo elemento ao final do array, expandindo-o automaticamente. 
    No caso acima, o número 7 é adicionado como o último elemento do array num.
    A saída será: [0, 1, 7]
  
    num.length = tamanho do array  
    console.log(num.length);
    A saída será: '3'

    num.sort() = coloca os valores do array em ordem crescente
    num.indexOf(2) = procura no array um determinado valor valor
    A saída será: 7
    
## **Funções**

As funções são blocos de código que podem ser definidos e reutilizados para executar uma tarefa específica. Elas ajudam a organizar e modularizar o código, tornando-o mais legível e fácil de manter. Aqui estão algumas características e exemplos de como trabalhar com funções em JavaScript:

    function nomeDaFuncao(parametro1, parametro2) {
      // Bloco de código da função
    }

    nomeDaFuncao(argumento1, argumento2); = chamada da função

Esses são apenas alguns conceitos básicos sobre funções em JavaScript. As funções têm uma ampla variedade de recursos e podem ser usadas de várias maneiras para manipular dados, executar tarefas e interagir com outros elementos do código. Elas são uma parte fundamental da linguagem JavaScript.


## **DOM = Document Object Model (Modelo de Objeto de Documento)**

É uma interface de programação em JavaScript que representa a estrutura do documento HTML ou XML em forma de uma árvore de objetos. O DOM permite que os programadores acessem e manipulem os elementos e conteúdos de um documento web de forma dinâmica.

Quando uma página da web é carregada em um navegador, o navegador cria uma representação interna do documento usando o DOM. Essa representação é organizada hierarquicamente, onde cada elemento do documento (como tags HTML) é representado por um objeto. Esses objetos podem ser manipulados e atualizados usando JavaScript para alterar dinamicamente o conteúdo, a aparência e o comportamento da página.

Com o DOM, é possível acessar e modificar elementos individuais, adicionar ou remover elementos, alterar atributos e estilos, além de lidar com eventos, como cliques e submissões de formulários. O DOM fornece uma maneira poderosa e flexível de interagir com os elementos de uma página da web e criar experiências interativas e dinâmicas para os usuários.


## **Acessando elementos usando seletores.**

Em JavaScript, existem vários métodos que retornam um HTMLCollection de elementos com base no nome da tag fornecido. Esses métodos permitem selecionar elementos específicos do documento com base em sua tag HTML. Aqui estão alguns dos principais métodos:

**1- querySelector():** O método é uma poderosa função do DOM que permite selecionar elementos com base em um seletor CSS especificado. Ele retorna o primeiro elemento que corresponde ao seletor fornecido.

    const elemento = document.querySelector('.classe-do-elemento');
    
Nesse exemplo, o método procura pelo primeiro elemento que possui a classe CSS "classe-do-elemento" e retorna esse elemento. Se nenhum elemento for encontrado, o valor retornado será null.

**2- querySelectorAll():** Este método retorna uma NodeList de elementos que correspondem a um seletor CSS especificado. Você pode passar o nome da tag como seletor para selecionar todos os elementos correspondentes a essa tag. Por exemplo:

    const elementos = document.querySelectorAll('div');
        
Isso retornará uma NodeList com todos os elementos `<div>` encontrados no documento.

**3- getElementsByName():** O método retorna uma NodeList de elementos com o atributo `name` especificado. No entanto, é importante observar que esse método funciona apenas para certos elementos específicos, como `input`, `select` e `textarea`. Por exemplo: 

    const elementos = document.getElementsByName('nome-do-elemento');

Isso retornará uma NodeList contendo todos os elementos com o atributo `name` igual a "nome-do-elemento".


**4- getElementsByTagName():** Esse método retorna uma HTMLCollection de elementos com o nome da tag especificada. Ele permite selecionar elementos por seu nome de tag diretamente. Por exemplo:

    const elementos = document.getElementsByTagName('div');

Isso retornará uma HTMLCollection com todos os elementos `<div>` encontrados no documento.

**5- getElementsByClassName():** Este método retorna uma HTMLCollection de elementos com a classe CSS especificada. Embora não se baseie diretamente no nome da tag, ele pode ser usado para selecionar elementos com base em uma classe comum. Por exemplo:

    const elementos = document.getElementsByClassName('minha-classe');

Isso retornará uma HTMLCollection com todos os elementos que possuem a classe CSS "minha-classe".

**6- getElementById():** O método é usado para retornar um elemento do DOM com base no valor do atributo id fornecido. Ao contrário dos métodos mencionados anteriormente, getElementById() retorna apenas um único elemento em vez de uma coleção.

    const elemento = document.getElementById('meu-elemento');
    
Nesse exemplo, o método procura por um elemento com o atributo id igual a "meu-elemento" e retorna esse elemento. Se nenhum elemento for encontrado com o id especificado, o valor retornado será null.

Esses métodos são úteis quando você deseja selecionar elementos específicos do documento com base em seu nome de tag. É importante observar que tanto `querySelectorAll()` quanto `getElementsByTagName()` retornam coleções estáticas, o que significa que, se elementos adicionais forem adicionados ao documento posteriormente, eles não serão automaticamente incluídos na coleção. Se você precisar lidar com uma coleção dinâmica que inclua novos elementos, é necessário atualizar a coleção manualmente.

## **Eventos DOM**

Eventos no DOM (Document Object Model) são ações ou ocorrências que acontecem em elementos HTML e desencadeiam a execução de código JavaScript. Eles permitem que os desenvolvedores respondam a interações do usuário, como cliques em botões, digitação em campos de formulário, movimentos do mouse, entre outros.

Quando um evento ocorre em um elemento HTML, o navegador dispara o evento e pode executar uma função JavaScript associada a ele, conhecida como manipulador de eventos. Os manipuladores de eventos são responsáveis por definir o comportamento que deve ocorrer quando o evento é acionado.

Existem muitos tipos de eventos DOM disponíveis, como:

- **Eventos de mouse:** ocorrem quando o usuário interage com o mouse, como `click`, `mouseover`, `mouseout`, etc.

- **Eventos de teclado:** ocorrem quando o usuário interage com o teclado, como `keydown`, `keyup`, etc.

- **Eventos de formulário:** ocorrem quando o usuário interage com elementos de formulário, como `submit`, `change`, etc.

- **Eventos de foco:** ocorrem quando um elemento ganha ou perde o foco, como `focus`, `blur`, etc.

- **Eventos de carregamento:** ocorrem quando a página ou um recurso é carregado, como `load`, `DOMContentLoaded`, etc.

Para associar um manipulador de eventos a um elemento HTML, você pode usar métodos como `addEventListener`, onde especifica o tipo de evento e a função a ser executada quando o evento ocorrer. O manipulador de eventos recebe um objeto de evento como argumento, que fornece informações sobre o evento e o elemento associado.

Os eventos no DOM desempenham um papel fundamental na criação de interatividade em páginas da web, permitindo que os desenvolvedores respondam e ajam com base nas ações dos usuários, tornando as aplicações mais dinâmicas e responsivas.
