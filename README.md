# Caderno virtual - Lógica da Programação e Algoritmos



## Conteúdo Técnico

## Switch
Switch: Estrutura de controle que permite escolher entre várias opções baseadas no valor de uma variável.

## String
String: Tipo de dado que representa uma sequência de caracteres, como texto.

## Number
Number: Tipo de dado que representa valores numéricos, sejam inteiros ou decimais.

## Prompt
Prompt: Função usada para exibir uma caixa de diálogo que solicita a entrada de dados do usuário.
`js

## Boolean
Boolean: Tipo de dado que pode ter apenas dois valores: true (verdadeiro) ou false (falso).
`js




## Atividades desenvolvidas
1

const livros = ["Javascript", "mongodb", "Node", "NodeJS", "HTML"] 
const Atualizar = livros.splice(0, 2, "css") 

console.log(Atualizar) 
console.log(livros)

const tamanho = livros.length

console.log(tamanho)

const corredorA1 = livros.slice(0, tamanho/2)
const corredorA2 = livros.slice(tamanho/2)

console.log("Os livrros do corredor A1, são: " + corredorA1)
console.log("Os livros do corredor A2, são: " + corredorA2)

2

const frutas = ["Maçã", "Cereja", "Laranja", "Melancia", "Cajá"];

console.log(frutas.pop(4));
console.log(frutas.push("Cajú"));
console.log(frutas.length);

3

const livros = ["Javascript","ECMAScript", "MongoDB","Meridiano de Sangue","O escaravelho do diabo","A piada mortal","Hellsing"];
console.log(livros[2]);
let consulta = livros.indexOf("MongoDB")
console.log(consulta)

console.log(livros.pop());

console.log(livros.push("NovoLivro"));

console.log(livros)

console.log(livros.sort());

console.log(livros.length);

4

const remédio = prompt("Qual remédio você deseja comprar?")

switch(remédio){
  case "Zydus":
    console.log(`O remédio ${remédio} custa R$3,90.`)
    break;
    case "Pharlab":
  case "Teuto":
  case "Caverdilol":
    console.log(`O remédio ${remédio} custa R$2,24.`)
    break;
    case "Paracetamol":
    console.log(`O remédio ${remédio} custa R$10,40.`)
    break;
  default:
    console.log('O remédio não está disponível.')
}
const bairro = prompt('Em qual bairro você mora?')
switch(bairro){
  case "Jardim São Paulo":
  case "Boa Viagem":
    console.log(`A entrega para ${bairro} vem com uma taxa de R$10,00` )
}

5

const produto = prompt("Qual produto você deseja comprar?")

switch(produto){
  case "Miojo":
    console.log(`O produto ${produto} custa R$3,50.`)
    break;
    case "Maçã":
  case "Biscoito treloso":
    console.log(`O produto ${produto} custa R$1,50 por unidade.`)
    break;
  default:
    console.log('O produto não está disponível.')
}

6

const produto = prompt('Qual fruta você deseja comprar?')

switch(produto) {
  case "Laranja":
    console.log("Laranja custa R$5,00")
    break;
  case "Morango":
    console.log("Morango custa R$10,00")
    break;
  default:
    console.log("Lamento, essa fruta não está disponível.")
}

7

const nome = prompt('Qual o seu nome?')
const nota1 = prompt('Insira a nota de Potuguês')
const nota2 = prompt('Insira a nota de História')
const nota3 = prompt('Insira a nota de Química')
const nota4 = prompt('Insira a nota de Geografia')
const nota5 = prompt('Insira a nota de Inglês')

const média = (parseInt(nota1) + parseInt(nota2) + parseInt(nota3) + parseInt(nota4) + parseInt(nota5)) / 5

if(média >= 7){
  console.log(`Parabéns, ${nome}! Você está aprovado(a).`)
} else if (média < 7 && média >= 4 ){
  console.log(`Atenção, ${nome}! Você está em recuperação`)
}

const senha = prompt("Qual é a senha?")
const senhaSecreta = "mediotec"


if(senha == senhaSecreta){
  console.log('Pode entrar!')
} else{
  console.log('Errou o lugar, viu.')
}
