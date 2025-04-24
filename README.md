# ProjetoDesafio6
Contagem regressiva:
Escreva um programa que exiba uma contagem regressiva de 100 a -100 utilizando um loop while.
 public static void main(String[] args) {
        //declaração 
        int n = 100;

        while (n>= -100) {
            System.out.println(n);
            n--;
        }
    }

    Soma dos números pares:
Escreva um programa que calcule a soma dos números pares de 1 a 20 utilizando um loop while.
 int n = 1;
        int soma = 0;

        while (n <= 20) {
            if (n % 2 == 0) {
                soma += n;
            }
            n++;
        }
        System.out.println("A soma dos números pares de 1 a 20 é: " + soma);
    }
}

Leitura de números até encontrar zero:
Escreva um programa que solicite números ao usuário até que ele insira zero e, em seguida, exiba a soma dos números digitados.
 int numero, soma;
        Scanner Ler = new Scanner(System.in);
        numero = 1;
        soma = 0;
        while (numero != 0) {
            System.out.println("digite um número");
            numero = Ler.nextInt();
            soma += numero;
            System.out.println("a soma dos números é:"+soma);
        }
Exercícios com do-while:

Cálculo de fatorial:
Escreva um programa que calcule o fatorial de um número fornecido pelo usuário usando um loop do-while.
int numero, fatorial, i;
        Scanner ler = new Scanner(System.in);
        fatorial  =   1;
        i  =  1;
        System.out.println("Digite um número");
        numero = ler.nextInt();
        if (numero < 0) {
            System.out.println("Número inválido");
            return;
        }
        do {
            fatorial  *=   i;
            i++;
        } while (i  <=  numero);
        System.out.println("O fatorial de "  + numero +  " é: "  + fatorial);
    }


Jogo de adivinhação:
Escreva um programa que implemente um jogo de adivinhação onde o usuário deve adivinhar um número entre 1 e 100, utilizando um loop do-while para repetir até que o usuário acerte o número. O numero da sorte deverá ser randomizado pelo computador, pesquise como funciona a biblioteca Math.random()
int tentativa, numeroSorte;
        Scanner ler = new Scanner(System.in);
        numeroSorte = (int) (Math.random() * 100) + 1;
        System.out.println("Digite um número de 1 a 100");
        do {
            System.out.println("Digite seu chute");
            tentativa = ler.nextInt();
            if (tentativa < numeroSorte) {
                System.out.println("Tente um número maior.");
            } else if (tentativa > numeroSorte) {
                System.out.println("Tente um número menor.");
            } else {
                System.out.println("Parabéns! Você acertou!");
            }
        } while (tentativa != numeroSorte);
    }


Exercícios com for:

Tabuada de multiplicação:
Escreva um programa que exiba a tabuada de multiplicação de um número fornecido pelo usuário usando um loop for. Você deve informar o numero e de quanto a quanto você quer fazer a tabuada por exemplo: tabuada do 2 de 1 a 20.
int numero, numero1, numero2, i;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite um número");
        numero = ler.nextInt();
        System.out.println("Primeiro número da multiplicação");
        numero1 = ler.nextInt();
        System.out.println("último número da multiplicação");
        numero2 = ler.nextInt();

        System.out.println("Tabuada do " + numero + " de " + numero1 + " até " + numero2);

        for (i = numero1; i <= numero2; i++) {
            System.out.println(numero + " x " + i + " = " + (numero * i));
        }


Soma dos números ímpares:
Escreva um programa que calcule a soma dos números ímpares de 1 a 200 utilizando um loop for.
int soma, i;
        soma = 0;
        for (i = 1; i <= 200; i++) {
            if (i % 2 != 0) {
                soma += i;
            }
        }
        System.out.println("A soma dos números ímpares de 1 a 200 é: " + soma);
    }



