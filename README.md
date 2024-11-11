# Atividade-While-4-Op.-Basicas
Crie um programa que apresente uma calculadora de quatro operações básicas (soma, subtração, multiplicação, divisão). O usuário deve continuar escolhendo operações até optar por sair.

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Ativ._4OpBasicas
{
    public class Program
    {
        static void Main(string[] args)
        {
            int op, cont, i = 1;

            Console.WriteLine("----- Escolha uma Operação: -----");
            Console.WriteLine("ADIÇÃO");
            Console.WriteLine("SUBTRAÇÃO");
            Console.WriteLine("MULTIPLICAÇÃO");
            Console.WriteLine("DIVISÃO");

            op = Convert.ToInt32(Console.ReadLine());

            
            while (i <= 10)
            {
                Console.WriteLine(i);
                i++;
            }
            Console.WriteLine("Deseja Sair? - S/N");
            Console.ReadKey();
        }
    }
}
