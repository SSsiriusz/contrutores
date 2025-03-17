# contrutores
class Carro {
    String marca;
    int ano;

    
    public Carro(String marca, int ano) {
        this.marca = marca;
        this.ano = ano;
    }

    public static void main(String[] args) {
        
        Carro meuCarro = new Carro("Toyota", 2020);

        
        System.out.println("Marca: " + meuCarro.marca);
        System.out.println("Ano: " + meuCarro.ano);
    }
}
class Pessoa {
    String nome;
    int idade;

   
    public Pessoa(String nome, int idade) {
        this.nome = nome;
        this.idade = idade;
    }

    
    public Pessoa() {
        this.nome = "Desconhecido";
        this.idade = 0;
    }

    public static void main(String[] args) {
        
        Pessoa pessoa1 = new Pessoa("João", 25);
        Pessoa pessoa2 = new Pessoa();

        
        System.out.println("Pessoa 1 - Nome: " + pessoa1.nome + ", Idade: " + pessoa1.idade);
        System.out.println("Pessoa 2 - Nome: " + pessoa2.nome + ", Idade: " + pessoa2.idade);
    }
}
class ContaBancaria {
    String titular;
    double saldo;
    String tipoConta;

    
    public ContaBancaria(String titular, double saldo, String tipoConta) {
        this.titular = titular;
        this.saldo = saldo;
        this.tipoConta = tipoConta;
    }

   
    public ContaBancaria(String titular) {
        this.titular = titular;
        this.saldo = 0.0;
        this.tipoConta = "Corrente";
    }

    public static void main(String[] args) {
        
        ContaBancaria conta1 = new ContaBancaria("Carlos", 1000.50, "Poupança");
        ContaBancaria conta2 = new ContaBancaria("Ana");

        
        System.out.println("Conta 1 - Titular: " + conta1.titular + ", Saldo: " + conta1.saldo + ", Tipo: " + conta1.tipoConta);
        System.out.println("Conta 2 - Titular: " + conta2.titular + ", Saldo: " + conta2.saldo + ", Tipo: " + conta2.tipoConta);
    }
}
class Produto {
    String nome;
    double preco;

   
    public Produto(String nome, double preco) {
        this.nome = nome;
        if (preco < 0) {
            this.preco = 0.0;
        } else {
            this.preco = preco;
        }
    }

    public static void main(String[] args) {
        
        Produto produto1 = new Produto("Celular", 500.0);
        Produto produto2 = new Produto("Tablet", -150.0);

        
        System.out.println("Produto 1 - Nome: " + produto1.nome + ", Preço: " + produto1.preco);
        System.out.println("Produto 2 - Nome: " + produto2.nome + ", Preço: " + produto2.preco);
    }
}
