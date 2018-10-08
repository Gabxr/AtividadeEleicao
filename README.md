#include <stdio.h>

int main()
{
	float a, b, c, d;
	float validos;
	printf("Quantos votos recebeu o candidato A? ");
	scanf("%f", &a);
	printf("Quantos votos recebeu o candidato B? ");
	scanf("%f", &b);
	printf("Quantos votos recebeu o candidato C? ");
	scanf("%f", &c);
	printf("Quantos votos recebeu o candidato D? ");
	scanf("%f", &d);

	validos = a + b + c + d;

	float nulos, brancos;
	float total;
	printf("Quantos foram os votos nulos? ");
	scanf("%f", &nulos);
	printf("Quantos foram os votos brancos? ");
	scanf("%f", &brancos);

	total = validos + nulos + brancos;
	
	float pvalidos;
	pvalidos=(validos*100)/total;		printf("--------------------------------------\n");
	printf("\nO percentual de votos validos eh: %.2f\n",pvalidos);
			printf("--------------------------------------\n");
	printf("Percentual de votos de cada candidato: \n");
	float pa,pb,pc,pd;
	pa=(a*100)/total;
	pb=(b*100)/total;
	pc=(c*100)/total;
	pd=(d*100)/total;
	
	printf("A: %.2f\n",pa);
	printf("B: %.2f\n",pb);
	printf("C: %.2f\n",pc);
	printf("D: %.2f\n",pd);
	
	float pbrancos,pnulos;
	pbrancos=(brancos*100)/total;
	pnulos=(nulos*100)/total;
	printf("\nO percentual de votos nulos eh de: %.2f\n",pnulos);
	printf("O percentual de votos brancos eh de: %.2f\n",pbrancos);
	
	int vencedor=0;
	char v;
	if (a>vencedor){
		vencedor=a;
		v='A';
	}
	if (b>vencedor){
		vencedor=b;
		v='B';
		}
	if (c>vencedor){
		vencedor=c;
		v='C';
		}
	if (d>vencedor){
		vencedor=d;
		v='D';
	}
		
		printf("\nO vencedor foi o candidato: %c\n",v);
	
	
	return 0;
}
