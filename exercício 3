using System;

public class Elevador
{
    private int andarAtual;
    private int totalAndares;

    public int AndarAtual
    {
        get { return andarAtual; }
        private set
        {
            if (value < 0)
                andarAtual = 0;
            else if (value > totalAndares)
                andarAtual = totalAndares;
            else
                andarAtual = value;
        }
    }

    public int TotalAndares
    {
        get { return totalAndares; }
    }

    public Elevador(int totalAndares)
    {
        if (totalAndares < 0)
            totalAndares = 0;
        this.totalAndares = totalAndares;
        this.AndarAtual = 0;
    }

    public void Subir()
    {
        if (AndarAtual < totalAndares)
            AndarAtual = AndarAtual + 1;
    }

    public void Descer()
    {
        if (AndarAtual > 0)
            AndarAtual = AndarAtual - 1;
    }
}

class Program
{
    static void Main()
    {
        Elevador e = new Elevador(10);
        Console.WriteLine(e.AndarAtual);
        e.Subir();
        Console.WriteLine(e.AndarAtual);
        e.Subir();
        Console.WriteLine(e.AndarAtual);
        e.Descer();
        Console.WriteLine(e.AndarAtual);
        for (int i = 0; i < 15; i++) e.Subir();
        Console.WriteLine(e.AndarAtual);
        for (int i = 0; i < 20; i++) e.Descer();
        Console.WriteLine(e.AndarAtual);
    }
}
