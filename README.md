# logica-de-programacao
Exercícios e projetos de lógica com Visualg.

## Lista de exercícios

01_conversor_seno.alg
Descrição: Recebe um ângulo em graus, converte para radianos e calcula o seno usando a função Sen. Mostra o resultado ao usuário.

## algoritmo "conversor_seno"
var
  angulo, s: Real
inicio
  Escreva("Informe um angulo: ")
  Leia(angulo)
  s <- Sen(GraupRad(angulo))
  Escreva("O seno de ", angulo, " é igual a ", s)
fimalgoritmo

## 02_classificacao_triangulo.alg
Descrição: Recebe três lados e verifica se eles formam um triângulo, além de classificar se é equilátero ou escaleno.

algoritmo "classificacao_triangulo"
var
  L1, L2, L3: real
  Eq, Es, tri: logico
inicio
  escreval("Digite o primeiro lado: ")
  leia(L1)
  escreval("Digite o segundo lado: ")
  leia(L2)
  escreval("Digite o terceiro lado: ")
  leia(L3)

  tri <- (L1 < L2 + L3) e (L2 < L1 + L3) e (L3 < L1 + L2)
  Eq <- (L1 = L2) e (L2 = L3)
  Es <- (L1 <> L2) e (L2 <> L3) e (L1 <> L3)

  escreval("Pode formar um triangulo? ", tri)
  escreval("O triangulo e equilatero? ", Eq)
  escreval("O triangulo e escaleno? ", Es)
fimalgoritmo

## 03_numero_par_ou_impar.alg
Descrição: Verifica se um número inteiro informado é par ou ímpar usando o operador Resto.

algoritmo "numero_par_ou_impar"
var
  numero: inteiro
inicio
  escreval("Me fale um numero inteiro para ver se ele é par ou impar")
  escreval("Digite o seu numero: ")
  leia(numero)

  se Resto(numero, 2) = 0 entao
    escreval("Esse número é par")
  senao
    escreval("Esse número é impar")
  fimse
fimalgoritmo

## 04_soma_simples.alg
Descrição: Lê dois números inteiros, soma-os e exibe o resultado.

algoritmo "soma_simples"
var
  N1, N2, S: inteiro
inicio
  Escreva("Informe um numero: ")
  Leia(N1)
  Escreva("Informe outro numero: ")
  Leia(N2)
  S <- N1 + N2
  Escreva("O resultado da soma entre ", N1, " e ", N2, " é igual a ", S)
fimalgoritmo
