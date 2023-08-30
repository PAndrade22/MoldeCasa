# MoldeCasa
Testando classes
namespace MoldeCarro
{
	public class Carro
	{
		private string nomeDoCarro;
		private string corDoCarro;
		private int anoDoCarro;

		public Carro(string nomeDoCarro, string corDoCarro, int anoDoCarro)
		{
			this.nomeDoCarro = nomeDoCarro;
			this.corDoCarro = corDoCarro;
			this.anoDoCarro = anoDoCarro;
		}
		public string getnomeDoCarro()
		{
			return (nomeDoCarro);
		}
		public string getcorDoCarro()
		{
			return (corDoCarro);
		}
		public int getanoDoCarro()
		{
			return (anoDoCarro);
		}
		public void setnomeDoCarro(string nomeDoCarro)
		{
			this.nomeDoCarro = nomeDoCarro;
		}
		public void setcorDoCarro(string corDoCarro)
		{
			this.corDoCarro = corDoCarro;
		}
		public void setanoDoCarro(int anoDoCarro)
		{
			this.anoDoCarro = anoDoCarro;
		}
		public void Ligar()
		{
			Console.WriteLine("Gire a chave do carro");
			string ligarCarro = Console.ReadLine();
			if (ligarCarro == "L" || ligarCarro == "l")
			{
				Console.WriteLine("O CARRO LIGOU");
			}
			else
			{
				Console.WriteLine("GIRE A CHAVE");
			}
		}
		public void Acelerar()
		{
			Console.WriteLine("Pise no acelerador.");
			string aceleradorDoCarro = Console.ReadLine();
			if (aceleradorDoCarro == "W" || aceleradorDoCarro == "w")
			{
				Console.WriteLine("O CARRO ESTÁ ANDANDO.");
			}
			else
			{
				Console.WriteLine("O CARRO ESTÁ PARADO. PISE NO ACELERADOR.");
			}
		}
		public void Freiar()
		{
			Console.WriteLine("Pise no freio para freiar o carro.");
			string freioDoCarro = Console.ReadLine();
			if (freioDoCarro == "S" || freioDoCarro == "s")
			{
              Console.WriteLine("O CARRO PAROU");
			}
			else
			{
				Console.WriteLine("O CARRO CONTINUA ANDANDO");
			}
		}
	}
	public class Program
 {
	  public static void Main(string[] args)
	{
        string nomeDoCarro = "Fiat", corDoCarro = "Azul";
	    int anoDoCarro = 2019;

	    Carro carroDoAno = new Carro (nomeDoCarro, corDoCarro, anoDoCarro);
		Console.WriteLine("nome do carro " + carroDoAno.getnomeDoCarro());
		Console.WriteLine("A cor do carro " + carroDoAno.getcorDoCarro());
		Console.WriteLine("Ano do carro "+ carroDoAno.getanoDoCarro());
	    carroDoAno.Ligar();
	    carroDoAno.Acelerar();
	    carroDoAno.Freiar();
	}
  }
}
