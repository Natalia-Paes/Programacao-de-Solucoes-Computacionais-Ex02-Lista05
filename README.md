# Programacao-de-Solucoes-Computacionais-Ex02-Lista05
Faça um programa para imprimir:     1     1   2     1   2   3     .....     1   2   3   ...  n para um n informado pelo usuário. Use uma função que receba um valor n inteiro imprima até a n-ésima linha.
import java.util.Scanner;

public class Ex02 {
    public static void main(String[] args) throws Exception {
        System.out.println("Informe um nùmero: ");
        Scanner sc = new Scanner(System.in);
        double numero = sc.nextDouble();
        executN(numero);
        sc.close();

    }

    public static void executN(double numero) {
        for (double a = 1; a <= numero; a++) {
            for (double b = 1; b <= a; b++) {
                System.out.println(b + "");
            }
            System.out.println("");
        }
    }
}
