# Projeto: Compilador Mips
Desenvolvendo um compilador MIPS em que pode compilar diversas linguagens

Introdução:

Criar um compilador MIPS capaz de aceitar várias linguagens de entrada é um grande desafio no mundo da programação de baixo nível e da arquitetura de computadores. A inspiração para este projeto surgiu durante o estudo da linguagem assembly MIPS na disciplina de Arquitetura de Computadores II, do curso de Ciência da Computação.

A linguagem assembly MIPS é conhecida por ser simples e muito eficiente, mas a transição do código de alto nível para o assembly pode ser desafiadora. No entanto, esta dificuldade é o que torna esse projeto tão interessante. Imagine ser capaz de traduzir código C aparentemente complexo em código assembly MIPS com facilidade, como no exemplo a seguir:

```C
int x = 2;
int y = 3;
int z = x + y;
```
Assembly:
```
#associações:
# x -> $s0
# y -> $s1
# z -> $s2

.text
.globl main
main:			
	ori $s0, $zero, 2 # x = 2
	ori $s1, $zero, 3 # y = 3
	add $s2,$s0,$s1	  # z = x + y
```
É claro que para isso, teria que aprender como um compilador funciona e os tipos de análises que devo ter para entender como a linguagem funciona. Desse modo nesse github vou colocar o que estou aprendendo e metas futuras para entregar esse projeto com êxito.
