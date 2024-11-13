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

  int opcao = 0;

  while (opcao != 5)
        {
                Console.WriteLine("Escolha uma operação:");
                Console.WriteLine("1. Soma");
                Console.WriteLine("2. Subtração");
                Console.WriteLine("3. Multiplicação");
                Console.WriteLine("4. Divisão");
                Console.WriteLine("5. Sair");
                Console.Write("Opção: ");
                opcao = int.Parse(Console.ReadLine());

  if (opcao == 5) break;

  Console.Write("Digite o primeiro número: ");
                double num1 = double.Parse(Console.ReadLine());
                Console.Write("Digite o segundo número: ");
                double num2 = double.Parse(Console.ReadLine());

  switch (opcao)
                {
                    case 1:
                        Console.WriteLine($"Resultado: {num1 + num2}");
                        break;
                    case 2:
                        Console.WriteLine($"Resultado: {num1 - num2}");
                        break;
                    case 3:
                        Console.WriteLine($"Resultado: {num1 * num2}");
                        break;
                    case 4:
                        if (num2 != 0)
                            Console.WriteLine($"Resultado: {num1 / num2}");
                        else
                            Console.WriteLine("Erro: Divisão por zero.");
                        break;
                    default:
                        Console.WriteLine("Opção inválida.");
                        break;
                }

  }
        }
    }
}
