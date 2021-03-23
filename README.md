
import java.util.Scanner;
import java.io.PrintStream;

    public class Calculadora{

        public static void main(String[]args){

            Scanner scan = new Scanner(System.in);
            PrintStream show = System.out;

            int n1;
            int n2;
            int resultado;

            show.println("\n### MENU ###");
            show.println("Escolha uma opção a baixo:");
            show.println("1. Somar.");
            show.println("2. Subtrair.");
            show.println("3. Multiplicar.");
            show.println("4. Dividir.");
            show.println("Informe o número da opção e aperte \"Enter\");
            int opcao = scan.nextInt();

            switch(opcao){

                case 1:
                    
                    show.println("Informe um número.");
                    n1 = scan.nextInt();
                    show.println("Informe um número.");
                    n2 = scan.nextInt();

                    resultado = n1 + n2;
                    show.println("O resultado é "+resultado);
                break;

                case 2:
                    show.println("Informe um número.");
                    n1 = scan.nextInt();
                    show.println("Informe um número.");
                    n2 = scan.nextInt();

                    resultado = n1 - n2;
                    show.println("O resultado é "+resultado);    
                break;

                case 3:
                    
                    show.println("Informe um número.");
                    n1 = scan.nextInt();
                    show.println("Informe um número.");
                    n2 = scan.nextInt();

                    resultado = n1 * n2;
                    show.println("O resultado é "+resultado);
                break;

                case 4:
                    
                    show.println("Informe um número.");
                    n1 = scan.nextInt();
                    show.println("Informe um número.");
                    n2 = scan.nextInt();

                    resultado = n1 / n2;
                    show.println("O resultado é "+resultado);
                break;

                default:
                show.println("Opção inválida! tente novamente.");
                
            }
        }
    }
