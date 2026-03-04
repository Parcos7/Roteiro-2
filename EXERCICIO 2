using System;

public class Carro
{
    private string modelo;
    private int velocidadeAtual;

    public string Modelo
    {
        get { return modelo; }
    }

    public int VelocidadeAtual
    {
        get { return velocidadeAtual; }
        private set
        {
            if (value < 0)
            {
                velocidadeAtual = 0;
            }
            else
            {
                velocidadeAtual = value;
            }
        }
    }

    public Carro(string modelo)
    {
        this.modelo = modelo;
        this.VelocidadeAtual = 0;
    }

    public void Acelerar(int valor)
    {
        if (valor <= 0)
        {
            Console.WriteLine("Valor de aceleração deve ser positivo.");
            return;
        }
        VelocidadeAtual = VelocidadeAtual + valor;
    }

    public void Frear(int valor)
    {
        if (valor <= 0)
        {
            Console.WriteLine("Valor de frenagem deve ser positivo.");
            return;
        }
        VelocidadeAtual = VelocidadeAtual - valor;
    }
}

class Program
{
    static void Main()
    {
        Carro c = new Carro("Ferrari");
        c.Acelerar(50);
        Console.WriteLine(c.VelocidadeAtual);
        c.Frear(30);
        Console.WriteLine(c.VelocidadeAtual);
        c.Frear(50);
        Console.WriteLine(c.VelocidadeAtual); 
    }
}
