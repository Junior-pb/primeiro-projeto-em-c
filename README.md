# primeiro-projeto-em-c

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main (){

	setlocale(LC_ALL, "");

	//1 - Crie um Menu. O menu deverá ter opções quaisquer de 0 a 9, se o usuário digitar algum número entre 1 e 9, o programa deverá reexibir o menu.

Caso o usuário digitar qualquer outro número, com excessão do 0, o programa deve informar que a opção desejada é inexistente.

E por fim, caso o usuário digitar 0, o programa deve exibir mensagem de despedida e terminar sua execução.
	
	int x;
	
	printf("Escolha um número inteiro de 0 a 9:\n");
	//exibir o menu
	scanf("%d", &x);	
	//colher o numero do usuario
	
	while (x >= 1 && x <= 9){
	//se for um número entre 1-9, retornar ao menu		
		printf("Escolha um número inteiro de 0 a 9:\n");
		scanf("%d", &x);
	}
	if (x == 0){
	//se zero dê xau
		printf("Adeus, o programa foi encerrado.");
	}
	if (x <0 || x > 9){
	//se != 1-9, diga inexistente
		printf("A opção desejada é inexistente");
    }	
	return 0;
}

