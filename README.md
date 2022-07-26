# Media-salarial-e-valor-de-credito-codigo-em-Java

Considere o seguinte enunciado de um problema:

Um banco concederá um crédito especial aos seus clientes, de acordo com o saldo médio no último ano. Faça um programa que receba o saldo médio de um cliente e calcule o valor do crédito, de acordo com os seguintes critérios:

Caso o saldo médio seja maior que R$ 1000,00, o percentual de crédito será de 30% do saldo médio.
Caso o saldo médio seja maior que R$ 800,00 e menor ou igual a R$ 1000,00, o percentual de crédito será de 25% do saldo médio.
Caso o saldo médio seja maior que R$ 600,00 e menor ou igual a R$ 800,00, o percentual de crédito será de 20% do saldo médio.
Caso o saldo médio seja menor ou igual a R$ 600,00, o percentual de crédito será de 10% do saldo médio.
Mostre o saldo médio e o valor do crédito.

Complete o programa em Java abaixo, arrastando e soltando os códigos nos lugares corretos, de forma que implemente corretamente uma solução para o problema acima.



public class CalculaCredito {
	public static void main(String[] args) {
		[double saldoMedio, valorCredito = 0;]
		
		System.out.print("Saldo medio no ano anterior: ");
		saldoMedio = Double.parseDouble(System.console().readLine());
				
		[if(saldoMedio > 1000)]
			valorCredito = saldoMedio * 30 / 100;
		else [if(saldoMedio > 800)]
			valorCredito = saldoMedio * 25 / 100;
		else [if(saldoMedio > 600)]
			valorCredito = saldoMedio * 20 / 100;
		[else] 
			valorCredito = saldoMedio * 10 / 100;
		
		System.out.printf("\nSALDO MEDIO = R$ %.2f\n", saldoMedio);
		[System.out.printf("VALOR DO CREDITO = R$ %.2f\n", valorCredito);]
	}
}
