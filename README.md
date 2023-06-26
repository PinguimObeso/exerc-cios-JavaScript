# exercícios JavaScript

1. Elabore um algoritmo que leia um número e, se ele for maior do que 20, imprima a metade desse número.
   
  let numero = prompt("Digite um número: ");
  numero = parseInt(numero);
  
  if (numero > 20) {
    let metade = numero / 2;
    console.log("A metade do número é: " + metade);
  }

2. Elabore um algoritmo para testar se uma senha digitada é igual a "Patinho Feio". Se a senha estiver correta, escreva "Acesso permitido"; caso contrário, emita a mensagem "Você não tem acesso ao sistema".

  let senha = prompt("Digite a senha: ");
  
  if (senha === "Patinho Feio") {
    console.log("Acesso permitido");
  } else {
    console.log("Você não tem acesso ao sistema");
  }

3. Elabore um algoritmo que leia dois números inteiros e efetue a adição. Caso o resultado seja maior que 10, imprima-o.

  let numero1 = parseInt(prompt("Digite o primeiro número: "));
  let numero2 = parseInt(prompt("Digite o segundo número: "));
  
  let resultado = numero1 + numero2;
  
  if (resultado > 10) {
    console.log("O resultado da adição é maior que 10: " + resultado);
  }

4. Elabore um algoritmo que indique se um número digitado está compreendido entre 20 e 90, ou não.

  let numero = parseInt(prompt("Digite um número: "));
  
  if (numero >= 20 && numero <= 90) {
    console.log("O número está compreendido entre 20 e 90");
  } else {
    console.log("O número está fora do intervalo de 20 a 90");
  }

5. Elabore um algoritmo que leia dois números e imprima o maior número

  let numero1 = parseInt(prompt("Digite o primeiro número: "));
  let numero2 = parseInt(prompt("Digite o segundo número: "));
  
  if (numero1 > numero2) {
    console.log("O maior número é: " + numero1);
  } else if (numero2 > numero1) {
    console.log("O maior número é: " + numero2);
  } else {
    console.log("Os números são iguais");
  }

6. Elabore um algoritmo que leia dois números e imprima qual é maior e qual é menor.

  let numero1 = parseInt(prompt("Digite o primeiro número: "));
  let numero2 = parseInt(prompt("Digite o segundo número: "));
  
  if (numero1 > numero2) {
    console.log("O maior número é: " + numero1);
    console.log("O menor número é: " + numero2);
  } else if (numero2 > numero1) {
    console.log("O maior número é: " + numero2);
    console.log("O menor número é: " + numero1);
  } else {
    console.log("Os números são iguais");
  }

7. Elabore um algoritmo que leia três números e imprima o menor número.

  let numero1 = parseInt(prompt("Digite o primeiro número: "));
  let numero2 = parseInt(prompt("Digite o segundo número: "));
  let numero3 = parseInt(prompt("Digite o terceiro número: "));
  
  let menor = numero1;
  
  if (numero2 < menor) {
    menor = numero2;
  }
  
  if (numero3 < menor) {
    menor = numero3;
  }
  
  console.log("O menor número é: " + menor);

8. Elabore um algoritmo que leia três números e os imprima em ordem crescente.

  let numero1 = parseInt(prompt("Digite o primeiro número: "));
  let numero2 = parseInt(prompt("Digite o segundo número: "));
  let numero3 = parseInt(prompt("Digite o terceiro número: "));
  
  if (numero1 <= numero2 && numero1 <= numero3) {
    console.log(numero1);
  
    if (numero2 <= numero3) {
      console.log(numero2);
      console.log(numero3);
    } else {
      console.log(numero3);
      console.log(numero2);
    }
  } else if (numero2 <= numero1 && numero2 <= numero3) {
    console.log(numero2);
  
    if (numero1 <= numero3) {
      console.log(numero1);
      console.log(numero3);
    } else {
      console.log(numero3);
      console.log(numero1);
    }
  } else {
    console.log(numero3);
  
    if (numero1 <= numero2) {
      console.log(numero1);
      console.log(numero2);
    } else {
      console.log(numero2);
      console.log(numero1);
    }
  }

9. Elabore um algoritmo que leia três números, obrigatoriamente em ordem crescente, e um quarto número que não siga esta regra. Mostre, em seguida, os quatro números em ordem decrescente.

  let numero1 = parseInt(prompt("Digite o primeiro número (ordem crescente): "));
  let numero2 = parseInt(prompt("Digite o segundo número (ordem crescente): "));
  let numero3 = parseInt(prompt("Digite o terceiro número (ordem crescente): "));
  let numero4 = parseInt(prompt("Digite o quarto número: "));
  
  console.log("Os números em ordem decrescente são:");
  
  console.log(numero4);
  
  if (numero4 >= numero3) {
    console.log(numero3);
    if (numero4 >= numero2) {
      console.log(numero2);
      console.log(numero1);
    } else {
      console.log(numero4);
      console.log(numero2);
      console.log(numero1);
    }
  } else {
    console.log(numero4);
    console.log(numero3);
    console.log(numero2);
    console.log(numero1);
  }

