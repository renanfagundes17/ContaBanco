# ContaBanco
projeto criado po sintaxe em java no modulo da DIO.


import java.util.Scanner;

public class ContaTerminal {
    public static void main(String[] args) {
        // Instanciar a classe Scanner para receber dados do usuário
        Scanner scanner = new Scanner(System.in);

        // Solicitar e capturar os dados da conta
        System.out.println("Por favor, digite o número da Agência:");
        String agencia = scanner.nextLine();

        System.out.println("Por favor, digite o número da Conta:");
        int numero = scanner.nextInt();
        scanner.nextLine(); // Consumir a quebra de linha pendente

        System.out.println("Por favor, digite o nome do Cliente:");
        String nomeCliente = scanner.nextLine();

        System.out.println("Por favor, digite o saldo disponível:");
        double saldo = scanner.nextDouble();

        // Exibir mensagem personalizada com os dados inseridos
        System.out.println("Olá " + nomeCliente + ", obrigado por criar uma conta em nosso banco.");
        System.out.println("Sua agência é " + agencia + ", conta " + numero + " e seu saldo " + saldo + " já está disponível para saque.");

        // Fechar o scanner
        scanner.close();
    }
}

    
