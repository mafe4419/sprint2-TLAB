# DESAFIO TYPESCRIPT

Use esse espaço para responder às questões teóricas:

## Instruções
Para executar o projeto, primeiro rode o comando: ```npm i``` para baixar as dependências do projeto.

A função `uuidv4` serve apenas para gerar uma string que será usada como o id quando necessário.

Para compilar e rodar o projeto você primeiro deve executar o comando `npx tsc` para transformar os arquivos `.ts` em `.js`.
Depois disso, os arquivos compilados estarão na pasta `dist`. Para executar, basta executar o seguinte comando: `node ./dist/index.js`.

Decerto algumas dúvidas irão surgir. Não se desespere, tome um ar, tente resolver com calma as questões, e, caso se veja sem saída, peça ajuda :).

## Questões teóricas

- [ ] O que exatamente é o Typescript?
É uma ferramenta orientada a objetos e visa aumentar a produtividade do código. Ela vai um pouco além do javascript, já que possui a possibilidade de programar tanto do lado do cliente quanto do lado do servidor (tipagem estática) e também adiciona outros recursos como interfaces, classes, herança e módulos.

- [ ] Descreva os tipos básicos do Typescript.
Possui 7 tipos básicos. Um tipo é um conjunto de valores.
**Undefined:** conjunto com um elemento indefinido, ou seja, ainda não recebeu um valor;
**Null:** conjunto com um elemento vazio;
**Boolean:** conjunto com dois elementos: false ou true;
**Number:** conjunto de todos os números;
**String** conjunto de textos;
**Symbols:** conjunto de todos os símbolos;
**Objects:** conjunto de todos os objetos, como funções e arrays. Arrays são tipos especiais que podem guardar vários valores de diferentes tipos de dados sequencialmente, usando uma sintaxe específica.


- [ ] O que é uma interface?
De forma simples, descreve a estrutura de um objeto, de uma classe ou de uma função, ou seja, descreve como devem se parecer.

- [ ] O que é uma classe?
Uma classe permite criar representações do mundo real para o código, nela você atribui valores de diferentes tipos como sendo características daquela classe. Obrigatoriamente, toda classe deve começar com letra maíuscula.
Exemplo:
   class Carro{
        marca: string;
        seats: number;
        doors: number;
   }

- [ ] O que é a herança?
Heranças são usadas para criar uma classe a partir de outra já existente. A classe existente é chamada de Base e a criada a partir dela é chamada de Derivada. A palavra que permite essa relação é a "extends".
Exemplo:
    class Carro extends Pneu {
        marca: string;
        diametro: number;
    }
  
- [ ] Quais as vantagens de usar o Typescript ao invés de somente o Javascript?
TS mostra os erros no durante a organização, JS apenas na execução. O TS oferece composição estática discricionária: os tipos de TS podem ser adicionados a fatores, capacidades, propriedades e assim por diante. O TS é executado em qualquer programa ou motor JS. TS ajuda na organização do código. O TS tem uma documentação melhor para APIs que está em um estado de harmonia com o código-fonte, algumas organizações relatam uma diminuição nos bugs quando mudam para o TS.

## Questões práticas
- [ ] Agora que você é bem familiarizado com o Typescript, vamos criar um simples projeto: <br>
Primeiro, clone o repositório anexado em sua máquina;
Como deve ter notado, na pasta `src` temos uma pasta `model` e um arquivo `index.js`. Por enquanto apenas guarde essas informações;

- [ ] Comece pelo arquivo `users.js` na pasta `models`. Nele, você deverá adicionar tipagem para as funções e também para o user. Antes de mais nada renomeie o arquivo para `users.ts`. Um user possui os seguintes atributos: `id`, `name`, `age` e `email`. Use de seu conhecimento na criação de interfaces para resolver esta questão;
  
- [ ] Agora, indo para o arquivo `bankAccount.js` na pasta `models`, você deverá adicionar tipagem para as funções e também para a bankAccount. Como na questão anterior, renomeie o arquivo para `bankAccount.ts`. Nessa questão você deverá identificar quais são os atributos da bankAccount de acordo com o que há disponível nas funções. De novo, use seus conhecimentos sobre interfaces e typescript para resolver a questão.

- [ ] Após ter feito a tipagem dos arquivos da pasta `models` é hora de resolver os erros do arquivo `index.js`. Comece trocando sua extensão para `index.ts`. Você logo verá que alguns erros estão acontecendo. Antes não seria possível identificá-los, pois nenhum dos arquivos possuía tipagem. O que você precisa fazer agora é basicamente corrigir os erros de acordo com o que o intellisense do seu editor de códigos indicar. 

- [ ] Com os erros resolvidos, precisamos apenas testar o código e executar a função de `withdraw` e a função de `deposit` da `bankAccount`. Para isso, primeiro deposite a quantia de 1000 unidades monetárias (um) e faça um saque de 200um. Para verificar se deu tudo certo, use a função `getBankAccountInfo` e dê um `console.log` na conta obtida.

## Desafio extra
- [ ] Refatore o projeto, mas usando classes para criar os `users` e as `bankAccounts`;