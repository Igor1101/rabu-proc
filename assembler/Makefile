
all: lex yac compile


lex:
	lex lexer.lex 

yac:
	yacc -d grammar.yac 

compile:
	gcc -O2 -Wno-implicit-function-declaration -o ex lex.yy.c y.tab.c -lfl
	./ex example.asm out.txt

debug:
	gcc -O2 -DYYDEBUG -Wno-implicit-function-declaration -o ex lex.yy.c y.tab.c -lfl 

