# Custo_carro_fabrica
O custo de um carro novo ao consumidor é a soma do custo de fábrica com a porcentagem do distribuidor e dos impostos(aplicados ao custo de fábrica). Supondo que o percentual do distribuidor seja de 28% e os impostos de 45%, escrever um algoritmo para ler o custo de fábrica de um carro, calcular e escrever o custo final ao consumidor
using System;

namespace Custo_carro_fabrica
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello!");

            
            Double custoConsumidor;
            Double porcentagemDistribuidor = 28.0;
            Double PercentualImpostos = 45.0;
            Double Destribuidor;
            Double ValorImpostos;

           
            Console.WriteLine("Informe o custo de fábrica de um carro novo");
            double custoFabrica = double.Parse(Console.ReadLine());


            ValorImpostos = (custoFabrica * PercentualImpostos) / 100;

            Destribuidor = (custoFabrica * porcentagemDistribuidor) / 100;

            custoConsumidor = (Destribuidor + ValorImpostos + custoFabrica);

            Console.WriteLine("Valor dos Impostos: " + ValorImpostos);
            Console.WriteLine("Valor do Destribuidor: " + Destribuidor);
            Console.WriteLine("Custo de Fabrica: " + custoFabrica);

            Console.WriteLine("O custo ao consumidor de um carro novo é: " + custoConsumidor);

            Console.ReadKey();
        }
    }

}
