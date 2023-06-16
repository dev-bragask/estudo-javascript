# Estudo-JavaScript
Estudo básico sobre JavaScript, armazenamento de dados, operadores, DOM, funções, condições, repetições e array.

## O que é JavaScript?
JavaScript é uma linguagem de programação utilizada para criar interatividade em páginas da web. Ela permite que os desenvolvedores criem aplicativos e sites mais dinâmicos, com recursos como animações, validação de formulários, efeitos visuais, jogos e muito mais.

Originalmente criada em 1995 pela Netscape, hoje em dia, o JavaScript é amplamente utilizado em todo o mundo em desenvolvimento web, e é suportado por todos os principais navegadores, incluindo o Google Chrome, Firefox, Safari e Internet Explorer. Ele é uma linguagem de programação orientada a objetos, com recursos como variáveis, funções, loops e condicionais, e também tem suporte para manipulação de eventos, AJAX e APIs. Com o JavaScript, é possível criar aplicações tanto do lado do cliente quanto do lado do servidor, utilizando plataformas como Node.js.


## **Armazenamento Dados**
Em JavaScript, "number" e "string" são tipos de dados fundamentais que são usados para armazenar diferentes tipos de informações.

Um "number" (número) é usado para armazenar valores numéricos, como inteiros e números de ponto flutuante. Esses valores podem ser usados em operações matemáticas, como adição, subtração, multiplicação e divisão. Por exemplo: **let x = 10**.

Uma "string" (cadeia de caracteres) é usada para armazenar texto, como nomes, frases ou parágrafos. As strings são delimitadas por aspas simples ('') ou aspas duplas (""). Por exemplo: **let nome = "Nícolas"**.

- **Number()** = É uma função que converte um valor em um número. 

    Number.parseFloat() = É um método que é usado para converter uma string em um número de ponto flutuante (Quebrado). Atravez desse método o javascript vai receber valores de número quebrado.
    
    Number.parseInt() =  É um método que é usado para converter uma string em um número inteiro. Atravez desse método o javascript vai receber valores de número inteiro.
    
    .toFixed() = É um método que é usado para formatar um número como uma string com um número específico de casas decimais.  <br/>
    
    .replace() = É um método que é usado para substituir uma parte de uma string por outra. Ele retorna uma nova string que é criada substituindo a parte da string original que corresponde a um padrão especificado por outra string ou valor.
    
- **String() =** É uma função que converte um valor em uma String.

    .toSting() = É um método que converte um valor em uma String, só que no final do código.
    
    .length() = Retorna o número de caracteres na string (tamanho da string).
    
    .toUpperCase() = É um método que retorna uma nova string com todos os caracteres em maiúsculo.
    
    .toLowerCase() =  É um método que retorna uma nova string com todos os caracteres em minúsculo.
    
    .toLocaleString() =  É um método que retorna uma string com o valor numérico formatado de acordo com a localidade do usuário. 
    
    Por exemplo: .toLocaleString('pt-BR' ,{style: 'currency' , currency: 'BRL'})
    
## **Variável**

Variáveis em JavaScript são usadas para armazenar dados e informações em um programa. Uma variável é um nome simbólico que faz referência a um valor armazenado na memória do computador.

Em JavaScript, as variáveis podem ser declaradas usando as palavras-chave var, let ou const. A diferença entre essas palavras-chave é a forma como as variáveis são declaradas e como elas podem ser usadas posteriormente.

É importante lembrar que as variáveis declaradas com const não podem ter seu valor atualizado posteriormente. Já as variáveis declaradas com let e var podem ser atualizadas posteriormente, mas com algumas diferenças importantes no escopo. Variáveis declaradas com let têm escopo de bloco, enquanto as variáveis declaradas com var têm escopo de função ou global.

- Template strings

Ao contrário das strings tradicionais em JavaScript, que são definidas com aspas simples ou duplas, as template strings são definidas com backticks (``). Isso permite a inclusão de variáveis e expressões dentro da string usando a sintaxe ${ } dentro das backticks.



## **Operadores**

- Aritméticos <br/>
    | 5 + 2 = 7 (soma) <br/> 
    | 5 - 2 = 3 (subtração) <br/>
    | 5 * 2 = 10 (multiplicação) <br/>
    | 5 / 2 = 2.5 (divisão) <br/>
    | 5 % 2 = 1 (divisão inteira/resto da divisão) <br/>
    | 5 ** 2 = 25 (potencia) <br/>
    
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
    
    `const a = 3;`
    `const b = -2;`
    
    `console.log(a > 0 && b < 0);`
    
    `Os dois valores tem que ser verdadeiros para aparecer true.`
    
    | - || disjunção ex:
    
    `const a = 3;`
    `const b = -2;`
   
    `console.log(a > 0 || b > 0);`
    
    `Apenas um dos valores precisa ser verdadeiro.`
    
- Auto atribuições  <br/>
    | n = 3 <br/>
    | n += 5 (8)
    
- Incremento  <br/>
    | x ++ (x+=)
    
    `O operador de incremento é representado pelo símbolo ++ e é usado para adicionar 1 ao valor de uma variável. Existem duas formas de usar o operador de incremento: o operador pode ser colocado antes da variável ou depois da variável.`
    
- Identidade <br/>
    | 5 == 5 true <br/>
    | 5 == ‘5’ true <br/>
    | 5 === ‘5’ false  
    | 5 === 5 true <br/>
    | 0 mesmo acontece com o !== 
    
- Ternário <br/>
    | Media >= 7 ? “aprovado” : “reprovado” <br/>
    `O operador ternário é uma forma compacta de escrever uma estrutura condicional simples em uma única linha. Ele é representado pelo símbolo ? e : e possui a seguinte sintaxe:` <br/>
    `condição ? valor se verdadeiro : valor se falso`
    
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
    
Neste exemplo, estamos verificando se a variável idade é maior ou igual a 18. Se for verdadeira, o código dentro do bloco if será executado, caso contrário, o código dentro do bloco else será executado. No caso, como a variável idade é igual a 18, o código dentro do bloco if será executado e a mensagem "Você é maior de idade." será impressa no console.


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
    
    
No primeiro exemplo, estamos usando a instrução for para imprimir os números de 1 a 5. A variável i é inicializada como 1, e o bloco de código dentro do for é executado enquanto i for menor ou igual a 5. A cada iteração, a variável i é incrementada em 1, e o número correspondente é impresso no console.

No segundo exemplo, estamos usando a instrução while para imprimir os números pares de 0 a 10. A variável j é inicializada como 0, e o bloco de código dentro do while é executado enquanto j for menor ou igual a 10. A cada iteração, a variável j é incrementada em 2 (para imprimir apenas números pares), e o número correspondente é impresso no console.

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
