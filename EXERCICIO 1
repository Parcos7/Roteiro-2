using System;

public class Produto
{
    private string nome;
    private decimal preco;

    public string Nome
    {
        get { return nome; }
    }

    public decimal Preco
    {
        get { return preco; }
        set
        {
            if (value < 0)
            {
                Console.WriteLine("Erro: o preço não pode ser negativo.");
                return;
            }
            preco = value;
        }
    }

    public Produto(string nome, decimal preco)
    {
        this.nome = nome;
        this.Preco = preco;
    }

    public void ExibirDetalhes()
    {
        Console.WriteLine($"Nome: {Nome} | Preço: {Preco.ToString("C")}");
    }
}

class Program
{
    static void Main()
    {
        Produto p = new Produto("Celular", 1500m);
        p.ExibirDetalhes();
        p.Preco = -200m;
        p.ExibirDetalhes();
    }
}
