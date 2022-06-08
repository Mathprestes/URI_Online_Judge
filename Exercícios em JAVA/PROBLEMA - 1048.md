PROBLEMA - 1048 - Aumento de Salário

A empresa ABC resolveu conceder um aumento de salários a seus funcionários de acordo com a tabela abaixo:

![image](https://user-images.githubusercontent.com/67755952/172598612-ae849ae6-89c1-4eda-a820-f86fbab79f2c.png)

Leia o salário do funcionário e calcule e mostre o novo salário, bem como o valor de reajuste ganho e o índice reajustado, em percentual.

Entrada
A entrada contém apenas um valor de ponto flutuante, com duas casas decimais.

Saída
Imprima 3 linhas na saída: o novo salário, o valor ganho de reajuste e o percentual de reajuste ganho, conforme exemplo abaixo.

import java.util.Scanner;

public class Main {
 
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        double A = sc.nextDouble();
        
        if (A <= 400.00) {
            double P = 15;
            int PORC = 15;
            double REAG = A*(P/100);
            double NEW = REAG + A;
            
            System.out.printf ("Novo salario: %.2f\n", NEW);
            System.out.printf ("Reajuste ganho: %.2f\n", REAG);
            System.out.println ("Em percentual: " + PORC + " %");
        }
        else if (A > 400.00 && A <= 800.00){
            double P = 12;
            int PORC = 12;
            double REAG = A*(P/100);
            double NEW = REAG + A;
            
            System.out.printf ("Novo salario: %.2f\n", NEW);
            System.out.printf ("Reajuste ganho: %.2f\n", REAG);
            System.out.println ("Em percentual: " + PORC + " %");
        }
        else if (A > 800.00 && A <= 1200.00){
            double P = 10;
            int PORC = 10;
            double REAG = A*(P/100);
            double NEW = REAG + A;
            
            System.out.printf ("Novo salario: %.2f\n", NEW);
            System.out.printf ("Reajuste ganho: %.2f\n", REAG);
            System.out.println ("Em percentual: " + PORC + " %");
        }
        else if (A > 1200.00 && A <= 2000.00){
            double P = 7;
            int PORC = 7;
            double REAG = A*(P/100);
            double NEW = REAG + A;
            
            System.out.printf ("Novo salario: %.2f\n", NEW);
            System.out.printf ("Reajuste ganho: %.2f\n", REAG);
            System.out.println ("Em percentual: " + PORC + " %");
        }
        else {
            double P = 4;
            int PORC = 4;
            double REAG = A*(P/100);
            double NEW = REAG + A;
            
            System.out.printf ("Novo salario: %.2f\n", NEW);
            System.out.printf ("Reajuste ganho: %.2f\n", REAG);
            System.out.println ("Em percentual: " + PORC + " %");
        }
        sc.close();
		}
    }
