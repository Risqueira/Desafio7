# Desafio7
# Questao 1
```java
package desafio7;

import java.util.Scanner;

/**
 *1. Algoritmo para imprimir a tabuada de um número o método recebe
por parâmetro apenas um numero inteiro que é a tabuada que você
quer resolver
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
# questao 2
```java
package desafio7;

import java.util.Scanner;

/**
 * 2. Algoritmo que recebe dois números inteiros e imprime o maior deles.
 *
 * @author henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        Scanner ler = new Scanner(System.in);
        int n1, n2;
        System.out.println("Digite o primeiro valor:");
        n1 = ler.nextInt();
        System.out.println("Digite o segundo valor:");
        n2 = ler.nextInt();
        NumerosInteiros(n1, n2);
    }

    public static void NumerosInteiros(int n1, int n2) {
        if (n1 > n2) {
            System.out.println("Primeiro valor e maior:" + n1);
        } else {
            System.out.println("Segundo valor e maior:" + n2);
        }
    }
}
```
# Questao 3
```java
package desafio7;

import java.util.Scanner;

/**
 * 3. Algoritmo que recebe duas strings e verifica e imprime se “são iguais”
 *
 * @author henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        Scanner ler = new Scanner(System.in);
        String s1, s2;
        System.out.println("Digite uma palavra:");
        s1 = ler.nextLine();
        System.out.println("Digite uma palavra:");
        s2 = ler.nextLine();
        Compara(s1, s2);

    }

    public static void Compara(String x, String y) {
        if (x.equals(y)) {
            System.out.println("Sao iguais");
        } else {
            System.out.println("Nao sao iguais");
        }

    }
}
```
# questao 4
```java
package desafio7;

import java.util.Scanner;

/**
 * 4. Algoritmo que recebe dois números inteiros e imprime o menor deles
 *
 * @author henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        Scanner ler = new Scanner(System.in);
        int n1, n2;
        System.out.println("Digite o primeiro valor:");
        n1 = ler.nextInt();
        System.out.println("Digite o segundo valor:");
        n2 = ler.nextInt();
        NumerosInteiros(n1, n2);
    }

    public static void NumerosInteiros(int n1, int n2) {
        if (n1 < n2) {
            System.out.println("Primeiro valor e menor:" + n1);
        } else {
            System.out.println("Segundo valor e menor:" + n2);
        }
    }
}
```
#questao 5
```java
package desafio7;

import java.util.Scanner;
import javax.swing.JOptionPane;

/**
 * 5. Crie um método que recebe por parâmetro duas strings e retorna um tipo
 * String com as seguintes resposta: “Os nomes são iguais” ou “Os nomes não são
 * iguais”
 *
 * @author henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        Scanner ler = new Scanner(System.in);
        String s1, s2;
        System.out.println("Digite uma palavra:");
        s1 = ler.nextLine();
        System.out.println("Digite uma palavra:");
        s2 = ler.nextLine();
        imprimirTexto(Compara(s1, s2));

    }

    public static String Compara(String x, String y) {
        String resp="Os nomes nao são iguais";
        if (x.equals(y)) {
            resp="Os nomes sao iguais";
        }
        return resp;
    }
    public static void imprimirTexto(String texto) {
        JOptionPane.showMessageDialog(null, texto);
    }
}

```
# QUESTAO 6
```java
package desafio7;

import java.util.Scanner;

/**
 * 6. Crie um método que recebe por parâmetro um tipo double e retorna um tipo
 * double também, calculando a conversão de temperatura de graus Celsius para
 * Fahrenheit – a fórmula para a conversão é (celsius * 1.8) + 32
 *
 * @author Henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        Scanner ler = new Scanner(System.in);
        double celsius, formulaF;
        System.out.println("Digite um valor:");
        celsius = ler.nextDouble();
        conversor(celsius);
    }

    public static double conversor(double c) {
        double formulaF = (c * 1.8) + 32;
        System.out.println("A temperatura de Celsius para Fahrenheit:" + formulaF + "°F");
        return formulaF;
    }

}
```
# Questao 7
```java
package desafio7;

import java.text.DecimalFormat;
import java.util.Scanner;

/**
 * 7. Crie um método para calcular a área de um círculo – o usuário envia por
 * parâmetro o seu raio e retorna o seu resultado (double) – Formula: PI.raio²
 *
 * @author Henrique
 */
public class Desafio7 {

    public static void main(String[] args) {
        Scanner ler = new Scanner(System.in);
        double raio;
        System.out.println("Digite o raio do círculo:");
        raio = ler.nextDouble();
        areaCirculo(raio);

    }

    public static double areaCirculo(double r) {
        DecimalFormat df = new DecimalFormat("0.00");
        double areaC = Math.PI * (Math.pow(r, 2));
        System.out.println("A área do círculo é:" + df.format(areaC));
        return areaC;
    }

}

```
