
# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(a,b){ return a + b;}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var soma2 = soma(5,5) + 5;

// Qual o valor atualizado dessa variável?
15;

// Declare uma nova variável, sem valor.
var c;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function Adiciona_Valor(valor1){ 
    valor1 = 10;
    return "O valor da variável agora é " + valor1;
}

// Invoque a função criada acima.
Adicionar_Valor(c);

// Qual o retorno da função? (Use comentários de bloco).
O valor da variável agora é 10

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function Multiplicacao_soma(a,b,c){
    if(typeof(a) == "number" && typeof(b) == "number" && typeof(c) == "number"){
        return ( a * b * c ) + 2;
    }else{ return 'Preencha todos os valores corretamente!';}
}

// Invoque a função criada acima, passando só dois números como argumento.
Multiplicacao_soma(2,3);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
Preencha todos os valores corretamente!

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
Multiplicacao_soma(1,2,3);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
8

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function TesteComArgumentos(a,b,c){
    if(typeof(a) === "number" && isNaN(b) && isNaN(c)){
        return (a);
    } else if(typeof(a) === "number" && typeof(b) === "number" && isNaN(c)){
        return a + b;
    } else if(typeof(a) === "number" && typeof(b) === "number" && typeof(c) === "number"){
        return (a + b) / c;
    } else if(typeof(a) == "undefined" && typeof(b) == "undefined" && typeof(c) == "undefined" ){
        return false;
    } else { return null}
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
TesteComArgumentos(1);
TesteComArgumentos(1,2);
TesteComArgumentos(1,2,3);
TesteComArgumentos();
TesteComArgumentos(undefined,true,'nome')
```
