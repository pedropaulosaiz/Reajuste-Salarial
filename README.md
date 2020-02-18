# Reajuste-Salarial
Programa em C# para fazer reajuste salarial

using System;

class MainClass {
  public static void Main (string[] args) {
    Double salario = 0;
    Double salarioNovo = 0;
    Console.WriteLine("Efetua o reajuste salarial");
    for (int i = 0; i < 3; i++)
    {
    Console.Write("Informe o salário: ");
    salario = Convert.ToDouble(Console.ReadLine());
    if (salario <= 1000)
    { //50%
    salarioNovo = salario + (salario * 0.5);
    }
    else
    { //35%
    salarioNovo = salario + (salario * 0.35);
    }
    Console.WriteLine("Salário reajustado: " + salarioNovo);
    }
    Console.ReadKey();
  }
}
