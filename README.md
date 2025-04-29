# Desafio7
# Questao 1
```java
package desafio7;

import java.util.Scanner;

/**
 *
 * @author henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        int n;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite um numero:");
        n = ler.nextInt();
        Tabuada(n);
    }

    public static void Tabuada(int x) {
        int i = 1;
        int fim = 10;
        while (i <= fim) {
            System.out.println(x + " x " + i + " = " + (x * i));
            i++;
        }
    }
}
```
