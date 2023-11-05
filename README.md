# Projeto-Compilador-Mips
Criar um compilador MIPS, em que ele aceitará várias linguagens de entrada e deverá entregar um compilador MIPS correspondente a linguagem

Bom, essa ideia surgiu qunaod comecei a ver a matéria sobre assembly MIPS na matéria de Arquitetura de computadores II no curso de Ciência da computação.

Assim que comecei a ver, me encantei imadiatamente com a possibilidade de transformar um simples código como:

```C
int x = 2
int y = 3
int z = x + y
```
Em assembly MIPS: 
``` Assembly
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
