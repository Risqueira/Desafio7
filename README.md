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

        Tabuada(10);
    }
    public static void Tabuada(int fim){
        int i = 1;
        int n;
        Scanner ler=new Scanner(System.in);
        System.out.println("Digite um numero:");
        n=ler.nextInt();
        while(i<=fim){
            System.out.println(n + " x " + i + " = " + (n * i));
            i++;
        }
    }
}
```
