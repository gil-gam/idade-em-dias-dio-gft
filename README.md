# idade-em-dias-dio-gft
Algoritmo que recebe a idade em dias e retorna em anos, meses e dias.

Linguagem: Java

Desafio: Você terá o desafio de ler um valor inteiro correspondente à idade de uma pessoa em dias e informe-a em anos, meses e dias.
Obs.: apenas para facilitar o cálculo, considere todo ano com 365 dias e todo mês com 30 dias. Nos casos de teste nunca haverá uma situação que permite 12 meses e alguns dias, como 360, 363 ou 364. 

Entrada: O arquivo de entrada contém um valor inteiro.
Saída: Imprima a saída conforme exemplo fornecido.

Exemplos de entrada: 
a) 400
b) 800
c) 30;
Exemplos de saída:
a) 1 ano, 1 mês, 5 dias;
b) 2 anos, 2 meses, 10 dias;
c) 0 anos, 1 mês, 0 dias.


Algoritmo:

import java.io.IOException;
import java.util.Scanner;

public class IdadeDias {
	
    public static void main(String[] args) throws IOException {
        Scanner leitor = new Scanner(System.in);
        int idadeDias = leitor.nextInt();
        int anos = idadeDias / 365;
        idadeDias -= anos * 365;
        int meses = idadeDias / 30;
        idadeDias -= meses * 30;
        int dias = idadeDias;
        System.out.println(anos + " ano(s)");
        System.out.println(meses + " mes(es)");
        System.out.println(dias + " dia(s)");
    }
	
}