10. Elabore um algoritmo que leia o nome e o peso de duas pessoas e imprima o nome da pessoa mais gorda.

  let nome1 = prompt("Digite o nome da primeira pessoa: ");
  let peso1 = parseFloat(prompt("Digite o peso da primeira pessoa: "));
  
  let nome2 = prompt("Digite o nome da segunda pessoa: ");
  let peso2 = parseFloat(prompt("Digite o peso da segunda pessoa: "));
  
  if (peso1 > peso2) {
    console.log("A pessoa mais gorda é: " + nome1);
  } else if (peso2 > peso1) {
    console.log("A pessoa mais gorda é: " + nome2);
  } else {
    console.log("As duas pessoas têm o mesmo peso");
  }

11. Elabore um algoritmo que leia um número e imprima se ele é par ou ímpar. Obs: Para o número ser par, o resto de sua divisão por dois deve ser zero.
  
  let numero = parseInt(prompt("Digite um número: "));
  
  if (numero % 2 === 0) {
    console.log("O número é par");
  } else {
    console.log("O número é ímpar");
  }

12. Elabore um algoritmo que leia um número e imprima uma das mensagens: é múltiplo de 3 ou não é múltiplo de 3.

  let numero = parseInt(prompt("Digite um número: "));
  
  if (numero % 3 === 0) {
    console.log("O número é múltiplo de 3");
  } else {
    console.log("O número não é múltiplo de 3");
  }

13. Faça um programa que peça uma nota, entre zero e dez. Mostre uma mensagem caso o valor seja inválido e continue pedindo até que o usuário informe um valor válido.

  let nota;
  
  do {
    nota = parseFloat(prompt("Digite uma nota entre zero e dez: "));
  
    if (nota < 0 || nota > 10) {
      console.log("Valor inválido. Digite novamente.");
    }
  } while (nota < 0 || nota > 10);
  
  console.log("Nota válida: " + nota);

14. Faça um programa que leia um nome de usuário e a sua senha e não aceite a senha igual ao nome do usuário, mostrando uma mensagem de erro e voltando a pedir as informações.

  let nomeUsuario;
  let senha;
  
  do {
    nomeUsuario = prompt("Digite o nome de usuário: ");
    senha = prompt("Digite a senha: ");
  
    if (senha === nomeUsuario) {
      console.log("Erro: a senha não pode ser igual ao nome de usuário.");
    }
  } while (senha === nomeUsuario);
  
  console.log("Nome de usuário: " + nomeUsuario);
  console.log("Senha: " + senha);

15. Faça um programa que leia e valide as seguintes informações:
  Nome: maior que 3 caracteres;
  Idade: entre 0 e 150;
  Salário: maior que zero;
  Sexo: 'f' ou 'm';
  Estado Civil: 's', 'c', 'v', 'd';
  Dica: se sua variável é texto, o tamanho dela está armazenado em: texto.length
  
  let nome;
  let idade;
  let salario;
  let sexo;
  let estadoCivil;
  
  do {
    nome = prompt("Digite o nome (maior que 3 caracteres): ");
  } while (nome.length <= 3);
  
  do {
    idade = parseInt(prompt("Digite a idade (entre 0 e 150): "));
  } while (idade < 0 || idade > 150);
  
  do {
    salario = parseFloat(prompt("Digite o salário (maior que zero): "));
  } while (salario <= 0);
  
  do {
    sexo = prompt("Digite o sexo (f - feminino / m - masculino): ");
  } while (sexo !== "f" && sexo !== "m");
  
  do {
    estadoCivil = prompt("Digite o estado civil (s - solteiro(a), c - casado(a), v - viúvo(a), d - divorciado(a)): ");
  } while (estadoCivil !== "s" && estadoCivil !== "c" && estadoCivil !== "v" && estadoCivil !== "d");
  
  console.log("Informações válidas:");
  console.log("Nome: " + nome);
  console.log("Idade: " + idade);
  console.log("Salário: " + salario);
  console.log("Sexo: " + sexo);
  console.log("Estado Civil: " + estadoCivil);

16. Faça um programa que imprima na tela os números de 1 a 20, um abaixo do outro. Depois, modifique o programa para que ele mostre os números um ao lado do outro.

  // Impressão um abaixo do outro
  for (let i = 1; i <= 20; i++) {
    console.log(i);
  }
  
  // Impressão um ao lado do outro
  let numeros = "";
  
  for (let i = 1; i <= 20; i++) {
    numeros += i + " ";
  }
  
  console.log(numeros);

17. Faça um programa que imprima na tela apenas os números ímpares entre 1 e 50.

  for (let i = 1; i <= 50; i++) {
    if (i % 2 !== 0) {
      console.log(i);
    }
  }

18. Faça um programa que receba dois números inteiros e gere os números inteiros que estão no intervalo compreendido por eles.

  let numero1 = parseInt(prompt("Digite o primeiro número: "));
  let numero2 = parseInt(prompt("Digite o segundo número: "));
  
  console.log("Números no intervalo entre " + numero1 + " e " + numero2 + ":");
  
  for (let i = numero1 + 1; i < numero2; i++) {
    console.log(i);
  }



